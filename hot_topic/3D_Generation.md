# 🔍 3D_Generation Papers · 2026-09-20

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[OmniVBench: A Benchmark and Large-Scale Dataset for Omni Reference-to-Video Generation](https://arxiv.org/abs/2609.22069)**  `arXiv:2609.22069`  `cs.CV`  
  _Wenxue Li, Peiyan Guan, Haoyang Jiang, Junxian Cai, Hualuo Liu, Chunjie Zhang, et al._
  <details open><summary>Abstract</summary>
  Reference-to-video (R2V) generation is evolving toward increasingly general and versatile reference control, giving rise to the emerging paradigm of omni R2V generation. However, existing benchmarks fall short of these emerging capabilities: their test cases cover limited reference types and compositions, and their evaluation protocols largely assess holistic reference consistency, overlooking whether reference factors are properly preserved, disentangled, and routed. Meanwhile, the high cost of constructing omni R2V training data makes suitable training resources scarce. To address these gaps, we introduce OmniVBench and the Omni-R2V Dataset for evaluating and training omni R2V models. OmniVBench expands R2V evaluation across broader reference types, fine-grained control tasks, and richer reference compositions, covering 7 task families and 18 fine-grained tasks spanning content, motion, style, structure, narrative, and multi-reference settings. We introduce factor-grounded evaluation with 12,172 case-specific checklist items, assessing whether intended reference factors are faithfully preserved, correctly disentangled and bound to their targets, and properly realized according to the instruction. We further introduce the Omni-R2V Dataset, bringing industrial-grade training resources for diverse R2V tasks to the broader research community. Drawing primarily on a large-scale corpus of professional video footage, it comprises 340K processed training samples spanning diverse reference types and multi-reference compositions. We develop task-specific pipelines for reference-target pair construction, offering a practical and scalable recipe for omni R2V data construction. Extensive evaluation of advanced open- and closed-source R2V models reveals clear performance gaps across task families and evaluation dimensions on OmniVBench, highlighting remaining limitations of current R2V models.
  </details>

- **[CompAdapt: Adaptable Composite Motion Modeling for Physics-Consistent Text-to-Video Generation](https://arxiv.org/abs/2609.21455)**  `arXiv:2609.21455`  `cs.CV`  
  _Haoran Qin, Renlong Wu, Tianyu Huang, Yukang Ding, Hui Li, Wangmeng Zuo_
  <details open><summary>Abstract</summary>
  While diffusion-based text-to-video (T2V) models have demonstrated impressive capability in generating realistic and temporally coherent videos, they often fail to respect fundamental physical dynamics. Although recent physics-constrained methods incorporate explicit dynamics priors to improve physical plausibility, they remain limited to simple single-type motions, depend on manually specified parameters, and struggle to generalize to unseen physical laws. In this work, we propose CompAdapt, a physics-consistent T2V framework for adaptable generation across complex real-world scenarios. It extends neural dynamics modeling beyond single-type motions to encompass composite physical behaviors, including coupled motions, multi-stage transitions, and multi-object collisions. Furthermore, CompAdapt translates natural language prompts into structured physical semantics, enabling end-to-end specification of motion types, temporal relations, and initial physical parameters. To generalize to novel physical environments, CompAdapt introduces dynamics-aware prior matching, achieving one-shot adaptation without retraining the core dynamics module. In addition, a physics-aware latent feature fusion module improves visual fidelity under fast and complex motion. Experiments on physics-focused T2V benchmarks demonstrate that CompAdapt improves physical consistency over both general T2V models and physics-constrained baselines, while preserving high visual quality and adaptability to unseen dynamics. The project page is available atthis https URL.
  </details>

- **[JEPA Guided Diffusion: Predictive Vision-Language Conditioning for Generative Traffic Forecasting](https://arxiv.org/abs/2609.21379)**  `arXiv:2609.21379`  `cs.CV`  
  _Trinh Tra Giang Nguyen, Thanh Nguyen Vo, Nguyen Hoai Thuong Bui, Ha Duc Bui_
  <details open><summary>Abstract</summary>
  Accurate traffic forecasting requires both understanding scene dynamics and synthesizing realistic future observations. Recent diffusion-based video generation models produce visually plausible predictions but require expensive end-to-end training and often entangle scene understanding with image synthesis. In this work, we propose a decoupled forecasting framework that separates future representation learning from video generation. A frozen V-JEPA encoder first extracts predictive latent representations from the observed traffic videos, capturing the underlying scene dynamics in a semantic latent space. A lightweight latent alignment module then projects these representations into the conditioning space of a frozen Cosmos diffusion module, enabling future video synthesis without retraining the large generative model. By freezing all foundation models and training only the lightweight alignment module, the proposed framework substantially reduces optimization complexity while preserving forecasting capability. Experimental results on the AI City Challenge 2026 Track 5 benchmark demonstrate that the proposed method achieved a score of 75.1297, ranking third in the competition. These results suggest that predictive world representations learned by V-JEPA can effectively guide downstream video generation, providing a practical and efficient alternative to end-to-end diffusion-based forecasting.
  </details>
