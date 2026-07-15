<!-- Provide a general summary of your changes in the Title above -->

## Summary

<!-- What does this PR do? Replace <issue-number> with the number of the corresponding task issue. -->

- Closes #<issue-number>

---

## Type of Change

<!-- Mark the type of change your PR introduces. -->

- [ ] 📚 **Documentation** (changes to `.md` files in `content/`)
- [ ] 🎨 **Theme / Layout** (changes to theme files, CSS, layouts)
- [ ] ⚙️ **Configuration** (changes to `hugo.toml`, workflows, etc.)
- [ ] 🐛 **Bug fix**
- [ ] ✨ **New feature**

---

## General Checklist

- [ ] I edited the line `- Closes #<issue-number>`.
- [ ] I wrote clear, imperative commit messages (e.g., "docs: add Russian localization").
- [ ] I reviewed my own diff before requesting review.
- [ ] I understand the changes I'm submitting.
- [ ] I tested the changes locally (`hugo server`) or via preview.
- [ ] GitHub Actions build (Hugo + Vale + Lychee) passes successfully.

---

## 📚 Documentation Checklist

<!-- 
  ⚠️ This section applies ONLY if your PR modifies `.md` files in `content/`.
  If your PR does NOT touch documentation, mark the checkbox below and skip this section:
-->

- [ ] **N/A — This PR does not change documentation** (skip the checklist below)

**If the checkbox above is unchecked, verify the following:**

### Terminology & Voice (STYLEGUIDE Section 3 & Principles 1, 3, 4)
- [ ] "VM" (EN) or "ВМ" (RU) capitalization and first-use rules are strictly followed.
- [ ] No forbidden terms (e.g., "виртуалка", "utilize", "platform" alone).
- [ ] No vague phrases (`various options`, `some settings`, `должным образом`).
- [ ] No marketing language (`easy`, `simple`, `powerful`, `бесшовный`).
- [ ] Actions over nouns (e.g., "Configure the parameters", not "Configuration must be performed").

### Formatting (STYLEGUIDE Section 4)
- [ ] Headings use **sentence case** (e.g., "How to create a virtual machine").
- [ ] **Front Matter titles contain NO Markdown** (e.g., `title: "Create a VM"`, not `title: "**Create a VM**"`).
- [ ] UI labels are **exact, bold, and NOT in quotes** (e.g., Click **QUICK CREATE**, not Click "Quick Create").
- [ ] Russian text uses «ёлочки» for regular text quotes, and straight quotes only for code.
- [ ] Code blocks specify a language (e.g., ` ```bash `).
- [ ] Links use relative paths for internal files (e.g., `../../images/sso.png`).
- [ ] Dates follow the format `Month Day, Year` (e.g., `July 13, 2026`).

### Structure & Content (STYLEGUIDE Section 5 & Principles 2, 5, 6)
- [ ] Numbered lists for sequential steps; bulleted for non-sequential items.
- [ ] Each step starts with an action verb; one action per step.
- [ ] Prerequisites appear **before** the steps, not inside them.
- [ ] Warnings are placed **BEFORE** the step and state the exact **consequence** (not just the risk).
- [ ] The page follows the reader's task, not the system's architecture.

### Localization Readiness (STYLEGUIDE Section 9)
- [ ] If this content exists in English, a corresponding file is added/updated in `content/ru/` (and vice versa).
- [ ] UI labels in Russian translations remain in English and bold (as they appear in the interface).
- [ ] Cross-references use lowercase "см." (RU) or "see" (EN) in parentheses.

---

### Reviewer Checklist

- [ ] I reviewed the linked Issue and verified that this change fully resolves the problem.
- [ ] I checked the live preview (via GitHub Pages deploy) and verified that the changes render correctly (images load, links work).
- [ ] I verified that Vale linter warnings/errors have been addressed or intentionally overridden.