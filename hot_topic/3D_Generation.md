# 🔍 3D_Generation Papers · 2025-09-25

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Conditional Video Generation for High-Efficiency Video Compression](https://arxiv.org/abs/2507.15269)**  `arXiv:2507.15269`  `cs.CV` `cs.AI`  
  _Fangqiu Yi, Jingyu Xu, Jiawei Shao, Chi Zhang, Xuelong Li_
  <details open><summary>Abstract</summary>
  Perceptual studies demonstrate that conditional diffusion models excel at reconstructing video content aligned with human visual perception. Building on this insight, we propose a video compression framework that leverages conditional diffusion models for perceptually optimized reconstruction. Specifically, we reframe video compression as a conditional generation task, where a generative model synthesizes video from sparse, yet informative signals. Our approach introduces three key modules: (1) Multi-granular conditioning that captures both static scene structure and dynamic spatio-temporal cues; (2) Compact representations designed for efficient transmission without sacrificing semantic richness; (3) Multi-condition training with modality dropout and role-aware embeddings, which prevent over-reliance on any single modality and enhance robustness. Extensive experiments show that our method significantly outperforms both traditional and neural codecs on perceptual quality metrics such as Fréchet Video Distance (FVD) and LPIPS, especially under high compression ratios.
  </details>

- **[NewtonGen: Physics-Consistent and Controllable Text-to-Video Generation via Neural Newtonian Dynamics](https://arxiv.org/abs/2509.21309)**  `arXiv:2509.21309`  `cs.CV`  
  _Yu Yuan, Xijun Wang, Tharindu Wickremasinghe, Zeeshan Nadir, Bole Ma, Stanley H. Chan_
  <details open><summary>Abstract</summary>
  A primary bottleneck in large-scale text-to-video generation today is physical consistency and controllability. Despite recent advances, state-of-the-art models often produce unrealistic motions, such as objects falling upward, or abrupt changes in velocity and direction. Moreover, these models lack precise parameter control, struggling to generate physically consistent dynamics under different initial conditions. We argue that this fundamental limitation stems from current models learning motion distributions solely from appearance, while lacking an understanding of the underlying dynamics. In this work, we propose NewtonGen, a framework that integrates data-driven synthesis with learnable physical principles. At its core lies trainable Neural Newtonian Dynamics (NND), which can model and predict a variety of Newtonian motions, thereby injecting latent dynamical constraints into the video generation process. By jointly leveraging data priors and dynamical guidance, NewtonGen enables physically consistent video synthesis with precise parameter control.
  </details>

- **[MotionFlow:Learning Implicit Motion Flow for Complex Camera Trajectory Control in Video Generation](https://arxiv.org/abs/2509.21119)**  `arXiv:2509.21119`  `cs.CV`  
  _Guojun Lei, Chi Wang, Yikai Wang, Hong Li, Ying Song, Weiwei Xu_
  <details open><summary>Abstract</summary>
  Generating videos guided by camera trajectories poses significant challenges in achieving consistency and generalizability, particularly when both camera and object motions are present. Existing approaches often attempt to learn these motions separately, which may lead to confusion regarding the relative motion between the camera and the objects. To address this challenge, we propose a novel approach that integrates both camera and object motions by converting them into the motion of corresponding pixels. Utilizing a stable diffusion network, we effectively learn reference motion maps in relation to the specified camera trajectory. These maps, along with an extracted semantic object prior, are then fed into an image-to-video network to generate the desired video that can accurately follow the designated camera trajectory while maintaining consistent object motions. Extensive experiments verify that our model outperforms SOTA methods by a large margin.
  </details>

- **[A Single Neuron Works: Precise Concept Erasure in Text-to-Image Diffusion Models](https://arxiv.org/abs/2509.21008)**  `arXiv:2509.21008`  `cs.CV`  
  _Qinqin He, Jiaqi Weng, Jialing Tao, Hui Xue_
  <details open><summary>Abstract</summary>
  Text-to-image models exhibit remarkable capabilities in image generation. However, they also pose safety risks of generating harmful content. A key challenge of existing concept erasure methods is the precise removal of target concepts while minimizing degradation of image quality. In this paper, we propose Single Neuron-based Concept Erasure (SNCE), a novel approach that can precisely prevent harmful content generation by manipulating only a single neuron. Specifically, we train a Sparse Autoencoder (SAE) to map text embeddings into a sparse, disentangled latent space, where individual neurons align tightly with atomic semantic concepts. To accurately locate neurons responsible for harmful concepts, we design a novel neuron identification method based on the modulated frequency scoring of activation patterns. By suppressing activations of the harmful concept-specific neuron, SNCE achieves surgical precision in concept erasure with minimal disruption to image quality. Experiments on various benchmarks demonstrate that SNCE achieves state-of-the-art results in target concept erasure, while preserving the model's generation capabilities for non-target concepts. Additionally, our method exhibits strong robustness against adversarial attacks, significantly outperforming existing methods.
  </details>
