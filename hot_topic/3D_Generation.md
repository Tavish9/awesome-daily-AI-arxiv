# 🔍 3D_Generation Papers · 2026-02-15

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Dual-Granularity Contrastive Reward via Generated Episodic Guidance for Efficient Embodied RL](https://arxiv.org/abs/2602.12636)**  `arXiv:2602.12636`  `cs.LG` `cs.RO`  
  _Xin Liu, Yixuan Li, Yuhui Chen, Yuxing Qin, Haoran Li, Dongbin Zhao_
  <details open><summary>Abstract</summary>
  Designing suitable rewards poses a significant challenge in reinforcement learning (RL), especially for embodied manipulation. Trajectory success rewards are suitable for human judges or model fitting, but the sparsity severely limits RL sample efficiency. While recent methods have effectively improved RL via dense rewards, they rely heavily on high-quality human-annotated data or abundant expert supervision. To tackle these issues, this paper proposes Dual-granularity contrastive reward via generated Episodic Guidance (DEG), a novel framework to seek sample-efficient dense rewards without requiring human annotations or extensive supervision. Leveraging the prior knowledge of large video generation models, DEG only needs a small number of expert videos for domain adaptation to generate dedicated task guidance for each RL episode. Then, the proposed dual-granularity reward that balances coarse-grained exploration and fine-grained matching, will guide the agent to efficiently approximate the generated guidance video sequentially in the contrastive self-supervised latent space, and finally complete the target task. Extensive experiments on 18 diverse tasks across both simulation and real-world settings show that DEG can not only serve as an efficient exploration stimulus to help the agent quickly discover sparse success rewards, but also guide effective RL and stable policy convergence independently.
  </details>

- **[SLA2: Sparse-Linear Attention with Learnable Routing and QAT](https://arxiv.org/abs/2602.12675)**  `arXiv:2602.12675`  `cs.LG` `cs.AI` `cs.CV`  
  _Jintao Zhang, Haoxu Wang, Kai Jiang, Kaiwen Zheng, Youhe Jiang, Ion Stoica, et al._
  <details open><summary>Abstract</summary>
  Sparse-Linear Attention (SLA) combines sparse and linear attention to accelerate diffusion models and has shown strong performance in video generation. However, (i) SLA relies on a heuristic split that assigns computations to the sparse or linear branch based on attention-weight magnitude, which can be suboptimal. Additionally, (ii) after formally analyzing the attention error in SLA, we identify a mismatch between SLA and a direct decomposition into sparse and linear attention. We propose SLA2, which introduces (I) a learnable router that dynamically selects whether each attention computation should use sparse or linear attention, (II) a more faithful and direct sparse-linear attention formulation that uses a learnable ratio to combine the sparse and linear attention branches, and (III) a sparse + low-bit attention design, where low-bit attention is introduced via quantization-aware fine-tuning to reduce quantization error. Experiments show that on video diffusion models, SLA2 can achieve 97% attention sparsity and deliver an 18.6x attention speedup while preserving generation quality.
  </details>

- **[Hand2World: Autoregressive Egocentric Interaction Generation via Free-Space Hand Gestures](https://arxiv.org/abs/2602.09600)**  `arXiv:2602.09600`  `cs.CV`  
  _Yuxi Wang, Wenqi Ouyang, Tianyi Wei, Yi Dong, Zhiqi Shen, Xingang Pan_
  <details open><summary>Abstract</summary>
  Egocentric interactive world models are essential for augmented reality and embodied AI, where visual generation must respond to user input with low latency, geometric consistency, and long-term stability. We study egocentric interaction generation from a single scene image under free-space hand gestures, aiming to synthesize photorealistic videos in which hands enter the scene, interact with objects, and induce plausible world dynamics under head motion. This setting introduces fundamental challenges, including distribution shift between free-space gestures and contact-heavy training data, ambiguity between hand motion and camera motion in monocular views, and the need for arbitrary-length video generation. We present Hand2World, a unified autoregressive framework that addresses these challenges through occlusion-invariant hand conditioning based on projected 3D hand meshes, allowing visibility and occlusion to be inferred from scene context rather than encoded in the control signal. To stabilize egocentric viewpoint changes, we inject explicit camera geometry via per-pixel Plücker-ray embeddings, disentangling camera motion from hand motion and preventing background drift. We further develop a fully automated monocular annotation pipeline and distill a bidirectional diffusion model into a causal generator, enabling arbitrary-length synthesis. Experiments on three egocentric interaction benchmarks show substantial improvements in perceptual quality and 3D consistency while supporting camera control and long-horizon interactive generation.
  </details>

- **[R3DPA: Leveraging 3D Representation Alignment and RGB Pretrained Priors for LiDAR Scene Generation](https://arxiv.org/abs/2601.07692)**  `arXiv:2601.07692`  `cs.CV`  
  _Nicolas Sereyjol-Garros, Ellington Kirby, Victor Besnier, Nermin Samet_
  <details open><summary>Abstract</summary>
  LiDAR scene synthesis is an emerging solution to scarcity in 3D data for robotic tasks such as autonomous driving. Recent approaches employ diffusion or flow matching models to generate realistic scenes, but 3D data remains limited compared to RGB datasets with millions of samples. We introduce R3DPA, the first LiDAR scene generation method to unlock image-pretrained priors for LiDAR point clouds, and leverage self-supervised 3D representations for state-of-the-art results. Specifically, we (i) align intermediate features of our generative model with self-supervised 3D features, which substantially improves generation quality; (ii) transfer knowledge from large-scale image-pretrained generative models to LiDAR generation, mitigating limited LiDAR datasets; and (iii) enable point cloud control at inference for object inpainting and scene mixing with solely an unconditional model. On the KITTI-360 benchmark R3DPA achieves state of the art performance. Code and pretrained models are available atthis https URL.
  </details>
