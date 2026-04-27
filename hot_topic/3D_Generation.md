# 🔍 3D_Generation Papers · 2026-04-26

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Video Analysis and Generation via a Semantic Progress Function](https://arxiv.org/abs/2604.22554)**  `arXiv:2604.22554`  `cs.CV`  
  _Gal Metzer, Sagi Polaczek, Ali Mahdavi-Amiri, Raja Giryes, Daniel Cohen-Or_
  <details open><summary>Abstract</summary>
  Transformations produced by image and video generation models often evolve in a highly non-linear manner: long stretches where the content barely changes are followed by sudden, abrupt semantic jumps. To analyze and correct this behavior, we introduce a Semantic Progress Function, a one-dimensional representation that captures how the meaning of a given sequence evolves over time. For each frame, we compute distances between semantic embeddings and fit a smooth curve that reflects the cumulative semantic shift across the sequence. Departures of this curve from a straight line reveal uneven semantic pacing. Building on this insight, we propose a semantic linearization procedure that reparameterizes (or retimes) the sequence so that semantic change unfolds at a constant rate, yielding smoother and more coherent transitions. Beyond linearization, our framework provides a model-agnostic foundation for identifying temporal irregularities, comparing semantic pacing across different generators, and steering both generated and real-world video sequences toward arbitrary target pacing.
  </details>

- **[When Models Outthink Their Safety: Unveiling and Mitigating Self-Jailbreak in Large Reasoning Models](https://arxiv.org/abs/2510.21285)**  `arXiv:2510.21285`  `cs.AI` `cs.CL`  
  _Yingzhi Mao, Chunkang Zhang, Junxiang Wang, Xinyan Guan, Boxi Cao, Yaojie Lu, et al._
  <details open><summary>Abstract</summary>
  Large Reasoning Models (LRMs) achieve strong performance on complex multi-step reasoning, yet they still exhibit severe safety failures such as harmful content generation. Existing methods often apply coarse-grained constraints over the entire reasoning trajectories, which can undermine reasoning capability while failing to address the root causes of unsafe behavior. In this work, we uncover a previously underexplored failure mode in LRMs, termed Self-Jailbreak, where models initially recognize the harmful intent of a query, but override this judgment during subsequent reasoning steps, ultimately generating unsafe outputs. Such a phenomenon reveals that LRMs are capable of recognizing harm, while safety failures primarily arise from reasoning steps. Motivated by this finding, we propose Chain-of-Guardrail(CoG), a trajectory-level training framework that mitigates Self-Jailbreak via targeted, step-level interventions while maintaining reasoning ability. Experiments across multiple safety and reasoning benchmarks indicate that CoG achieves a favorable balance between safety and reasoning performance compared with existing approaches.
  </details>

- **[Agentic World Modeling: Foundations, Capabilities, Laws, and Beyond](https://arxiv.org/abs/2604.22748)**  `arXiv:2604.22748`  `cs.AI`  
  _Meng Chu, Xuan Billy Zhang, Kevin Qinghong Lin, Lingdong Kong, Jize Zhang, Teng Tu, et al._
  <details open><summary>Abstract</summary>
  As AI systems move from generating text to accomplishing goals through sustained interaction, the ability to model environment dynamics becomes a central bottleneck. Agents that manipulate objects, navigate software, coordinate with others, or design experiments require predictive environment models, yet the term world model carries different meanings across research communities. We introduce a "levels x laws" taxonomy organized along two axes. The first defines three capability levels: L1 Predictor, which learns one-step local transition operators; L2 Simulator, which composes them into multi-step, action-conditioned rollouts that respect domain laws; and L3 Evolver, which autonomously revises its own model when predictions fail against new evidence. The second identifies four governing-law regimes: physical, digital, social, and scientific. These regimes determine what constraints a world model must satisfy and where it is most likely to fail. Using this framework, we synthesize over 400 works and summarize more than 100 representative systems spanning model-based reinforcement learning, video generation, web and GUI agents, multi-agent social simulation, and AI-driven scientific discovery. We analyze methods, failure modes, and evaluation practices across level-regime pairs, propose decision-centric evaluation principles and a minimal reproducible evaluation package, and outline architectural guidance, open problems, and governance challenges. The resulting roadmap connects previously isolated communities and charts a path from passive next-step prediction toward world models that can simulate, and ultimately reshape, the environments in which agents operate.
  </details>
