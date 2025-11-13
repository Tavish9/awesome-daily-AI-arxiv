# 🔍 3D_Generation Papers · 2025-11-12

[![Total Papers](https://img.shields.io/badge/Papers-2-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Human-Corrected Labels Learning: Enhancing Labels Quality via Human Correction of VLMs Discrepancies](https://arxiv.org/abs/2511.09063)**  `arXiv:2511.09063`  `cs.LG`  
  _Zhongnian Li, Lan Chen, Yixin Xu, Shi Xu, Xinzheng Xu_
  <details open><summary>Abstract</summary>
  Vision-Language Models (VLMs), with their powerful content generation capabilities, have been successfully applied to data annotation processes. However, the VLM-generated labels exhibit dual limitations: low quality (i.e., label noise) and absence of error correction mechanisms. To enhance label quality, we propose Human-Corrected Labels (HCLs), a novel setting that efficient human correction for VLM-generated noisy labels. As shown in Figure 1(b), HCL strategically deploys human correction only for instances with VLM discrepancies, achieving both higher-quality annotations and reduced labor costs. Specifically, we theoretically derive a risk-consistent estimator that incorporates both human-corrected labels and VLM predictions to train classifiers. Besides, we further propose a conditional probability method to estimate the label distribution using a combination of VLM outputs and model predictions. Extensive experiments demonstrate that our approach achieves superior classification performance and is robust to label noise, validating the effectiveness of HCL in practical weak supervision scenarios. Codethis https URL
  </details>

- **[PAN: A World Model for General, Interactable, and Long-Horizon World Simulation](https://arxiv.org/abs/2511.09057)**  `arXiv:2511.09057`  `cs.CV` `cs.AI` `cs.CL` `cs.LG`  
  _PAN Team Institute of Foundation Models, Jiannan Xiang, Yi Gu, Zihan Liu, Zeyu Feng, Qiyue Gao, et al._
  <details open><summary>Abstract</summary>
  A world model enables an intelligent agent to imagine, predict, and reason about how the world evolves in response to its actions, and accordingly to plan and strategize. While recent video generation models produce realistic visual sequences, they typically operate in the prompt-to-full-video manner without causal control, interactivity, or long-horizon consistency required for purposeful reasoning. Existing world modeling efforts, on the other hand, often focus on restricted domains (e.g., physical, game, or 3D-scene dynamics) with limited depth and controllability, and struggle to generalize across diverse environments and interaction formats. In this work, we introduce PAN, a general, interactable, and long-horizon world model that predicts future world states through high-quality video simulation conditioned on history and natural language actions. PAN employs the Generative Latent Prediction (GLP) architecture that combines an autoregressive latent dynamics backbone based on a large language model (LLM), which grounds simulation in extensive text-based knowledge and enables conditioning on language-specified actions, with a video diffusion decoder that reconstructs perceptually detailed and temporally coherent visual observations, to achieve a unification between latent space reasoning (imagination) and realizable world dynamics (reality). Trained on large-scale video-action pairs spanning diverse domains, PAN supports open-domain, action-conditioned simulation with coherent, long-term dynamics. Extensive experiments show that PAN achieves strong performance in action-conditioned world simulation, long-horizon forecasting, and simulative reasoning compared to other video generators and world models, taking a step towards general world models that enable predictive simulation of future world states for reasoning and acting.
  </details>
