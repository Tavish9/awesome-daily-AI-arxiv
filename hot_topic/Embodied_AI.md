# 🔍 Embodied_AI Papers · 2025-12-07

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[Evo-1: Lightweight Vision-Language-Action Model with Preserved Semantic Alignment](https://arxiv.org/abs/2511.04555)**  `arXiv:2511.04555`  `cs.RO` `cs.CV`  
  _Tao Lin, Yilei Zhong, Yuxin Du, Jingjing Zhang, Jiting Liu, Yinxinyu Chen, et al._
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models have emerged as a powerful framework that unifies perception, language, and control, enabling robots to perform diverse tasks through multimodal understanding. However, current VLA models typically contain massive parameters and rely heavily on large-scale robot data pretraining, leading to high computational costs during training, as well as limited deployability for real-time inference. Moreover, most training paradigms often degrade the perceptual representations of the vision-language backbone, resulting in overfitting and poor generalization to downstream tasks. In this work, we present Evo-1, a lightweight VLA model that reduces computation and improves deployment efficiency, while maintaining strong performance without pretraining on robot data. Evo-1 builds on a native multimodal Vision-Language model (VLM), incorporating a novel cross-modulated diffusion transformer along with an optimized integration module, together forming an effective architecture. We further introduce a two-stage training paradigm that progressively aligns action with perception, preserving the representations of the VLM. Notably, with only 0.77 billion parameters, Evo-1 achieves state-of-the-art results on the Meta-World and RoboTwin suite, surpassing the previous best models by 12.4% and 6.9%, respectively, and also attains a competitive result of 94.8% on LIBERO. In real-world evaluations, Evo-1 attains a 78% success rate with high inference frequency and low memory overhead, outperforming all baseline methods. We release code, data, and model weights to facilitate future research on lightweight and efficient VLA models.
  </details>

- **[Real-Time Execution of Action Chunking Flow Policies](https://arxiv.org/abs/2506.07339)**  `arXiv:2506.07339`  `cs.RO` `cs.AI` `cs.LG`  
  _Kevin Black, Manuel Y. Galliker, Sergey Levine_
  <details open><summary>Abstract</summary>
  Modern AI systems, especially those interacting with the physical world, increasingly require real-time performance. However, the high latency of state-of-the-art generalist models, including recent vision-language action models (VLAs), poses a significant challenge. While action chunking has enabled temporal consistency in high-frequency control tasks, it does not fully address the latency problem, leading to pauses or out-of-distribution jerky movements at chunk boundaries. This paper presents a novel inference-time algorithm that enables smooth asynchronous execution of action chunking policies. Our method, real-time chunking (RTC), is applicable to any diffusion- or flow-based VLA out of the box with no re-training. It generates the next action chunk while executing the current one, "freezing" actions guaranteed to execute and "inpainting" the rest. To test RTC, we introduce a new benchmark of 12 highly dynamic tasks in the Kinetix simulator, as well as evaluate 6 challenging real-world bimanual manipulation tasks. Results demonstrate that RTC is fast, performant, and uniquely robust to inference delay, significantly improving task throughput and enabling high success rates in precise tasks $\unicode{x2013}$ such as lighting a match $\unicode{x2013}$ even in the presence of significant latency. Seethis https URLfor videos.
  </details>

- **[Training-Time Action Conditioning for Efficient Real-Time Chunking](https://arxiv.org/abs/2512.05964)**  `arXiv:2512.05964`  `cs.RO` `cs.AI`  
  _Kevin Black, Allen Z. Ren, Michael Equi, Sergey Levine_
  <details open><summary>Abstract</summary>
  Real-time chunking (RTC) enables vision-language-action models (VLAs) to generate smooth, reactive robot trajectories by asynchronously predicting action chunks and conditioning on previously committed actions via inference-time inpainting. However, this inpainting method introduces computational overhead that increases inference latency. In this work, we propose a simple alternative: simulating inference delay at training time and conditioning on action prefixes directly, eliminating any inference-time overhead. Our method requires no modifications to the model architecture or robot runtime, and can be implemented with only a few additional lines of code. In simulated experiments, we find that training-time RTC outperforms inference-time RTC at higher inference delays. In real-world experiments on box building and espresso making tasks with the $\pi_{0.6}$ VLA, we demonstrate that training-time RTC maintains both task performance and speed parity with inference-time RTC while being computationally cheaper. Our results suggest that training-time action conditioning is a practical drop-in replacement for inference-time inpainting in real-time robot control.
  </details>

- **[HiMoE-VLA: Hierarchical Mixture-of-Experts for Generalist Vision-Language-Action Policies](https://arxiv.org/abs/2512.05693)**  `arXiv:2512.05693`  `cs.RO` `cs.AI`  
  _Zhiying Du, Bei Liu, Yaobo Liang, Yichao Shen, Haidong Cao, Xiangyu Zheng, et al._
  <details open><summary>Abstract</summary>
  The development of foundation models for embodied intelligence critically depends on access to large-scale, high-quality robot demonstration data. Recent approaches have sought to address this challenge by training on large collections of heterogeneous robotic datasets. However, unlike vision or language data, robotic demonstrations exhibit substantial heterogeneity across embodiments and action spaces as well as other prominent variations such as senor configurations and action control frequencies. The lack of explicit designs for handling such heterogeneity causes existing methods to struggle with integrating diverse factors, thereby limiting their generalization and leading to degraded performance when transferred to new settings. In this paper, we present HiMoE-VLA, a novel vision-language-action (VLA) framework tailored to effectively handle diverse robotic data with heterogeneity. Specifically, we introduce a Hierarchical Mixture-of-Experts (HiMoE) architecture for the action module which adaptively handles multiple sources of heterogeneity across layers and gradually abstracts them into shared knowledge representations. Through extensive experimentation with simulation benchmarks and real-world robotic platforms, HiMoE-VLA demonstrates a consistent performance boost over existing VLA baselines, achieving higher accuracy and robust generalization across diverse robots and action spaces. The code and models are publicly available atthis https URL.
  </details>
