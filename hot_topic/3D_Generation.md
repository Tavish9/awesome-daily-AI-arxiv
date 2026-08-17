# 🔍 3D_Generation Papers · 2026-08-16

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[ForgeWM: Progressive Causal Training for Few-Step Action-Conditioned Video World Models](https://arxiv.org/abs/2608.14022)**  `arXiv:2608.14022`  `cs.CV` `cs.AI`  
  _Xinye Li, Lingshuai Lin, Lei Wang, Liuzhou Zhang, Jialin Cui, Qingshan Li, et al._
  <details open><summary>Abstract</summary>
  Action-conditioned video world models require low-latency causal generation and reliable responses to game-native controls. Although causal distillation enables one- or few-step video synthesis, extending it to interactive world models remains challenging, as discrete keyboard states and continuous mouse motion must remain aligned with temporally compressed latent chunks during causal training and autoregressive rollout. We introduce ForgeWM, a progressive framework that transforms a bidirectional action-conditioned video generator into efficient few-step world models through domain adaptation, teacher-forced causal training, causal consistency distillation, and on-policy distribution matching with a bidirectional teacher. The resulting budget-specialized students operate at steady-state denoising budgets of 1, 2, and 4 steps. ForgeWM further supports a dual-path deployment protocol combining latency-critical interaction with optional replay-time refinement, where the one-step student re-noises and refines its saved draft. On paired Minecraft trajectories, ForgeWM leads the evaluated systems in Imaging Quality, reference-aligned motion-profile agreement, action-sign accuracy, and mouse-control accuracy, while achieving the lowest reference LPIPS; the same four-stage recipe transfers to gamepad-controlled FPS gameplay. Replay-time refinement matches four-step reference quality while remaining roughly three times closer to the experienced trajectory than regeneration from noise. These results demonstrate ForgeWM's effectiveness for controllable few-step video generation.
  </details>

- **[Beyond Text Conditioning: A Systematic Study of MLLM-DiT Fusion for Video Generation](https://arxiv.org/abs/2608.14043)**  `arXiv:2608.14043`  `cs.CV`  
  _Yanbo Ding, Yijia Fan, Caihua Shan, Yifan Yang, Yifei Shen, Weijie Wang, et al._
  <details open><summary>Abstract</summary>
  Diffusion Transformers (DiTs) have become the dominant paradigm for high-fidelity video generation, yet their ability to perform high-level semantic planning remains limited. While hybrid architectures integrating MLLMs with diffusion backbones have shown strong advantages in image synthesis, such designs remain underexplored in video generation, where existing approaches often treat MLLMs primarily as frozen feature encoders rather than semantic generators. To fill this gap, we systematically study how an MLLM should be integrated with a DiT for video generation by answering three questions: what intermediate representation should bridge the MLLM and DiT, how the MLLM should generate it, and how the DiT should incorporate it during diffusion rendering. Our analysis reveals three key findings: (1) discrete semantic visual tokens produced by an EMA-based tokenizer provide a stable and expressive interface, (2) autoregressive causal modeling is effective for generating these tokens, and (3) explicit visual-token conditioning is more effective than prompt refinement or latent bridging. Based on these findings, we propose BiVidGen, a hybrid framework where an MLLM first generates semantic visual tokens and a DiT renders videos conditioned on both text and these tokens via multi-layer cross-attention. Extensive experiments show that BiVidGen improves semantic alignment and temporal coherence over a fine-tuned DiT baseline, achieving stronger performance on VBench-Long. These results demonstrate that explicit MLLM-based visual planning provides an effective intermediate interface for text-to-video generation beyond text-only conditioning.
  </details>

- **[Spatially-Grounded Text-to-Video Generation via Inference-Time Gradient-Free Optimization](https://arxiv.org/abs/2608.13037)**  `arXiv:2608.13037`  `cs.CV`  
  _Guillaume Jeanneret, Mathis Koroglu, Hugo Caselles-Dupré, Arnaud Dapogny, Matthieu Cord_
  <details open><summary>Abstract</summary>
  Diffusion Transformer Text-to-Video models have achieved remarkable synthesis quality, yet fine-grained spatial controllability remains a significant challenge. While existing training-free methods produce solid overall results in spatially grounded generation, \ie, placing a specific object in a designated location, they rely on gradient-based optimization techniques that incur prohibitive computational overhead, a bottleneck amplified in modern large-scale architectures. To address this limitation, we present Gradient-free Analytical Trajectory Optimization Video Generation (GATO-Vid), a novel training-free and gradient-free approach for precise spatial guidance. Rather than relying on costly backward passes, we introduce an alternative cross-attention score and solve it analytically to obtain an exact, closed-form solution. To use our analytical solution, we propose an on-the-fly injection mechanism tailored to the topological manifold of the transformer's latent space. Our experiments demonstrate that GATO-Vid significantly outperforms existing baselines in localization accuracy while introducing minimal computational overhead.
  </details>

- **[HandsOnWorld: Unconstrained Egocentric Video Generation with Camera-Disentangled Hand Control](https://arxiv.org/abs/2607.02075)**  `arXiv:2607.02075`  `cs.CV`  
  _Yushuo Chen, Xiaoyu Shi, Xiaoshi Wu, Xintao Wang, Pengfei Wan, Yebin Liu_
  <details open><summary>Abstract</summary>
  We present HandsOnWorld, a framework for hand-controlled egocentric video generation that learns directly from unconstrained monocular video. Prior generators depend on 3D hand annotations from multi-view or marker-based motion capture, confining them to narrow, instrumented scene distributions. To bridge this gap, we introduce a protagonist-centered annotation pipeline that filters monocular 3D reconstructions at the action-semantic, image-quality, and 3D-geometric levels, yielding EgoVid-Pro, a dataset of clean, protagonist-only hand trajectories spanning 103K clips and roughly 12M frames across diverse everyday scenes. These unconstrained scenes exhibit substantial camera ego-motion that is largely absent from tabletop captures, exposing the entanglement of camera and hand motion in existing camera-space control signals. We therefore propose the Plücker Hand Map, which extends Plücker rays from camera geometry to the hand surface, representing hand motion in the same world frame as the camera and disentangling the two motion sources at the representation level. Experiments show that HandsOnWorld outperforms prior methods in visual fidelity and control accuracy and generalizes beyond laboratory settings.
  </details>
