# 🔍 Embodied_AI Papers · 2025-11-10

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[TwinVLA: Data-Efficient Bimanual Manipulation with Twin Single-Arm Vision-Language-Action Models](https://arxiv.org/abs/2511.05275)**  `arXiv:2511.05275`  `cs.RO` `cs.LG`  
  _Hokyun Im, Euijin Jeong, Jianlong Fu, Andrey Kolobov, Youngwoon Lee_
  <details open><summary>Abstract</summary>
  Vision-language-action models (VLAs) trained on large-scale robotic datasets have demonstrated strong performance on manipulation tasks, including bimanual tasks. However, because most public datasets focus on single-arm demonstrations, adapting VLAs for bimanual tasks typically requires substantial additional bimanual data and fine-tuning. To address this challenge, we introduce TwinVLA, a modular framework that composes two copies of a pretrained single-arm VLA into a coordinated bimanual VLA. Unlike monolithic cross-embodiment models trained on mixtures of single-arm and bimanual data, TwinVLA improves both data efficiency and performance by composing pretrained single-arm policies. Across diverse bimanual tasks in real-world and simulation settings, TwinVLA outperforms a comparably-sized monolithic RDT-1B model without requiring any bimanual pretraining. Furthermore, it narrows the gap to state-of-the-art model, $\pi_0$ which rely on extensive proprietary bimanual data and compute cost. These results establish our modular composition approach as a data-efficient and scalable path toward high-performance bimanual manipulation, leveraging public single-arm data.
  </details>

- **[EveryDayVLA: A Vision-Language-Action Model for Affordable Robotic Manipulation](https://arxiv.org/abs/2511.05397)**  `arXiv:2511.05397`  `cs.RO` `cs.CV`  
  _Samarth Chopra, Alex McMoil, Ben Carnovale, Evan Sokolson, Rajkumar Kubendran, Samuel Dickerson_
  <details open><summary>Abstract</summary>
  While Vision-Language-Action (VLA) models map visual inputs and language instructions directly to robot actions, they often rely on costly hardware and struggle in novel or cluttered scenes. We introduce EverydayVLA, a 6-DOF manipulator that can be assembled for under $300, capable of modest payloads and workspace. A single unified model jointly outputs discrete and continuous actions, and our adaptive-horizon ensemble monitors motion uncertainty to trigger on-the-fly re-planning for safe, reliable operation. On LIBERO, EverydayVLA matches state-of-the-art success rates, and in real-world tests it outperforms prior methods by 49% in-distribution and 34.9% out-of-distribution. By combining a state-of-the-art VLA with cost-effective hardware, EverydayVLA democratizes access to a robotic foundation model and paves the way for economical use in homes and research labs alike. Experiment videos and details:this https URL
  </details>

- **[GeoAware-VLA: Implicit Geometry Aware Vision-Language-Action Model](https://arxiv.org/abs/2509.14117)**  `arXiv:2509.14117`  `cs.RO`  
  _Ali Abouzeid, Malak Mansour, Zezhou Sun, Dezhen Song_
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models often fail to generalize to novel camera viewpoints, a limitation stemming from their difficulty in inferring robust 3D geometry from 2D images. We introduce GeoAware-VLA, a simple yet effective approach that enhances viewpoint invariance by integrating strong geometric priors into the vision backbone. Instead of training a visual encoder or relying on explicit 3D data, we leverage a frozen, pretrained geometric vision model as a feature extractor. A trainable projection layer then adapts these geometrically-rich features for the policy decoder, relieving it of the burden of learning 3D consistency from scratch. Through extensive evaluations on LIBERO benchmark subsets, we show GeoAware-VLA achieves substantial improvements in zero-shot generalization to novel camera poses, boosting success rates by over 2x in simulation. Crucially, these benefits translate to the physical world; our model shows a significant performance gain on a real robot, especially when evaluated from unseen camera angles. Our approach proves effective across both continuous and discrete action spaces, highlighting that robust geometric grounding is a key component for creating more generalizable robotic agents.
  </details>

- **[Visual Spatial Tuning](https://arxiv.org/abs/2511.05491)**  `arXiv:2511.05491`  `cs.CV`  
  _Rui Yang, Ziyu Zhu, Yanwei Li, Jingjia Huang, Shen Yan, Siyuan Zhou, et al._
  <details open><summary>Abstract</summary>
  Capturing spatial relationships from visual inputs is a cornerstone of human-like general intelligence. Several previous studies have tried to enhance the spatial awareness of Vision-Language Models (VLMs) by adding extra expert encoders, which brings extra overhead and usually harms general capabilities. To enhance the spatial ability in general architectures, we introduce Visual Spatial Tuning (VST), a comprehensive framework to cultivate VLMs with human-like visuospatial abilities, from spatial perception to reasoning. We first attempt to enhance spatial perception in VLMs by constructing a large-scale dataset termed VST-P, which comprises 4.1 million samples spanning 19 skills across single views, multiple images, and videos. Then, we present VST-R, a curated dataset with 135K samples that instruct models to reason in space. In particular, we adopt a progressive training pipeline: supervised fine-tuning to build foundational spatial knowledge, followed by reinforcement learning to further improve spatial reasoning abilities. Without the side-effect to general capabilities, the proposed VST consistently achieves state-of-the-art results on several spatial benchmarks, including $34.8\%$ on MMSI-Bench and $61.2\%$ on VSIBench. It turns out that the Vision-Language-Action models can be significantly enhanced with the proposed spatial tuning paradigm, paving the way for more physically grounded AI.
  </details>
