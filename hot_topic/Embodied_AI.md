# 🔍 Embodied_AI Papers · 2026-02-22

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[SimVLA: A Simple VLA Baseline for Robotic Manipulation](https://arxiv.org/abs/2602.18224)**  `arXiv:2602.18224`  `cs.RO` `cs.LG`  
  _Yuankai Luo, Woping Chen, Tong Liang, Baiqiao Wang, Zhenguo Li_
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models have emerged as a promising paradigm for general-purpose robotic manipulation, leveraging large-scale pre-training to achieve strong performance. The field has rapidly evolved with additional spatial priors and diverse architectural innovations. However, these advancements are often accompanied by varying training recipes and implementation details, which can make it challenging to disentangle the precise source of empirical gains. In this work, we introduce SimVLA, a streamlined baseline designed to establish a transparent reference point for VLA research. By strictly decoupling perception from control, using a standard vision-language backbone and a lightweight action head, and standardizing critical training dynamics, we demonstrate that a minimal design can achieve state-of-the-art performance. Despite having only 0.5B parameters, SimVLA outperforms multi-billion-parameter models on standard simulation benchmarks without robot pretraining. SimVLA also reaches on-par real-robot performance compared to pi0.5. Our results establish SimVLA as a robust, reproducible baseline that enables clear attribution of empirical gains to future architectural innovations. Website:this https URL
  </details>

- **[How Fast Can I Run My VLA? Demystifying VLA Inference Performance with VLA-Perf](https://arxiv.org/abs/2602.18397)**  `arXiv:2602.18397`  `cs.RO`  
  _Wenqi Jiang, Jason Clemons, Karu Sankaralingam, Christos Kozyrakis_
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models have recently demonstrated impressive capabilities across various embodied AI tasks. While deploying VLA models on real-world robots imposes strict real-time inference constraints, the inference performance landscape of VLA remains poorly understood due to the large combinatorial space of model architectures and inference systems. In this paper, we ask a fundamental research question: How should we design future VLA models and systems to support real-time inference? To address this question, we first introduce VLA-Perf, an analytical performance model that can analyze inference performance for arbitrary combinations of VLA models and inference systems. Using VLA-Perf, we conduct the first systematic study of the VLA inference performance landscape. From a model-design perspective, we examine how inference performance is affected by model scaling, model architectural choices, long-context video inputs, asynchronous inference, and dual-system model pipelines. From the deployment perspective, we analyze where VLA inference should be executed -- on-device, on edge servers, or in the cloud -- and how hardware capability and network performance jointly determine end-to-end latency. By distilling 15 key takeaways from our comprehensive evaluation, we hope this work can provide practical guidance for the design of future VLA models and inference systems.
  </details>

- **[UAOR: Uncertainty-aware Observation Reinjection for Vision-Language-Action Models](https://arxiv.org/abs/2602.18020)**  `arXiv:2602.18020`  `cs.CV` `cs.RO`  
  _Jiabing Yang, Yixiang Chen, Yuan Xu, Peiyan Li, Xiangnan Wu, Zichen Wen, et al._
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models leverage pretrained Vision-Language Models (VLMs) as backbones to map images and instructions to actions, demonstrating remarkable potential for generalizable robotic manipulation. To enhance performance, existing methods often incorporate extra observation cues (e.g., depth maps, point clouds) or auxiliary modules (e.g., object detectors, encoders) to enable more precise and reliable task execution, yet these typically require costly data collection and additional training. Inspired by the finding that Feed-Forward Network (FFN) in language models can act as "key-value memory", we propose Uncertainty-aware Observation Reinjection (UAOR), an effective, training-free and plug-and-play module for VLA models. Specifically, when the current language model layer exhibits high uncertainty, measured by Action Entropy, it reinjects key observation information into the next layer's Feed-Forward Network (FFN) through attention retrieval. This mechanism helps VLAs better attend to observations during inference, enabling more confident and faithful action generation. Comprehensive experiments show that our method consistently improves diverse VLA models across simulation and real-world tasks with minimal overhead. Notably, UAOR eliminates the need for additional observation cues or modules, making it a versatile and practical plug-in for existing VLA pipelines. The project page is atthis https URL.
  </details>

- **[ROCKET: Residual-Oriented Multi-Layer Alignment for Spatially-Aware Vision-Language-Action Models](https://arxiv.org/abs/2602.17951)**  `arXiv:2602.17951`  `cs.CV` `cs.AI`  
  _Guoheng Sun, Tingting Du, Kaixi Feng, Chenxiang Luo, Xingguo Ding, Zheyu Shen, et al._
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models enable instruction-following robotic manipulation, but they are typically pretrained on 2D data and lack 3D spatial understanding. An effective approach is representation alignment, where a strong vision foundation model is used to guide a 2D VLA model. However, existing methods usually apply supervision at only a single layer, failing to fully exploit the rich information distributed across depth; meanwhile, naïve multi-layer alignment can cause gradient interference. We introduce ROCKET, a residual-oriented multi-layer representation alignment framework that formulates multi-layer alignment as aligning one residual stream to another. Concretely, ROCKET employs a shared projector to align multiple layers of the VLA backbone with multiple layers of a powerful 3D vision foundation model via a layer-invariant mapping, which reduces gradient conflicts. We provide both theoretical justification and empirical analyses showing that a shared projector is sufficient and outperforms prior designs, and further propose a Matryoshka-style sparse activation scheme for the shared projector to balance multiple alignment losses. Our experiments show that, combined with a training-free layer selection strategy, ROCKET requires only about 4% of the compute budget while achieving 98.5% state-of-the-art success rate on LIBERO. We further demonstrate the superior performance of ROCKET across LIBERO-Plus and RoboTwin, as well as multiple VLA models. The code and model weights can be found atthis https URL.
  </details>
