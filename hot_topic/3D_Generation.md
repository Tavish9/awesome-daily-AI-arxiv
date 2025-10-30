# 🔍 3D_Generation Papers · 2025-10-29

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[LaM-SLidE: Latent Space Modeling of Spatial Dynamical Systems via Linked Entities](https://arxiv.org/abs/2502.12128)**  `arXiv:2502.12128`  `cs.LG` `cs.AI`  
  _Florian Sestak, Artur Toshev, Andreas Fürst, Günter Klambauer, Andreas Mayr, Johannes Brandstetter_
  <details open><summary>Abstract</summary>
  Generative models are spearheading recent progress in deep learning, showcasing strong promise for trajectory sampling in dynamical systems as well. However, whereas latent space modeling paradigms have transformed image and video generation, similar approaches are more difficult for most dynamical systems. Such systems -- from chemical molecule structures to collective human behavior -- are described by interactions of entities, making them inherently linked to connectivity patterns, entity conservation, and the traceability of entities over time. Our approach, LaM-SLidE (Latent Space Modeling of Spatial Dynamical Systems via Linked Entities), bridges the gap between: (1) keeping the traceability of individual entities in a latent system representation, and (2) leveraging the efficiency and scalability of recent advances in image and video generation, where pre-trained encoder and decoder enable generative modeling directly in latent space. The core idea of LaM-SLidE is the introduction of identifier representations (IDs) that enable the retrieval of entity properties and entity composition from latent system representations, thus fostering traceability. Experimentally, across different domains, we show that LaM-SLidE performs favorably in terms of speed, accuracy, and generalizability. Code is available atthis https URL.
  </details>

- **[VFXMaster: Unlocking Dynamic Visual Effect Generation via In-Context Learning](https://arxiv.org/abs/2510.25772)**  `arXiv:2510.25772`  `cs.CV`  
  _Baolu Li, Yiming Zhang, Qinghe Wang, Liqian Ma, Xiaoyu Shi, Xintao Wang, et al._
  <details open><summary>Abstract</summary>
  Visual effects (VFX) are crucial to the expressive power of digital media, yet their creation remains a major challenge for generative AI. Prevailing methods often rely on the one-LoRA-per-effect paradigm, which is resource-intensive and fundamentally incapable of generalizing to unseen effects, thus limiting scalability and creation. To address this challenge, we introduce VFXMaster, the first unified, reference-based framework for VFX video generation. It recasts effect generation as an in-context learning task, enabling it to reproduce diverse dynamic effects from a reference video onto target content. In addition, it demonstrates remarkable generalization to unseen effect categories. Specifically, we design an in-context conditioning strategy that prompts the model with a reference example. An in-context attention mask is designed to precisely decouple and inject the essential effect attributes, allowing a single unified model to master the effect imitation without information leakage. In addition, we propose an efficient one-shot effect adaptation mechanism to boost generalization capability on tough unseen effects from a single user-provided video rapidly. Extensive experiments demonstrate that our method effectively imitates various categories of effect information and exhibits outstanding generalization to out-of-domain effects. To foster future research, we will release our code, models, and a comprehensive dataset to the community.
  </details>

- **[When Models Outthink Their Safety: Mitigating Self-Jailbreak in Large Reasoning Models with Chain-of-Guardrails](https://arxiv.org/abs/2510.21285)**  `arXiv:2510.21285`  `cs.AI` `cs.CL`  
  _Yingzhi Mao, Chunkang Zhang, Junxiang Wang, Xinyan Guan, Boxi Cao, Yaojie Lu, et al._
  <details open><summary>Abstract</summary>
  Large Reasoning Models (LRMs) demonstrate remarkable capabilities on complex reasoning tasks but remain vulnerable to severe safety risks, including harmful content generation and jailbreak attacks. Existing mitigation strategies rely on injecting heuristic safety signals during training, which often suppress reasoning ability and fail to resolve the safety-reasoning trade-off. To systematically investigate this issue, we analyze the reasoning trajectories of diverse LRMs and uncover a phenomenon we term Self-Jailbreak, where models override their own risk assessments and justify responding to unsafe prompts. This finding reveals that LRMs inherently possess the ability to reject unsafe queries, but this ability is compromised, resulting in harmful outputs. Building on these insights, we propose the Chain-of-Guardrail (CoG), a training framework that recomposes or backtracks unsafe reasoning steps, steering the model back onto safe trajectories while preserving valid reasoning chains. Extensive experiments across multiple reasoning and safety benchmarks demonstrate that CoG substantially improves the safety of current LRMs while preserving comparable reasoning ability, significantly outperforming prior methods that suffer from severe safety-reasoning trade-offs.
  </details>
