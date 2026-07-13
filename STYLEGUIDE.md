# STYLEGUIDE.md — Innopolis VM Documentation

# Innopolis VM Documentation Style Guide

**Version:** 0.1 (Draft)
**Last updated:** 2026-07-13
**Owner:** Stanislav Saraev
**Status:** Living document — update when you discover new patterns

---

## 1. Purpose & Scope

This guide defines how we write, format, and structure documentation for [Innopolis VM](https://vm.innopolis.university). Its goal is to make our content clear, consistent, and focused on the user's task.

### 👥 Target Audience (Who reads our docs)

Our documentation is read by students, instructors, and staff of Innopolis University. They come to the docs with a specific task, not to admire the writing. Therefore, **the text must not be harder than the system itself**.

We write from the reader's task, not the system's architecture. This means:

- **No assumed sysadmin knowledge:** Explain prerequisites simply or link to definitions (e.g., "What is an SSH key?").
- **Anticipate anxiety:** Users fear breaking things or losing data. Warnings must state the exact consequence (e.g., "This will permanently delete all files. You cannot undo this.").
- **Consistency reduces mental effort:** Using the same term for the same thing everywhere frees the reader's cognitive load for the actual task.

### 🛠️ Who should use this guide

- **Authors** writing or editing documentation
- **Reviewers** checking PRs objectively against these rules
- **Translators** adapting content to Russian
- **New team members** during onboarding

### 📦 What it covers

- **Terminology:** What to call things (and what to avoid)
- **Voice & Tone:** How the product sounds in different situations
- **Structure:** How we organize different types of content
- **Infostyle principles:** How to write clearly and remove verbal noise

---

## 2. Voice & Tone

### Voice (always)

- **Calm** — we don't panic, we don't oversell
- **Direct** — we say what we mean
- **Helpful** — we solve problems, we don't describe features

### Tone (depends on context)

| Situation    | Tone                  | Example                                                            |
| ------------ | --------------------- | ------------------------------------------------------------------ |
| Instructions | Neutral, step-by-step | "Click**Create VM**."                                        |
| Warnings     | Serious, specific     | "This will delete all files. You cannot undo this."                |
| Errors       | Honest, actionable    | "We couldn't connect to the VM. Check your network and try again." |
| Introduction | Welcoming, factual    | "Innopolis VM lets you create virtual machines for your projects." |

### Never do this:

- ❌ "Our powerful and innovative platform..."
- ❌ "Simple and seamless experience..."
- ❌ "We are very sorry you've lost your password..."

### Always do this:

- ✅ "Innopolis VM is a service for creating virtual machines."
- ✅ "To reset your password, enter your email address."
- ✅ "Connection failed. Check your SSH key and try again."

---

## 3. Terminology

### Approved Terms

| Term                   | Definition                    | First use              | After first use                 |
| ---------------------- | ----------------------------- | ---------------------- | ------------------------------- |
| **Innopolis VM** | The service/platform          | Always "Innopolis VM"  | "Innopolis VM" or "the service" |
| **VM**           | Virtual machine               | "virtual machine (VM)" | "VM"                            |
| **SSH key**      | Public key for authentication | "SSH key"              | "SSH key"                       |
| **IP address**   | Network address               | "IP address"           | "IP"                            |
| **Subscription** | Access plan for resources     | "subscription"         | "subscription"                  |
| **Dashboard**    | VM management page            | "dashboard"            | "dashboard"                     |

### Forbidden Terms

| Don't use                         | Use instead            | Why                |
| --------------------------------- | ---------------------- | ------------------ |
| virtual machine (after first use) | VM                     | Brevity            |
| platform, system, service (alone) | Innopolis VM           | Specificity        |
| utilize                           | use                    | Plain language     |
| perform configuration             | configure              | Action over noun   |
| appropriate permissions           | Owner permission       | Specificity        |
| various options                   | [name the options]     | Clarity            |
| easy, simple, powerful            | [show what it does]    | Honesty            |
| seamless, innovative              | [describe the feature] | No marketing noise |

### Interface Labels

Always use **exact labels** from the UI, in **bold**:

- ✅ "Click **Create VM Instance**"
- ❌ "Click the create button"
- ✅ "Select **FROM GALLERY**"
- ❌ "Choose the gallery option"

---

## 4. Grammar & Mechanics

### Capitalization

- **Sentence case** for headings: "How to create a virtual machine"
- **Title Case** for UI labels: "Create VM Instance"
- **Lowercase** for general terms: "virtual machine", "subscription"

### Punctuation

- **Oxford comma:** "create, filter, and export" (not "create, filter and export")
- **Em dash** for parentheticals: "The VM — if running — shows an IP address."
- **Period** at the end of complete sentences in lists

### Dates & Numbers

- **Dates:** "July 13, 2026" (not "13.07.2026" or "07/13/26")
- **Numbers:** Spell out 1–9, use digits for 10+ (except in technical contexts: "port 22", "IP 10.13.127.89")

### Code & Commands

- Always specify language: ``bash`, ``toml`, ````yaml`
- Inline code: `hugo server`, `content/docs/`
- Block code for commands users should copy

### Links

- **Relative paths** for internal links: `../../images/sso.png`
- **Absolute URLs** for external links: `https://vm.innopolis.university`
- **Descriptive link text:** "Visit [Innopolis VM](https://vm.innopolis.university)" (not "click here")

---

## 5. Structure

### Page Anatomy

Every documentation page should follow this pattern:

```
1. Title (what this page covers)
2. Prerequisites (if any)
3. Context (1-2 sentences: why this matters)
4. Steps (numbered, action-first)
5. Expected result (what success looks like)
6. Troubleshooting (if common issues exist)
```

### Headings

- **H2** (`##`) for main sections
- **H3** (`###`) for subsections
- **H4+** — avoid if possible (restructure instead)

### Lists

- **Numbered** for sequential steps
- **Bulleted** for non-sequential items
- **One action per step** — don't combine "click X and then Y"

### Warnings & Notes

- Use Hugo shortcodes if available: `{{< hint warning >}}`
- Place **before** the step, not after
- State the **consequence**, not just the risk

---

## 6. Infostyle Principles

These are our core writing rules, adapted from Infostyle methodology.

### Principle 1: Remove Verbal Noise

Cut words that take space but add no meaning.

| Instead of                            | Write                                |
| ------------------------------------- | ------------------------------------ |
| "in order to"                         | "to"                                 |
| "due to the fact that"                | "because"                            |
| "utilize"                             | "use"                                |
| "perform configuration"               | "configure"                          |
| "functionality for report management" | "create, filter, and export reports" |

### Principle 2: Actions Over Nouns

Instructions run on verbs. Make them visible.

| Instead of                                      | Write                               |
| ----------------------------------------------- | ----------------------------------- |
| "Configuration of parameters must be performed" | "Configure the parameters"          |
| "Account connection is available"               | "To connect your account, go to..." |
| "Selection of the template"                     | "Choose a template"                 |

### Principle 3: Be Specific

Name real things: numbers, roles, limits, consequences.

| Instead of                         | Write                                       |
| ---------------------------------- | ------------------------------------------- |
| "You need appropriate permissions" | "You need Owner permission"                 |
| "Various options are available"    | "You can choose Ubuntu, Debian, or Windows" |
| "As soon as possible"              | "Within 24 hours"                           |

### Principle 4: Be Honest

Show, don't praise. Let the reader decide if it's "easy."

| Instead of                     | Write                          |
| ------------------------------ | ------------------------------ |
| "Our API is easy to integrate" | Show a 3-line code example     |
| "Simple and seamless checkout" | Describe what actually happens |
| "Powerful platform"            | List what it does              |

### Principle 5: Write from the Reader's Task

Follow the user's journey, not the system's architecture.

| Instead of                                                                 | Write                                                                         |
| -------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| "Password recovery functionality is available in the authorization module" | "To reset your password, select**Forgot password** on the sign-in page" |
| "The configuration interface can be accessed via the dashboard"            | "Open the dashboard to configure settings"                                    |

### Principle 6: Show Consequence

Especially for errors, warnings, and confirmations.

| Instead of                         | Write                                                                      |
| ---------------------------------- | -------------------------------------------------------------------------- |
| "Request failed"                   | "We couldn't load the report. Refresh the page or try again later."        |
| "This action may affect your data" | "This will permanently delete all files. You cannot undo this."            |
| "Login is incorrect"               | "The username or password is incorrect. Try again or reset your password." |

---

## 7. Examples: Before & After

### Example 1: Creating a VM

**Before:**

> "The configuration of the relevant parameters must be performed prior to the activation of the service. Users should ensure that all necessary fields are properly filled in order to utilize the functionality."

**After:**

> "Before you create a VM, fill in all required fields: name, password, and subscription. Then click **Create VM Instance**."

### Example 2: Error Message

**Before:**

> "An error has occurred during the connection process. Please try again later."

**After:**

> "We couldn't connect to the VM. Check your SSH key and network connection, then try again."

### Example 3: Feature Description

**Before:**

> "Our platform provides convenient functionality for virtual machine management, allowing users to perform various operations seamlessly."

**After:**

> "You can create, start, stop, and delete VMs from the dashboard."

---

## 8. Localization Notes (EN → RU)

When translating to Russian:

1. **Keep terms consistent** — use the glossary in Section 3
2. **Don't translate UI labels** — keep them in English as they appear in the interface
3. **Adapt sentence structure** — Russian allows longer sentences, but keep Infostyle principles
4. **Test with real users** — what's clear in English may need restructuring in Russian

### RU-specific rules:

- Use "вы" (formal) for all user-facing text
- Avoid passive voice where possible
- Keep technical terms in English when no standard Russian equivalent exists (e.g., "dashboard", "SSH key")

---

## 9. Review Checklist

Before merging a documentation PR, check:

- [ ] Terminology matches Section 3
- [ ] No forbidden terms (Section 3)
- [ ] Headings use sentence case (Section 4)
- [ ] UI labels are exact and bold (Section 3)
- [ ] Steps start with action verbs (Principle 2)
- [ ] No vague phrases like "various options" (Principle 3)
- [ ] No marketing language (Principle 4)
- [ ] Warnings state consequences (Principle 6)
- [ ] Links use relative paths (Section 4)
- [ ] Code blocks specify language (Section 4)

---

## 10. How to Update This Guide

1. **Propose changes** via Pull Request
2. **Discuss** in the PR comments
3. **Merge** when the team agrees
4. **Announce** major changes in the team chat

---

## References

- [Google Developer Style Guide](https://developers.google.com/style)
- [Ozon Style Guide](https://docs.ozon.ru/styleguide)
- [Apple Style Guide](https://support.apple.com/guide/applestyleguide)
- Maxim Ilyakhov, "Пиши, Сокращай" (Infostyle methodology)
- Nora Gal, "Слово живое и мёртвое" (critique of bureaucratic language)

---

*This is a living document. If a rule doesn't work in practice, propose a change.*

---
