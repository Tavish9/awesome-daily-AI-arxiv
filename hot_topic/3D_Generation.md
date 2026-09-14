# 🔍 3D_Generation Papers · 2026-09-13

[![Total Papers](https://img.shields.io/badge/Papers-2-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[CLAP: Cross-Embodiment Video World Models are Zero-Shot Physical Simulators](https://arxiv.org/abs/2608.27406)**  `arXiv:2608.27406`  `cs.RO` `cs.AI` `cs.CV`  
  _Kechen Liu, Ola Shorinwa_
  <details open><summary>Abstract</summary>
  State-of-the-art action-conditioned video models are typically restricted to a single robot embodiment, preventing them from leveraging the vast corpus of heterogeneous video data that contains rich signals for learning generalizable physics. To bridge this gap, we introduce CLAP, a framework for cross-embodiment action-conditioned video generation capable of being trained on diverse, internet-scale videos across human and robotic agents. CLAP is grounded in the insight that universal physical laws govern spatiotemporal dynamics regardless of the actor. However, cross-embodiment learning is non-trivial because action representations vary sharply across robot platforms and are typically absent in human videos. CLAP addresses this fundamental challenge through the following core contributions. First, CLAP reconciles disparate action spaces using end-effector poses, language instructions, and latent actions. Second, to resolve their individual limitations, CLAP introduces a curriculum-based cross-embodiment learning recipe that first learns foundational physical priors across unlabeled video data using latent actions and subsequently grounds them in end-effector action spaces for zero-shot deployment to real-world tasks. Crucially, CLAP approaches or surpasses state-of-the-art single-embodiment video models in challenging environments like DROID. These performance advantages compound via few-shot adaptation to establish a novel paradigm for training single-embodiment video world models. Ultimately, CLAP delivers the most comprehensive suite of action-conditioned video world models to date - spanning diverse action-conditioning spaces (end-effector, language, and latent) and robot morphologies (including cross-embodiment, DROID, Bridge, bimanual YAM robots, and G1 humanoids). We open-source all code and models. Project Website atthis https URL.
  </details>

- **[Physics-Aware Video Generation via Agentic Planning and Graph-Guided Optimization](https://arxiv.org/abs/2609.13006)**  `arXiv:2609.13006`  `cs.CV`  
  _Minh-Loi Nguyen, Xuan-Vu Le, Thanh-Toan Do, Tam V. Nguyen, Minh-Triet Tran, Trung-Nghia Le_
  <details open><summary>Abstract</summary>
  Video diffusion models (VDMs) have demonstrated remarkable capabilities in synthesizing high-fidelity, photorealistic video content. However, they fundamentally lack an intrinsic understanding of physical laws and frequently produce visually appealing but causally illogical sequences characterized by structural hallucinations and physically implausible dynamics. Injecting physical awareness via training-free test-time optimization is a promising alternative, yet existing methods rely on global gradient updates and rigid scheduling heuristics that inadvertently corrupt passive backgrounds and fail to model complex dynamic state changes. To address this, we propose PhysPlan, a novel training-free guidance framework that shifts the paradigm from stochastic visual interpolation to agentic physics simulation. First, a VLM operates as an iterative cognitive simulator, decomposing multimodal inputs into a Chain-of-Visual-Thought to create a multimodal representation of kinematic trajectories and 3D depth geometries. Second, these signals drives an object-centric test-time optimization. Unlike prior training-free methods that rely on global gradients and rigid scheduling heuristics, PhysPlan introduces Object-Centric Gradient Routing to isolate kinematic modifications and completely lock the passive environment. Furthermore, our Kinetic Intensity Profiling dynamically parameterizes framework hyperparameters to accommodate the varying severity of physical deformations. Extensive evaluations on the PhyGenBench and Physics-IQ benchmarks demonstrate that PhysPlan significantly outperforms both foundational and controllable VDM baselines, offering a promising approach for improving the physical understanding of video generation.
  </details>
