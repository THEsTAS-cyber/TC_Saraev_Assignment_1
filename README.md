# Innopolis VM Documentation

This repository contains the official user documentation for **Innopolis VM**. It has been transformed from a basic collection of Markdown files into a modern, production-ready **Docs as Code** ecosystem. 

By combining deterministic automation, strategic AI usage, and clear standards, the documentation process is now predictable, scalable, and user-centric.

---

## 🌐 Live Environments

*   🚀 **Production**: [https://thestas-cyber.github.io/TC_Saraev_Assignment_1/](https://thestas-cyber.github.io/TC_Saraev_Assignment_1/)
*   🚧 **Stage (Preview)**: [https://thestas-cyber.github.io/TC_Saraev_Assignment_1/stage/](https://thestas-cyber.github.io/TC_Saraev_Assignment_1/stage/)

---

## 🚀 Key Improvements & Transformations

### 1. Repository Configuration & Workflow
*   Created two protected branches (`stage` and `main`) to enforce quality control.
*   Added issue and pull request templates that require at least one review before merging.
*   Created a project board for tracking user stories and pending tasks.

### 2. Foundation and Standards
Automation requires clear rules. I established a single source of truth by creating a comprehensive [`STYLEGUIDE.md`](STYLEGUIDE.md). It enforces strict rules: unified terminology (e.g., first use of "virtual machine (VM)", then strictly "VM") and precise UI formatting (exact interface labels in **bold**, never in quotes). The entire documentation was restructured into a logical, task-oriented flow: *Welcome → Setup → Basics → Functions → Troubleshoot → Reference*.

### 3. Deterministic Automation (CI/CD)
To prevent human error, I built a GitHub Actions pipeline that automatically validates every Pull Request for both English and Russian versions:
*   **Style & Terminology:** `Vale` enforces the `STYLEGUIDE.md` rules.
*   **Spell Checking:** `CSpell` (English) and `LanguageTool` (Russian) catch typos and grammatical errors.
*   **Link & Image Verification:** `Lychee` ensures zero broken links or missing images in the built site.
*   **Commit Linting:** A custom script enforces *Conventional Commits* for a clean Git history.
*   **Dual Environments:** The pipeline builds and deploys to a `stage` environment for safe review, and `main` for production.

### 4. Generative Approach (AI & Content Refinement)
AI was used strategically to enhance quality, not to blindly generate content, strictly following the rule that *every sentence must be verifiable*:
*   **Translation & Localization:** AI assisted in translating docs to Russian. Using prompt engineering (Persona and Constraint patterns), I ensured UI labels remained in English and the tone matched the target audience. Every output was manually fact-checked.
*   **Rephrasing for Clarity:** Applied Infostyle principles to remove verbal noise and use active voice (e.g., changing *"You can see the details of creation..."* to *"To view the creation progress..."*).
*   **Structural Improvements:** Explicitly clarified the difference between **Quick Create** and **From Gallery**. Redesigned the Troubleshooting section into a diagnostic framework: *Symptom → Possible causes → Checks → Solutions → Escalation*.

### 5. Monitoring and Feedback
To track user flow and gather actionable feedback for continuous improvement:
*   **GoatCounter Analytics:** Tracks page views and popular content in the *production* environment only, ensuring privacy and avoiding test-data pollution. Available at [Goat Counter](https://thestas-cyber.goatcounter.com/)
*   **Automated Feedback Loop:** Added bilingual "Was this page helpful? 👍 / 👎" buttons. Clicking them automatically generates a GitHub Issue with a pre-filled title and the exact page URL, turning passive readers into active contributors.

---

## 🛠️ Tech Stack

*   **Static Site Generator:** Hugo (Extended)
*   **Theme:** [Hugo Book](https://github.com/alex-shpak/hugo-book)
*   **CI/CD:** GitHub Actions
*   **Linting & Validation:** Vale, CSpell, LanguageTool, Lychee
*   **Analytics:** GoatCounter

---

## 💻 Local Development

To run the documentation locally, you need [Hugo Extended](https://gohugo.io/installation/) installed.

1. Clone the repository:
   ```bash
   git clone https://github.com/THEsTAS-cyber/TC_Saraev_Assignment_1.git
   cd TC_Saraev_Assignment_1
