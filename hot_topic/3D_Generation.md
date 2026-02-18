# 🔍 3D_Generation Papers · 2026-02-17

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Consistency-Preserving Diverse Video Generation](https://arxiv.org/abs/2602.15287)**  `arXiv:2602.15287`  `cs.CV`  
  _Xinshuang Liu, Runfa Blark Li, Truong Nguyen_
  <details open><summary>Abstract</summary>
  Text-to-video generation is expensive, so only a few samples are typically produced per prompt. In this low-sample regime, maximizing the value of each batch requires high cross-video diversity. Recent methods improve diversity for image generation, but for videos they often degrade within-video temporal consistency and require costly backpropagation through a video decoder. We propose a joint-sampling framework for flow-matching video generators that improves batch diversity while preserving temporal consistency. Our approach applies diversity-driven updates and then removes only the components that would decrease a temporal-consistency objective. To avoid image-space gradients, we compute both objectives with lightweight latent-space models, avoiding video decoding and decoder backpropagation. Experiments on a state-of-the-art text-to-video flow-matching model show diversity comparable to strong joint-sampling baselines while substantially improving temporal consistency and color naturalness. Code will be released.
  </details>

- **[Train Short, Inference Long: Training-free Horizon Extension for Autoregressive Video Generation](https://arxiv.org/abs/2602.14027)**  `arXiv:2602.14027`  `cs.CV`  
  _Jia Li, Xiaomeng Fu, Xurui Peng, Weifeng Chen, Youwei Zheng, Tianyu Zhao, et al._
  <details open><summary>Abstract</summary>
  Autoregressive video diffusion models have emerged as a scalable paradigm for long video generation. However, they often suffer from severe extrapolation failure, where rapid error accumulation leads to significant temporal degradation when extending beyond training horizons. We identify that this failure primarily stems from the spectral bias of 3D positional embeddings and the lack of dynamic priors in noise sampling. To address these issues, we propose FLEX (Frequency-aware Length EXtension), a training-free inference-time framework that bridges the gap between short-term training and long-term inference. FLEX introduces Frequency-aware RoPE Modulation to adaptively interpolate under-trained low-frequency components while extrapolating high-frequency ones to preserve multi-scale temporal discriminability. This is integrated with Antiphase Noise Sampling (ANS) to inject high-frequency dynamic priors and Inference-only Attention Sink to anchor global structure. Extensive evaluations on VBench demonstrate that FLEX significantly outperforms state-of-the-art models at 6x extrapolation (30s duration) and matches the performance of long-video fine-tuned baselines at 12x scale (60s duration). As a plug-and-play augmentation, FLEX seamlessly integrates into existing inference pipelines for horizon extension. It effectively pushes the generation limits of models such as LongLive, supporting consistent and dynamic video synthesis at a 4-minute scale. Project page is available atthis https URL.
  </details>

- **[Improving LLM Reliability through Hybrid Abstention and Adaptive Detection](https://arxiv.org/abs/2602.15391)**  `arXiv:2602.15391`  `cs.AI`  
  _Ankit Sharma, Nachiket Tapas, Jyotiprakash Patra_
  <details open><summary>Abstract</summary>
  Large Language Models (LLMs) deployed in production environments face a fundamental safety-utility trade-off either a strict filtering mechanisms prevent harmful outputs but often block benign queries or a relaxed controls risk unsafe content generation. Conventional guardrails based on static rules or fixed confidence thresholds are typically context-insensitive and computationally expensive, resulting in high latency and degraded user experience. To address these limitations, we introduce an adaptive abstention system that dynamically adjusts safety thresholds based on real-time contextual signals such as domain and user history. The proposed framework integrates a multi-dimensional detection architecture composed of five parallel detectors, combined through a hierarchical cascade mechanism to optimize both speed and precision. The cascade design reduces unnecessary computation by progressively filtering queries, achieving substantial latency improvements compared to non-cascaded models and external guardrail systems. Extensive evaluation on mixed and domain-specific workloads demonstrates significant reductions in false positives, particularly in sensitive domains such as medical advice and creative writing. The system maintains high safety precision and near-perfect recall under strict operating modes. Overall, our context-aware abstention framework effectively balances safety and utility while preserving performance, offering a scalable solution for reliable LLM deployment.
  </details>
