## Description
<!-- Please include a summary of the change and which issue is fixed. Include relevant motivation and context. -->

Fixes # (issue number)

## Type of Change
<!-- Please check the relevant option(s) -->
- [ ] 🐛 Bug fix (non-breaking change which fixes an issue)
- [ ] ✨ New Prompt / Analytical Framework
- [ ] 💻 Webapp enhancement / feature
- [ ] 📚 Documentation / Wiki update
- [ ] 🛠️ Refactoring / Maintenance

## Scientific Constraint Checklist
<!--
If your PR introduces or modifies prompts, you MUST check all of the following.
If your PR is only for webapp/docs, check the "Not Applicable" box.
-->
- [ ] **No Internet Data:** The prompt explicitly forbids the use of external knowledge.
- [ ] **Memory-Only:** The prompt relies exclusively on the provided conversational context.
- [ ] **No External Profiling:** The prompt forbids assuming demographics or external traits.
- [ ] **Uncertainty Handling:** The prompt forces the model to state confidence levels (e.g., Low/Mod/High).
- [ ] **Epistemic Boundaries:** The prompt enforces a strict separation between *Observation*, *Inference*, and *Speculation*.
- [ ] **N/A** (This PR does not modify or add prompts).

## Additional Verification
- [ ] My code/prompt follows the style guidelines of this project
- [ ] I have performed a self-review of my own code/prompt
- [ ] I have commented my code/prompt, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation (README, /docs, or Wiki)
- [ ] My changes generate no new warnings or methodology violations

## Output Example (For Prompts)
<!-- If you added a new prompt, please paste a snippet of the generated output here demonstrating that it adheres to the epistemic boundaries. -->
