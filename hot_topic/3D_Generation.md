# 🔍 3D_Generation Papers · 2026-01-13

[![Total Papers](https://img.shields.io/badge/Papers-2-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[FilmSceneDesigner: Chaining Set Design for Procedural Film Scene Generation](https://arxiv.org/abs/2511.19137)**  `arXiv:2511.19137`  `cs.CV`  
  _Zhifeng Xie, Keyi Zhang, Yiye Yan, Yuling Guo, Fan Yang, Jiting Zhou, et al._
  <details open><summary>Abstract</summary>
  Film set design plays a pivotal role in cinematic storytelling and shaping the visual atmosphere. However, the traditional process depends on expert-driven manual modeling, which is labor-intensive and time-consuming. To address this issue, we introduce FilmSceneDesigner, an automated scene generation system that emulates professional film set design workflow. Given a natural language description, including scene type, historical period, and style, we design an agent-based chaining framework to generate structured parameters aligned with film set design workflow, guided by prompt strategies that ensure parameter accuracy and coherence. On the other hand, we propose a procedural generation pipeline which executes a series of dedicated functions with the structured parameters for floorplan and structure generation, material assignment, door and window placement, and object retrieval and layout, ultimately constructing a complete film scene from scratch. Moreover, to enhance cinematic realism and asset diversity, we construct SetDepot-Pro, a curated dataset of 6,862 film-specific 3D assets and 733 materials. Experimental results and human evaluations demonstrate that our system produces structurally sound scenes with strong cinematic fidelity, supporting downstream tasks such as virtual previs, construction drawing and mood board creation.
  </details>

- **[Simulating the Visual World with Artificial Intelligence: A Roadmap](https://arxiv.org/abs/2511.08585)**  `arXiv:2511.08585`  `cs.AI` `cs.CV`  
  _Jingtong Yue, Ziqi Huang, Zhaoxi Chen, Xintao Wang, Pengfei Wan, Ziwei Liu_
  <details open><summary>Abstract</summary>
  The landscape of video generation is shifting, from a focus on generating visually appealing clips to building virtual environments that support interaction and maintain physical plausibility. These developments point toward the emergence of video foundation models that function not only as visual generators but also as implicit world models, models that simulate the physical dynamics, agent-environment interactions, and task planning that govern real or imagined worlds. This survey provides a systematic overview of this evolution, conceptualizing modern video foundation models as the combination of two core components: an implicit world model and a video renderer. The world model encodes structured knowledge about the world, including physical laws, interaction dynamics, and agent behavior. It serves as a latent simulation engine that enables coherent visual reasoning, long-term temporal consistency, and goal-driven planning. The video renderer transforms this latent simulation into realistic visual observations, effectively producing videos as a "window" into the simulated world. We trace the progression of video generation through four generations, in which the core capabilities advance step by step, ultimately culminating in a world model, built upon a video generation model, that embodies intrinsic physical plausibility, real-time multimodal interaction, and planning capabilities spanning multiple spatiotemporal scales. For each generation, we define its core characteristics, highlight representative works, and examine their application domains such as robotics, autonomous driving, and interactive gaming. Finally, we discuss open challenges and design principles for next-generation world models, including the role of agent intelligence in shaping and evaluating these systems. An up-to-date list of related works is maintained at this link.
  </details>
