# 🔍 Embodied_AI Papers · 2026-02-17

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[ActionCodec: What Makes for Good Action Tokenizers](https://arxiv.org/abs/2602.15397)**  `arXiv:2602.15397`  `cs.RO` `cs.AI`  
  _Zibin Dong, Yicheng Liu, Shiduo Zhang, Baijun Ye, Yifu Yuan, Fei Ni, et al._
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models leveraging the native autoregressive paradigm of Vision-Language Models (VLMs) have demonstrated superior instruction-following and training efficiency. Central to this paradigm is action tokenization, yet its design has primarily focused on reconstruction fidelity, failing to address its direct impact on VLA optimization. Consequently, the fundamental question of \textit{what makes for good action tokenizers} remains unanswered. In this paper, we bridge this gap by establishing design principles specifically from the perspective of VLA optimization. We identify a set of best practices based on information-theoretic insights, including maximized temporal token overlap, minimized vocabulary redundancy, enhanced multimodal mutual information, and token independence. Guided by these principles, we introduce \textbf{ActionCodec}, a high-performance action tokenizer that significantly enhances both training efficiency and VLA performance across diverse simulation and real-world benchmarks. Notably, on LIBERO, a SmolVLM2-2.2B fine-tuned with ActionCodec achieves a 95.5\% success rate without any robotics pre-training. With advanced architectural enhancements, this reaches 97.4\%, representing a new SOTA for VLA models without robotics pre-training. We believe our established design principles, alongside the released model, will provide a clear roadmap for the community to develop more effective action tokenizers.
  </details>

- **[Selective Perception for Robot: Task-Aware Attention in Multimodal VLA](https://arxiv.org/abs/2602.15543)**  `arXiv:2602.15543`  `cs.RO`  
  _Young-Chae Son, Jung-Woo Lee, Yoon-Ji Choi, Dae-Kwan Ko, Soo-Chul Lim_
  <details open><summary>Abstract</summary>
  In robotics, Vision-Language-Action (VLA) models that integrate diverse multimodal signals from multi-view inputs have emerged as an effective approach. However, most prior work adopts static fusion that processes all visual inputs uniformly, which incurs unnecessary computational overhead and allows task-irrelevant background information to act as noise. Inspired by the principles of human active perception, we propose a dynamic information fusion framework designed to maximize the efficiency and robustness of VLA models. Our approach introduces a lightweight adaptive routing architecture that analyzes the current text prompt and observations from a wrist-mounted camera in real-time to predict the task-relevance of multiple camera views. By conditionally attenuating computations for views with low informational utility and selectively providing only essential visual features to the policy network, Our framework achieves computation efficiency proportional to task relevance. Furthermore, to efficiently secure large-scale annotation data for router training, we established an automated labeling pipeline utilizing Vision-Language Models (VLMs) to minimize data collection and annotation costs. Experimental results in real-world robotic manipulation scenarios demonstrate that the proposed approach achieves significant improvements in both inference efficiency and control performance compared to existing VLA models, validating the effectiveness and practicality of dynamic information fusion in resource-constrained, real-time robot control environments.
  </details>

- **[MoIRA: Modular Instruction Routing Architecture for Multi-Task Robotics](https://arxiv.org/abs/2507.01843)**  `arXiv:2507.01843`  `cs.RO`  
  _Dmytro Kuzmenko, Nadiya Shvai_
  <details open><summary>Abstract</summary>
  Mixture-of-Experts (MoE) approaches have recently gained traction in robotics applications due to their ability to dynamically allocate computational resources and specialize sub-networks for distinct tasks or environmental contexts, enabling more efficient decision-making. Such systems often comprise sparsely activated experts combined under a single monolithic architecture and require a well-configured internal routing mechanism, which does not allow for selective low-level expert and router customization and requires additional training. We propose MoIRA, an architecture-agnostic modular MoE framework designed to coordinate existing experts with an external text-based router. MoIRA incorporates two zero-shot routing options: embedding-based similarity and prompt-driven language model inference. In our experiments, we choose large Vision-Language-Action models, gr00t-N1 and $\pi_0$, as the underlying experts, and train low-rank adapters for low-overhead inference. We evaluate MoIRA on various GR1 Humanoid tasks and LIBERO Spatial and Goal benchmarks, where it consistently outperforms generalist models and competes with other MoE pipelines. Additionally, we analyse the robustness of the proposed approach to the variations of the instructions. While relying solely on textual descriptions of tasks and experts, MoIRA demonstrates the practical viability of modular deployment with precise, low-effort routing and provides an alternative, scalable foundation for future multi-expert robotic systems.
  </details>
