# 🔍 3D_Generation Papers · 2026-04-27

[![Total Papers](https://img.shields.io/badge/Papers-6-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Genie Sim PanoRecon: Fast Immersive Scene Generation from Single-View Panorama](https://arxiv.org/abs/2604.07105)**  `arXiv:2604.07105`  `cs.RO`  
  _Zhijun Li, Yongxin Su, Di Yang, Jichao Wang, Zheyuan Xing, Qian Wang, et al._
  <details open><summary>Abstract</summary>
  We present Genie Sim PanoRecon, a feed-forward Gaussian-splatting pipeline that delivers high-fidelity, low-cost 3D scenes for robotic manipulation simulation. The panorama input is decomposed into six non-overlapping cube-map faces, processed in parallel, and seamlessly reassembled. To guarantee geometric consistency across views, we devise a depth-aware fusion strategy coupled with a training-free depth-injection module that steers the monocular feed-forward network to generate coherent 3D Gaussians. The whole system reconstructs photo-realistic scenes in seconds and has been integrated into Genie Sim - a LLM-driven simulation platform for embodied synthetic data generation and evaluation - to provide scalable backgrounds for manipulation tasks. For code details, please refer to:this https URL.
  </details>

- **[What Drives Compositional Generalization? The Importance of Continuous Training Objectives in Visual Generative Models](https://arxiv.org/abs/2510.03075)**  `arXiv:2510.03075`  `cs.CV` `cs.AI` `cs.LG`  
  _Karim Farid, Rajat Sahay, Yumna Ali Alnaggar, Simon Schrodi, Volker Fischer, Cordelia Schmid, et al._
  <details open><summary>Abstract</summary>
  Compositional generalization, the ability to generate novel combinations of known concepts, is a key ingredient for visual generative models. Yet, not all mechanisms that enable or inhibit it are fully understood. In this work, we conduct a systematic study of how various design choices influence compositional generalization in image and video generation in a positive or negative way. Through controlled experiments, we identify two key factors: (i) whether the training objective operates on a discrete or continuous distribution, and (ii) to what extent conditioning provides information about the constituent concepts during training. Building on these insights, we show that relaxing the MaskGIT discrete loss with an auxiliary continuous JEPA-based objective can improve compositional performance in discrete models like MaskGIT.
  </details>

- **[World-R1: Reinforcing 3D Constraints for Text-to-Video Generation](https://arxiv.org/abs/2604.24764)**  `arXiv:2604.24764`  `cs.CV`  
  _Weijie Wang, Xiaoxuan He, Youping Gu, Yifan Yang, Zeyu Zhang, Yefei He, et al._
  <details open><summary>Abstract</summary>
  Recent video foundation models demonstrate impressive visual synthesis but frequently suffer from geometric inconsistencies. While existing methods attempt to inject 3D priors via architectural modifications, they often incur high computational costs and limit scalability. We propose World-R1, a framework that aligns video generation with 3D constraints through reinforcement learning. To facilitate this alignment, we introduce a specialized pure text dataset tailored for world simulation. Utilizing Flow-GRPO, we optimize the model using feedback from pre-trained 3D foundation models and vision-language models to enforce structural coherence without altering the underlying architecture. We further employ a periodic decoupled training strategy to balance rigid geometric consistency with dynamic scene fluidity. Extensive evaluations reveal that our approach significantly enhances 3D consistency while preserving the original visual quality of the foundation model, effectively bridging the gap between video generation and scalable world simulation.
  </details>

- **[Latent Inter-Frame Pruning: A Training-Free Method Bridging Traditional Video Compression and Modern Diffusion Transformers for Efficient Generation](https://arxiv.org/abs/2604.23858)**  `arXiv:2604.23858`  `cs.CV`  
  _Dennis Menn, Chih-Hsien Chou_
  <details open><summary>Abstract</summary>
  Video generation, while capable of generating realistic videos, is computationally expensive and slow, prohibiting real-time applications. In this paper, we observe that video latents encoded via an autoencoder under the Latent Diffusion Model (LDM) framework contain redundancy along the temporal axis. Analogous to how traditional video compression algorithms avoid transmitting redundant frame data, we propose the Latent Inter-frame Pruning framework to prune (skip the re-computation of) duplicated latent patches, thereby reducing computational burden and increasing throughput. However, direct pruning results in visual artifacts due to the discrepancy between full-sequence training and pruned inference. To resolve these artifacts, we propose an Attention Recovery mechanism to bridge the train-inference gap. With our proposed method, we increase video editing throughput by 1.44$\times$, achieving 12.44 FPS on an NVIDIA RTX 6000 while maintaining video quality. We hope our work inspires further research into integrating traditional video compression methods with modern video generation pipelines. This work is a preliminary work on Training-free Latent Inter-Frame Pruning with Attention Recovery.
  </details>

- **[Learning to Credit the Right Steps: Objective-aware Process Optimization for Visual Generation](https://arxiv.org/abs/2604.19234)**  `arXiv:2604.19234`  `cs.CV`  
  _Rui Li, Ke Hao, Yuanzhi Liang, Haibin Huang, Chi Zhang, Yun Gu, et al._
  <details open><summary>Abstract</summary>
  Reinforcement learning, particularly Group Relative Policy Optimization (GRPO), has emerged as an effective framework for post-training visual generative models with human preference signals. However, its effectiveness is fundamentally limited by coarse reward credit assignment. In modern visual generation, multiple reward models are often used to capture heterogeneous objectives, such as visual quality, motion consistency, and text alignment. Existing GRPO pipelines typically collapse these rewards into a single static scalar and propagate it uniformly across the entire diffusion trajectory. This design ignores the stage-specific roles of different denoising steps and produces mistimed or incompatible optimization signals. To address this issue, we propose Objective-aware Trajectory Credit Assignment (OTCA), a structured framework for fine-grained GRPO training. OTCA consists of two key components. Trajectory-Level Credit Decomposition estimates the relative importance of different denoising steps. Multi-Objective Credit Allocation adaptively weights and combines multiple reward signals throughout the denoising process. By jointly modeling temporal credit and objective-level credit, OTCA converts coarse reward supervision into a structured, timestep-aware training signal that better matches the iterative nature of diffusion-based generation. Extensive experiments show that OTCA consistently improves both image and video generation quality across evaluation metrics.
  </details>

- **[SceneScribe-1M: A Large-Scale Video Dataset with Comprehensive Geometric and Semantic Annotations](https://arxiv.org/abs/2604.07990)**  `arXiv:2604.07990`  `cs.CV`  
  _Yunnan Wang, Kecheng Zheng, Jianyuan Wang, Minghao Chen, David Novotny, Christian Rupprecht, et al._
  <details open><summary>Abstract</summary>
  The convergence of 3D geometric perception and video synthesis has created an unprecedented demand for large-scale video data that is rich in both semantic and spatio-temporal information. While existing datasets have advanced either 3D understanding or video generation, a significant gap remains in providing a unified resource that supports both domains at scale. To bridge this chasm, we introduce SceneScribe-1M, a new large-scale, multi-modal video dataset. It comprises one million in-the-wild videos, each meticulously annotated with detailed textual descriptions, precise camera parameters, dense depth maps, and consistent 3D point tracks. We demonstrate the versatility and value of SceneScribe-1M by establishing benchmarks across a wide array of downstream tasks, including monocular depth estimation, scene reconstruction, and dynamic point tracking, as well as generative tasks such as text-to-video synthesis, with or without camera control. By open-sourcing SceneScribe-1M, we aim to provide a comprehensive benchmark and a catalyst for research, fostering the development of models that can both perceive the dynamic 3D world and generate controllable, realistic video content.
  </details>
