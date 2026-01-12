# 🔍 Embodied_AI Papers · 2026-01-11

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[GR-Dexter Technical Report](https://arxiv.org/abs/2512.24210)**  `arXiv:2512.24210`  `cs.RO`  
  _Ruoshi Wen, Guangzeng Chen, Zhongren Cui, Min Du, Yang Gou, Zhigang Han, et al._
  <details open><summary>Abstract</summary>
  Vision-language-action (VLA) models have enabled language-conditioned, long-horizon robot manipulation, but most existing systems are limited to grippers. Scaling VLA policies to bimanual robots with high degree-of-freedom (DoF) dexterous hands remains challenging due to the expanded action space, frequent hand-object occlusions, and the cost of collecting real-robot data. We present GR-Dexter, a holistic hardware-model-data framework for VLA-based generalist manipulation on a bimanual dexterous-hand robot. Our approach combines the design of a compact 21-DoF robotic hand, an intuitive bimanual teleoperation system for real-robot data collection, and a training recipe that leverages teleoperated robot trajectories together with large-scale vision-language and carefully curated cross-embodiment datasets. Across real-world evaluations spanning long-horizon everyday manipulation and generalizable pick-and-place, GR-Dexter achieves strong in-domain performance and improved robustness to unseen objects and unseen instructions. We hope GR-Dexter serves as a practical step toward generalist dexterous-hand robotic manipulation.
  </details>

- **[CombatVLA: An Efficient Vision-Language-Action Model for Combat Tasks in 3D Action Role-Playing Games](https://arxiv.org/abs/2503.09527)**  `arXiv:2503.09527`  `cs.CV` `cs.AI`  
  _Peng Chen, Pi Bu, Yingyao Wang, Xinyi Wang, Ziming Wang, Jie Guo, et al._
  <details open><summary>Abstract</summary>
  Recent advances in Vision-Language-Action models (VLAs) have expanded the capabilities of embodied intelligence. However, significant challenges remain in real-time decision-making in complex 3D environments, which demand second-level responses, high-resolution perception, and tactical reasoning under dynamic conditions. To advance the field, we introduce CombatVLA, an efficient VLA model optimized for combat tasks in 3D action role-playing games(ARPGs). Specifically, our CombatVLA is a 3B model trained on video-action pairs collected by an action tracker, where the data is formatted as action-of-thought (AoT) sequences. Thereafter, CombatVLA seamlessly integrates into an action execution framework, allowing efficient inference through our truncated AoT strategy. Experimental results demonstrate that CombatVLA not only outperforms all existing models on the combat understanding benchmark but also achieves a 50-fold acceleration in game combat. Moreover, it has a higher task success rate than human players. We will open-source all resources, including the action tracker, dataset, benchmark, model weights, training code, and the implementation of the framework atthis https URL.
  </details>

- **[LatentVLA: Efficient Vision-Language Models for Autonomous Driving via Latent Action Prediction](https://arxiv.org/abs/2601.05611)**  `arXiv:2601.05611`  `cs.CV`  
  _Chengen Xie, Bin Sun, Tianyu Li, Junjie Wu, Zhihui Hao, XianPeng Lang, et al._
  <details open><summary>Abstract</summary>
  End-to-end autonomous driving models trained on largescale datasets perform well in common scenarios but struggle with rare, long-tail situations due to limited scenario diversity. Recent Vision-Language-Action (VLA) models leverage broad knowledge from pre-trained visionlanguage models to address this limitation, yet face critical challenges: (1) numerical imprecision in trajectory prediction due to discrete tokenization, (2) heavy reliance on language annotations that introduce linguistic bias and annotation burden, and (3) computational inefficiency from multi-step chain-of-thought reasoning hinders real-time deployment. We propose LatentVLA, a novel framework that employs self-supervised latent action prediction to train VLA models without language annotations, eliminating linguistic bias while learning rich driving representations from unlabeled trajectory data. Through knowledge distillation, LatentVLA transfers the generalization capabilities of VLA models to efficient vision-based networks, achieving both robust performance and real-time efficiency. LatentVLA establishes a new state-of-the-art on the NAVSIM benchmark with a PDMS score of 92.4 and demonstrates strong zeroshot generalization on the nuScenes benchmark.
  </details>

- **[Multimodal Interpretation of Remote Sensing Images: Dynamic Resolution Input Strategy and Multi-scale Vision-Language Alignment Mechanism](https://arxiv.org/abs/2512.23243)**  `arXiv:2512.23243`  `cs.CV`  
  _Siyu Zhang, Lianlei Shan, Runhe Qiu_
  <details open><summary>Abstract</summary>
  Multimodal fusion of remote sensing images serves as a core technology for overcoming the limitations of single-source data and improving the accuracy of surface information extraction, which exhibits significant application value in fields such as environmental monitoring and urban planning. To address the deficiencies of existing methods, including the failure of fixed resolutions to balance efficiency and detail, as well as the lack of semantic hierarchy in single-scale alignment, this study proposes a Vision-language Model (VLM) framework integrated with two key innovations: the Dynamic Resolution Input Strategy (DRIS) and the Multi-scale Vision-language Alignment Mechanism (MS-VLAM).Specifically, the DRIS adopts a coarse-to-fine approach to adaptively allocate computational resources according to the complexity of image content, thereby preserving key fine-grained features while reducing redundant computational overhead. The MS-VLAM constructs a three-tier alignment mechanism covering object, local-region and global levels, which systematically captures cross-modal semantic consistency and alleviates issues of semantic misalignment and granularitythis http URLresults on the RS-GPT4V dataset demonstrate that the proposed framework significantly improves the accuracy of semantic understanding and computational efficiency in tasks including image captioning and cross-modal retrieval. Compared with conventional methods, it achieves superior performance in evaluation metrics such as BLEU-4 and CIDEr for image captioning, as well as R@10 for cross-modal retrieval. This technical framework provides a novel approach for constructing efficient and robust multimodal remote sensing systems, laying a theoretical foundation and offering technical guidance for the engineering application of intelligent remote sensing interpretation.
  </details>
