<!-- Provide a general summary of your changes in the Title above -->

## Summary

<!-- What does this PR do?

Replace <issue-number> with the number of the corresponding task issue.

Add more details if necessary.
-->

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

<!-- Go over all the following points, and put an `x` in all the boxes that apply. -->
<!-- If you're unsure about any of these, don't hesitate to ask. We're here to help! -->

- [ ] I edited the line `- Closes #<issue-number>`.
- [ ] I wrote clear commit messages.
- [ ] I reviewed my own diff before requesting review.
- [ ] I understand the changes I'm submitting.
- [ ] I tested the changes I'm submitting.
- [ ] GitHub Actions build passes successfully.

---

## 📚 Documentation Checklist

<!-- 
  ⚠️ This section applies ONLY if your PR modifies `.md` files in `content/`.
  
  If your PR does NOT touch documentation, mark the checkbox below and skip this section:
-->

- [ ] **N/A — This PR does not change documentation** (skip the checklist below)

**If the checkbox above is unchecked, verify the following:**

### Terminology & Voice (Infostyle Principles 1, 3, 4)

- [ ] Terminology matches Section 3 of `STYLEGUIDE.md`
- [ ] No forbidden terms from the glossary (Section 3)
- [ ] No vague phrases: `various options`, `some settings`, `proper configuration`, `as soon as possible`
- [ ] No marketing language: `easy`, `simple`, `powerful`, `seamless`, `innovative`
- [ ] Actions over nouns — no `perform configuration`, `utilize`, `in order to`

### Formatting (Section 4)

- [ ] Headings use **sentence case** (e.g., "How to create a virtual machine")
- [ ] UI labels are **exact and bold** (e.g., "**Create VM Instance**", not "the create button")
- [ ] Code blocks specify a language (e.g., ` ```bash `, ` ```toml `)
- [ ] Links use relative paths for internal files (e.g., `../../images/sso.png`)
- [ ] Links use absolute URLs for external sites (e.g., `https://vm.innopolis.university`)
- [ ] Dates follow the format `Month Day, Year` (e.g., `July 13, 2026`)
- [ ] Numbers: spell out 1–9, use digits for 10+

### Structure & Content (Principles 2, 5, 6)

- [ ] Numbered lists used for sequential steps; bulleted for non-sequential items
- [ ] Each step starts with an action verb
- [ ] One action per step (no "click X and then Y")
- [ ] Prerequisites appear **before** the steps, not inside them
- [ ] Warnings state the **consequence**, not just the risk
- [ ] Error messages explain: what happened → why → what to do next
- [ ] The page follows the reader's task, not the system's architecture

### Localization Readiness (Section 8)

- [ ] If this content should also exist in Russian, a corresponding file is added/updated in `content/ru/`
- [ ] UI labels in Russian translations remain in English (as they appear in the interface)
- [ ] UI labels are exact, bold, and **not** in quotes (Section 3)
- [ ] Technical terms are consistent with the glossary

---

### Reviewer Checklist

- [ ] I reviewed the linked Issue (if applicable) and verified that this change fully resolves the reported problem.
- [ ] I checked the live preview (via GitHub Pages, Vercel, or Netlify) and verified that the changes render correctly.
