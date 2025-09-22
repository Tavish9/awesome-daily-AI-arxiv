# 🔍 3D_Generation Papers · 2025-09-21

[![Total Papers](https://img.shields.io/badge/Papers-2-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Lynx: Towards High-Fidelity Personalized Video Generation](https://arxiv.org/abs/2509.15496)**  `arXiv:2509.15496`  `cs.CV`  
  _Shen Sang, Tiancheng Zhi, Tianpei Gu, Jing Liu, Linjie Luo_
  <details open><summary>Abstract</summary>
  We present Lynx, a high-fidelity model for personalized video synthesis from a single input image. Built on an open-source Diffusion Transformer (DiT) foundation model, Lynx introduces two lightweight adapters to ensure identity fidelity. The ID-adapter employs a Perceiver Resampler to convert ArcFace-derived facial embeddings into compact identity tokens for conditioning, while the Ref-adapter integrates dense VAE features from a frozen reference pathway, injecting fine-grained details across all transformer layers through cross-attention. These modules collectively enable robust identity preservation while maintaining temporal coherence and visual realism. Through evaluation on a curated benchmark of 40 subjects and 20 unbiased prompts, which yielded 800 test cases, Lynx has demonstrated superior face resemblance, competitive prompt following, and strong video quality, thereby advancing the state of personalized video generation.
  </details>

- **[OpenViGA: Video Generation for Automotive Driving Scenes by Streamlining and Fine-Tuning Open Source Models with Public Data](https://arxiv.org/abs/2509.15479)**  `arXiv:2509.15479`  `cs.CV`  
  _Björn Möller, Zhengyang Li, Malte Stelzer, Thomas Graave, Fabian Bettels, Muaaz Ataya, et al._
  <details open><summary>Abstract</summary>
  Recent successful video generation systems that predict and create realistic automotive driving scenes from short video inputs assign tokenization, future state prediction (world model), and video decoding to dedicated models. These approaches often utilize large models that require significant training resources, offer limited insight into design choices, and lack publicly available code and datasets. In this work, we address these deficiencies and present OpenViGA, an open video generation system for automotive driving scenes. Our contributions are: Unlike several earlier works for video generation, such as GAIA-1, we provide a deep analysis of the three components of our system by separate quantitative and qualitative evaluation: Image tokenizer, world model, video decoder. Second, we purely build upon powerful pre-trained open source models from various domains, which we fine-tune by publicly available automotive data (BDD100K) on GPU hardware at academic scale. Third, we build a coherent video generation system by streamlining interfaces of our components. Fourth, due to public availability of the underlying models and data, we allow full reproducibility. Finally, we also publish our code and models on Github. For an image size of 256x256 at 4 fps we are able to predict realistic driving scene videos frame-by-frame with only one frame of algorithmic latency.
  </details>
