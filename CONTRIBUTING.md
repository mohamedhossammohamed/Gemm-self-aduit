# Contributing to Memory-Constrained AI Self-Analysis Systems

First off, thank you for considering contributing to this project! It's people like you that make experimental frameworks like this possible.

This project is a research-oriented lab for **memory-constrained inference** and cognitive reflection experiments. Because of the specific methodological constraints, we ask that all contributors carefully read these guidelines before submitting a pull request or issue.

## Code of Conduct

By participating in this project, you agree to abide by the [Code of Conduct](./CODE_OF_CONDUCT.md). We expect all contributors to follow it in all their interactions with the project.

## Core Scientific Constraints

Before contributing new prompts, examples, or webapp features, please ensure your work respects our core principles:

- ❌ **No internet data:** The model must rely solely on the provided prompt and context.
- ❌ **No retrieval augmentation (RAG):** Do not add mechanisms to fetch external context.
- ❌ **No external profiling:** Avoid assuming personality traits based on external demographic data.
- ❌ **No demographic assumptions:** Do not embed assumptions about the user's background.
- ✅ **Memory-only inference:** Rely entirely on the historical conversation data provided.
- ✅ **Persistent conversational analysis:** Focus on longitudinal observation of patterns over time.
- ✅ **Explicit uncertainty handling:** Prompts must require the model to state its confidence level.
- ✅ **Distinction between evidence and speculation:** Enforce clear separation between observed behavior, inferred patterns, and hypotheses.

## How Can I Contribute?

### 1. Proposing New Prompts

If you have an idea for a new analysis prompt, it should fit into one of the existing categories (Core, Visualization, or Experimental).

When submitting a new prompt:
- Ensure it aligns with our [Core Scientific Constraints](#core-scientific-constraints).
- Use the **Prompt Proposal Issue Template** to discuss the prompt before opening a Pull Request.
- Follow the formatting of existing prompts in the `/prompts` directory.
- Include sections in your prompt that force the model to separate evidence from interpretation.

### 2. Improving Documentation & The Wiki

Good documentation is crucial for an experimental project. You can contribute by:
- Improving the `README.md` or existing files in the `/docs` directory.
- Contributing to the **GitHub Wiki**.

#### How to Contribute to the GitHub Wiki
The documentation is also maintained in the project's GitHub Wiki. Since GitHub Wikis are backed by Git, you can contribute to them in two ways:

**Method 1: Direct Edits (If you have access)**
1. Navigate to the `Wiki` tab on the GitHub repository page.
2. Click `Edit` on any page or `New Page` to create a new one.
3. Write your changes in Markdown and click `Save Page`.

**Method 2: Cloning the Wiki (For complex edits or if you want to propose changes locally)**
Every GitHub Wiki has its own Git repository.
1. Find the Wiki clone URL (usually at the bottom right of the Wiki homepage: `https://github.com/<username>/<repo>.wiki.git`).
2. Clone it to your local machine:
   ```bash
   git clone https://github.com/USERNAME/REPOSITORY.wiki.git
   ```
3. Make your edits locally using Markdown.
4. Commit and push your changes back to the wiki repository.
*(Note: If you do not have direct push access to the wiki, please open a regular issue discussing your proposed wiki changes, or include the markdown files in a Pull Request in the `docs/` folder, and a maintainer will sync it to the Wiki).*

### 3. Reporting Bugs

If you find a bug (e.g., in the webapp, or a prompt that consistently fails to follow constraints), please report it!
- Check existing issues to see if it has already been reported.
- Use the **Bug Report Issue Template** to provide detailed information.
- Provide examples of the inputs that caused the failure, if applicable.

### 4. Suggesting Enhancements

Have an idea for a new feature in the webapp or a structural improvement?
- Check existing issues to avoid duplicates.
- Use the **Feature Request Issue Template** to submit your idea.

## Pull Request Process

1. **Fork the repository** and create your branch from `main`.
2. **Branch naming:** Use a descriptive name like `feature/new-risk-prompt`, `bugfix/webapp-timeline`, or `docs/update-wiki-guide`.
3. If you've added or changed prompts, ensure you've tested them to verify they strictly adhere to the epistemic boundaries.
4. Update the `README.md` or `/docs` if your changes impact the project structure or prompt usage guide.
5. Submit a Pull Request using the provided **Pull Request Template**. Ensure you check off all relevant boxes regarding our scientific constraints.
6. A maintainer will review your PR. Be prepared to discuss your changes and make revisions based on feedback.

## Methodological References

For a deeper understanding of the project's constraints, please read the following before contributing:
- `/docs/methodology.md`
- `/docs/limitations.md`
- `/docs/ethics.md`
- `/manifesto/philosophy.md`

Thank you for contributing to the Memory-Constrained AI Self-Analysis Systems!
