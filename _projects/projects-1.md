---
title: "Mechanics of Learned Reasoning 1: TempoBench"
excerpt: "Mechanics of Learned Reasoning 1: TempoBench<br/><img src='/images/tempobench.png' width="500">. <a href="reasoning.nikolausholzer.com">project page</a>"
collection: portfolio
link: "https://reasoning.nikolausholzer.com/mlr/mlr1/"
---

This is a shortened version of the full article available on my research website.

---

As a small teaser and good high level overview, please enjoy our **paper abstract:**

<div class="full-width-image">

![Performance overview](../../../assets/overview.png)

</div>

---

Large Language Models (LLMs) are increasingly excelling and outpacing human performance on many tasks. However, to improve LLM reasoning, researchers either rely on ad-hoc generated datasets or formal mathematical proof systems such as the Lean proof assistant. Whilst ad-hoc generated methods can capture the decision chains of real-world reasoning processes, they may encode some inadvertent bias in the space of reasoning they cover; they also cannot be formally verified. On the other hand, systems like Lean can guarantee verifiability, but are not well-suited to capture the nature of agentic decision chain-based tasks. This creates a gap both in performance for functions such as business agents or code assistants, and in the usefulness of LLM reasoning benchmarks, whereby these fall short in reasoning structure or real-world alignment. We introduce TempoBench, the first formally grounded and verifiable diagnostic benchmark that parametrizes difficulty to systematically analyze how LLMs perform reasoning. TempoBench uses two evaluation benchmarks to break down reasoning ability. First, temporal trace evaluation (TTE) tests the ability of an LLM to understand and simulate the execution of a given multi-step reasoning system. Subsequently, temporal causal evaluation (TCE) tests an LLM's ability to perform multi-step causal reasoning and to distill cause-and-effect relations from complex systems. We find that models score 65.6% on TCE-normal, and 7.5% on TCE-hard. This shows that state-of-the-art (sota) LLMs clearly understand the TCE task but perform poorly as system complexity increases. Our code is available at our [GitHub repository](https://github.com/nik-hz/tempobench), you can find the paper on [Arxiv](https://arxiv.org/abs/2510.27544).
