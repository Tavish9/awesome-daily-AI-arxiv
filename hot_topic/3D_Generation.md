# 🔍 3D_Generation Papers · 2026-02-18

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Factored Latent Action World Models](https://arxiv.org/abs/2602.16229)**  `arXiv:2602.16229`  `cs.LG`  
  _Zizhao Wang, Chang Shi, Jiaheng Hu, Kevin Rohling, Roberto Martín-Martín, Amy Zhang, et al._
  <details open><summary>Abstract</summary>
  Learning latent actions from action-free video has emerged as a powerful paradigm for scaling up controllable world model learning. Latent actions provide a natural interface for users to iteratively generate and manipulate videos. However, most existing approaches rely on monolithic inverse and forward dynamics models that learn a single latent action to control the entire scene, and therefore struggle in complex environments where multiple entities act simultaneously. This paper introduces Factored Latent Action Model (FLAM), a factored dynamics framework that decomposes the scene into independent factors, each inferring its own latent action and predicting its own next-step factor value. This factorized structure enables more accurate modeling of complex multi-entity dynamics and improves video generation quality in action-free video settings compared to monolithic models. Based on experiments on both simulation and real-world multi-entity datasets, we find that FLAM outperforms prior work in prediction accuracy and representation quality, and facilitates downstream policy learning, demonstrating the benefits of factorized latent action models.
  </details>

- **[Quant VideoGen: Auto-Regressive Long Video Generation via 2-Bit KV-Cache Quantization](https://arxiv.org/abs/2602.02958)**  `arXiv:2602.02958`  `cs.LG`  
  _Haocheng Xi, Shuo Yang, Yilong Zhao, Muyang Li, Han Cai, Xingyang Li, et al._
  <details open><summary>Abstract</summary>
  Despite rapid progress in autoregressive video diffusion, an emerging system algorithm bottleneck limits both deployability and generation capability: KV cache memory. In autoregressive video generation models, the KV cache grows with generation history and quickly dominates GPU memory, often exceeding 30 GB, preventing deployment on widely available hardware. More critically, constrained KV cache budgets restrict the effective working memory, directly degrading long horizon consistency in identity, layout, and motion. To address this challenge, we present Quant VideoGen (QVG), a training free KV cache quantization framework for autoregressive video diffusion models. QVG leverages video spatiotemporal redundancy through Semantic Aware Smoothing, producing low magnitude, quantization friendly residuals. It further introduces Progressive Residual Quantization, a coarse to fine multi stage scheme that reduces quantization error while enabling a smooth quality memory trade off. Across LongCat Video, HY WorldPlay, and Self Forcing benchmarks, QVG establishes a new Pareto frontier between quality and memory efficiency, reducing KV cache memory by up to 7.0 times with less than 4% end to end latency overhead while consistently outperforming existing baselines in generation quality.
  </details>

- **[A Survey: Spatiotemporal Consistency in Video Generation](https://arxiv.org/abs/2502.17863)**  `arXiv:2502.17863`  `cs.CV` `cs.AI`  
  _Zhiyu Yin, Kehai Chen, Xuefeng Bai, Ruili Jiang, Juntao Li, Hongdong Li, et al._
  <details open><summary>Abstract</summary>
  Video generation aims to produce temporally coherent sequences of visual frames, representing a pivotal advancement in Artificial Intelligence Generated Content (AIGC). Compared to static image generation, video generation poses unique challenges: it demands not only high-quality individual frames but also strong temporal coherence to ensure consistency throughout the spatiotemporal sequence. Although research addressing spatiotemporal consistency in video generation has increased in recent years, systematic reviews focusing on this core issue remain relatively scarce. To fill this gap, this paper views the video generation task as a sequential sampling process from a high-dimensional spatiotemporal distribution, and further discusses spatiotemporal consistency. We provide a systematic review of the latest advancements in the field. The content spans multiple dimensions including generation models, feature representations, generation frameworks, post-processing techniques, training strategies, benchmarks and evaluation metrics, with a particular focus on the mechanisms and effectiveness of various methods in maintaining spatiotemporal consistency. Finally, this paper explores future research directions and potential challenges in this field, aiming to provide valuable insights for advancing video generation technology. The project link isthis https URL.
  </details>
