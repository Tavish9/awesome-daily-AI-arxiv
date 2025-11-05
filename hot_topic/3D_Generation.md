# 🔍 3D_Generation Papers · 2025-11-04

[![Total Papers](https://img.shields.io/badge/Papers-1-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[ID-Composer: Multi-Subject Video Synthesis with Hierarchical Identity Preservation](https://arxiv.org/abs/2511.00511)**  `arXiv:2511.00511`  `cs.CV`  
  _Panwang Pan, Jingjing Zhao, Yuchen Lin, Chenguo Lin, Chenxin Li, Haopeng Li, et al._
  <details open><summary>Abstract</summary>
  Video generative models pretrained on large-scale datasets can produce high-quality videos, but are often conditioned on text or a single image, limiting controllability and applicability. We introduce ID-Composer, a novel framework that addresses this gap by tackling multi-subject video generation from a text prompt and reference images. This task is challenging as it requires preserving subject identities, integrating semantics across subjects and modalities, and maintaining temporal consistency. To faithfully preserve the subject consistency and textual information in synthesized videos, ID-Composer designs a hierarchical identity-preserving attention mechanism, which effectively aggregates features within and across subjects and modalities. To effectively allow for the semantic following of user intention, we introduce semantic understanding via pretrained vision-language model (VLM), leveraging VLM's superior semantic understanding to provide fine-grained guidance and capture complex interactions between multiple subjects. Considering that standard diffusion loss often fails in aligning the critical concepts like subject ID, we employ an online reinforcement learning phase to drive the overall training objective of ID-Composer into RLVR. Extensive experiments demonstrate that our model surpasses existing methods in identity preservation, temporal consistency, and video quality.
  </details>
