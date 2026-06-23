---
title: "GIF: Locally Sound Geometric Information Flow Control for LLMs"
excerpt: "GIF: Locally Sound Geometric Information Flow Control for LLMs<br/><img src='/images/gif-title.png' width='750'>."
collection: projects
link: "https://geomifc.github.io/"
---

*Preprint*

---

Large language models increasingly mediate interactions between sensitive data, untrusted inputs, and privileged actions in modern agentic systems, creating significant security and privacy risks. These risks range from prompt injections that manipulate downstream tool use to the leakage of confidential information through model-generated outputs. Recent Information Flow Control (IFC)-based defenses show promise, but lack a principled semantic foundation for reasoning about information flow through the model itself. Since any input token may influence any output token in an autoregressive LLM, existing approaches suffer from severe taint explosion.

We present *Geometric Information Flow* (GIF), a semantic framework for tracking information flow from input tokens to downstream outputs. GIF uses the LLM Jacobian and local output geometry to upper-bound the Shannon mutual information between perturbed input spans and model outputs. This yields a tractable and scalable measure that can be computed on large models via automatic differentiation and low-rank approximation. Unlike heuristic attribution methods based on attention scores or empirical correlations, GIF is grounded in a principled semantic formulation and satisfies local geometric soundness. We provide a *fully mechanized Lean 4 proof* that GIF upper-bounds the true information flow induced by a given prompt under local regularity assumptions.

We evaluate GIF on integrity and confidentiality tasks across multiple benchmarks spanning various prompt injection attack vectors and privacy-leakage-susceptible scenarios. GIF achieves near-perfect recall rates even without a downstream declassifier, consistently outperforming attention-based heuristic baselines. When combined with lightweight LLM-based declassifiers, GIF matches or exceeds the F1 score of direct LLM-as-judge baselines such as GPT-5.5 xhigh reasoning while using declassifiers with up to 81× lower token cost. We further show that GIF flows detected using small surrogate models transfer to larger state-of-the-art models and other model families, even when the surrogate is up to 200× smaller than the target, suggesting the possibility of using GIF in black-box deployments without gradient access. Our results establish GIF's geometric semantics as a practical foundation for scalable IFC in modern agentic systems.

[Project page](https://geomifc.github.io/) · [Paper (PDF)](https://geomifc.github.io/GIF-paper.pdf) · [Lean 4 proof](https://geomifc.github.io/GIF-lean-proof.zip)
