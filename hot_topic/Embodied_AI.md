# 🔍 Embodied_AI Papers · 2026-01-25

[![Total Papers](https://img.shields.io/badge/Papers-2-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[ReViP: Reducing False Completion in Vision-Language-Action Models with Vision-Proprioception Rebalance](https://arxiv.org/abs/2601.16667)**  `arXiv:2601.16667`  `cs.RO` `cs.CV`  
  _Zhuohao Li, Yinghao Li, Jian-Jian Jiang, Lang Zhou, Tianyu Zhang, Wei-Shi Zheng_
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models have advanced robotic manipulation by combining vision, language, and proprioception to predict actions. However, previous methods fuse proprioceptive signals directly with VLM-encoded vision-language features, resulting in state-dominant bias and false completions despite visible execution failures. We attribute this to modality imbalance, where policies over-rely on internal state while underusing visual evidence. To address this, we present ReViP, a novel VLA framework with Vision-Proprioception Rebalance to enhance visual grounding and robustness under perturbations. The key insight is to introduce auxiliary task-aware environment priors to adaptively modulate the coupling between semantic perception and proprioceptive dynamics. Specifically, we use an external VLM as a task-stage observer to extract real-time task-centric visual cues from visual observations, which drive a Vision-Proprioception Feature-wise Linear Modulation to enhance environmental awareness and reduce state-driven errors. Moreover, to evaluate false completion, we propose the first False-Completion Benchmark Suite built on LIBERO with controlled settings such as Object-Drop. Extensive experiments show that ReViP effectively reduces false-completion rates and improves success rates over strong VLA baselines on our suite, with gains extending to LIBERO, RoboTwin 2.0, and real-world evaluations.
  </details>

- **[FantasyVLN: Unified Multimodal Chain-of-Thought Reasoning for Vision-Language Navigation](https://arxiv.org/abs/2601.13976)**  `arXiv:2601.13976`  `cs.CV` `cs.RO`  
  _Jing Zuo, Lingzhou Mu, Fan Jiang, Chengcheng Ma, Mu Xu, Yonggang Qi_
  <details open><summary>Abstract</summary>
  Achieving human-level performance in Vision-and-Language Navigation (VLN) requires an embodied agent to jointly understand multimodal instructions and visual-spatial context while reasoning over long action sequences. Recent works, such as NavCoT and NavGPT-2, demonstrate the potential of Chain-of-Thought (CoT) reasoning for improving interpretability and long-horizon planning. Moreover, multimodal extensions like OctoNav-R1 and CoT-VLA further validate CoT as a promising pathway toward human-like navigation reasoning. However, existing approaches face critical drawbacks: purely textual CoTs lack spatial grounding and easily overfit to sparse annotated reasoning steps, while multimodal CoTs incur severe token inflation by generating imagined visual observations, making real-time navigation impractical. In this work, we propose FantasyVLN, a unified implicit reasoning framework that preserves the benefits of CoT reasoning without explicit token overhead. Specifically, imagined visual tokens are encoded into a compact latent space using a pretrained Visual AutoRegressor (VAR) during CoT reasoning training, and the model jointly learns from textual, visual, and multimodal CoT modes under a unified multi-CoT strategy. At inference, our model performs direct instruction-to-action mapping while still enjoying reasoning-aware representations. Extensive experiments on LH-VLN show that our approach achieves reasoning-aware yet real-time navigation, improving success rates and efficiency while reducing inference latency by an order of magnitude compared to explicit CoT methods.
  </details>
