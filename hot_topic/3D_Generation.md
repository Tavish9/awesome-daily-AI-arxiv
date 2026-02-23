# 🔍 3D_Generation Papers · 2026-02-22

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Generated Reality: Human-centric World Simulation using Interactive Video Generation with Hand and Camera Control](https://arxiv.org/abs/2602.18422)**  `arXiv:2602.18422`  `cs.CV`  
  _Linxi Xie, Lisong C. Sun, Ashley Neall, Tong Wu, Shengqu Cai, Gordon Wetzstein_
  <details open><summary>Abstract</summary>
  Extended reality (XR) demands generative models that respond to users' tracked real-world motion, yet current video world models accept only coarse control signals such as text or keyboard input, limiting their utility for embodied interaction. We introduce a human-centric video world model that is conditioned on both tracked head pose and joint-level hand poses. For this purpose, we evaluate existing diffusion transformer conditioning strategies and propose an effective mechanism for 3D head and hand control, enabling dexterous hand--object interactions. We train a bidirectional video diffusion model teacher using this strategy and distill it into a causal, interactive system that generates egocentric virtual environments. We evaluate this generated reality system with human subjects and demonstrate improved task performance as well as a significantly higher level of perceived amount of control over the performed actions compared with relevant baselines.
  </details>

- **[Predict to Skip: Linear Multistep Feature Forecasting for Efficient Diffusion Transformers](https://arxiv.org/abs/2602.18093)**  `arXiv:2602.18093`  `cs.CV`  
  _Hanshuai Cui, Zhiqing Tang, Qianli Ma, Zhi Yao, Weijia Jia_
  <details open><summary>Abstract</summary>
  Diffusion Transformers (DiT) have emerged as a widely adopted backbone for high-fidelity image and video generation, yet their iterative denoising process incurs high computational costs. Existing training-free acceleration methods rely on feature caching and reuse under the assumption of temporal stability. However, reusing features for multiple steps may lead to latent drift and visual degradation. We observe that model outputs evolve smoothly along much of the diffusion trajectory, enabling principled predictions rather than naive reuse. Based on this insight, we propose \textbf{PrediT}, a training-free acceleration framework that formulates feature prediction as a linear multistep problem. We employ classical linear multistep methods to forecast future model outputs from historical information, combined with a corrector that activates in high-dynamics regions to prevent error accumulation. A dynamic step modulation mechanism adaptively adjusts the prediction horizon by monitoring the feature change rate. Together, these components enable substantial acceleration while preserving generation fidelity. Extensive experiments validate that our method achieves up to $5.54\times$ latency reduction across various DiT-based image and video generation models, while incurring negligible quality degradation.
  </details>

- **[A Single Image and Multimodality Is All You Need for Novel View Synthesis](https://arxiv.org/abs/2602.17909)**  `arXiv:2602.17909`  `cs.CV`  
  _Amirhosein Javadi, Chi-Shiang Gau, Konstantinos D. Polyzos, Tara Javidi_
  <details open><summary>Abstract</summary>
  Diffusion-based approaches have recently demonstrated strong performance for single-image novel view synthesis by conditioning generative models on geometry inferred from monocular depth estimation. However, in practice, the quality and consistency of the synthesized views are fundamentally limited by the reliability of the underlying depth estimates, which are often fragile under low texture, adverse weather, and occlusion-heavy real-world conditions. In this work, we show that incorporating sparse multimodal range measurements provides a simple yet effective way to overcome these limitations. We introduce a multimodal depth reconstruction framework that leverages extremely sparse range sensing data, such as automotive radar or LiDAR, to produce dense depth maps that serve as robust geometric conditioning for diffusion-based novel view synthesis. Our approach models depth in an angular domain using a localized Gaussian Process formulation, enabling computationally efficient inference while explicitly quantifying uncertainty in regions with limited observations. The reconstructed depth and uncertainty are used as a drop-in replacement for monocular depth estimators in existing diffusion-based rendering pipelines, without modifying the generative model itself. Experiments on real-world multimodal driving scenes demonstrate that replacing vision-only depth with our sparse range-based reconstruction substantially improves both geometric consistency and visual quality in single-image novel-view video generation. These results highlight the importance of reliable geometric priors for diffusion-based view synthesis and demonstrate the practical benefits of multimodal sensing even at extreme levels of sparsity.
  </details>
