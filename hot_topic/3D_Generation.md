# 🔍 3D_Generation Papers · 2026-06-24

[![Total Papers](https://img.shields.io/badge/Papers-1-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Information-Theoretic Classifier-Free Guidance with Adaptive Schedule Optimization](https://arxiv.org/abs/2606.24025)**  `arXiv:2606.24025`  `cs.LG`  
  _Haobo Chen, Xiangxiang Xu, Yuheng Bu_
  <details open><summary>Abstract</summary>
  Diffusion models have achieved strong performance in image, text-to-image, and video generation, where conditional generation is often controlled by classifier-free guidance (CFG). CFG improves condition consistency by increasing a guidance weight, but stronger guidance typically reduces diversity and distributional coverage. It remains unclear how this consistency-coverage trade-off should be controlled across the reverse trajectory, since the distribution induced by CFG is not simply the fixed-time tilted distribution given by the guided score field. To address this issue, we propose an information-theoretic framework for CFG schedule optimization. Our approach uses a clean endpoint reference to specify the desired consistency-coverage trade-off, while optimizing the actual distribution induced by the guided sampler toward this reference. We derive trajectory-level formulas to estimate the objective from samples and score evaluations, avoiding explicit density estimation. On ImageNet-512 with EDM-XXL and COCO with SD-XL, the learned schedules achieve competitive or improved trade-offs over constant guidance and allocate guidance selectively across noise levels.
  </details>
