---
title: "TempoBench: Evaluating Temporal Causal Reasoning in Large Language Models"
excerpt: "TempoBench: Evaluating Temporal Causal Reasoning in Large Language Models<br/><img src='/images/tempobench-title.png' width='750'>."
collection: projects
link: "https://arxiv.org/abs/2510.27544"
---

**Nikolaus Holzer, William Fishell, Baishakhi Ray, Mark Santolucito** — Columbia University

*COLM 2026*

---

Temporal reasoning involves understanding how systems evolve over time through input-driven state transitions. A key aspect is *temporal causal reasoning*: causally reasoning about what prior inputs were necessary in causing an observed outcome. While large language models (LLMs) perform well at forward simulation, predicting outputs from inputs, they struggle to identify the minimal causal inputs of outcomes. To study this distinction, we define two tasks: *trace simulation* (SIM), which requires models to simulate system execution, and *minimal causal attribution* (MIN), which identifies the minimal set of inputs necessary for a given outcome. We introduce TempoBench, the first formally verified benchmark for temporal causal reasoning, built from synthesized Mealy machines with controllable complexity and provably correct causal labels. Across frontier models, we observe that despite achieving up to 96% accuracy on the SIM task, performance on the causal attribution MIN task drops below 25%; models fail to reason about causal necessity. Over 94% of causal errors involve overspecification, where models perform retrieval and list all possible inputs rather than reasoning about the minimal causal subset. Fine-tuning on TempoBench training corpus improves causal reasoning and generalizes better than math, code, or instruction training, with gains across standard reasoning benchmarks.

![TempoBench pipeline](/images/tb-pipeline.png)

![Feature importance for MIN task](/images/tb-feature-importance.png)

[arXiv](https://arxiv.org/abs/2510.27544) · [GitHub](https://github.com/nik-hz/tempobench)
