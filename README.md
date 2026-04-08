# The Pitfalls and Necessity of Verifying AI Artifacts with AI

**Correlated Errors, Cross-Model Validation, and the Architecture of Machine Confidence**

Dusty Wilhelm Murray · Sigmantics AB · March 2026 · v4.0

### When you ask an AI to verify its own output, why does it still fail — and what does a verification architecture that actually works look like?

Asking the same model to check its own work is not 99.84% reliable.  
It is closer to 97–98%.  
And the errors that slip through are the worst kind: confident, plausible, and wrong.

This repo contains the full technical report from **Sigmantics AB** — the problem diagnosis, the proposed hybrid architecture, a five-stage verification pipeline, and a worked demonstration where the paper's own fabricated citation was caught and corrected by the process it describes.

### 📄 The Paper

**[Read the full report → the-pitfalls-and-necessity-of-verifying-ai-artifacts-with-ai-v4.pdf](the-pitfalls-and-necessity-of-verifying-ai-artifacts-with-ai-v4.pdf)**

(12 pages · includes claim taxonomy, confidence scoring function, groundedness escalation protocol, implementation cost model, and the real-world fabricated-citation demonstration)

### What's inside the repo

- `the-pitfalls-and-necessity-of-verifying-ai-artifacts-with-ai-v4.pdf` — the complete technical report
- `the-pitfalls-and-necessity-of-verifying-ai-artifacts-with-ai-v4.docx` — editable source document
- `LICENSE` — CC BY 4.0

### Key takeaway

Same-model verification produces correlated failures. Cross-model validation helps but doesn't eliminate the problem — frontier models increasingly share training data, scaling recipes, and blind spots. The solution is a hybrid pipeline: deterministic tools for factual and mathematical claims, cross-model LLM review for structure and logic, and human escalation for groundedness. A smaller model that fails independently is more valuable than a stronger model that fails in correlated ways.

The goal is not to make AI infallible. The goal is to make AI failure modes **visible, measurable, and auditable** — so that the cost of being wrong is a managed risk rather than an unpriced surprise.

---

**Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)**  
Made with [AssetForge](https://github.com/sigmantics/assetforge) · Sigmantics AB · Stockholm, 2026
