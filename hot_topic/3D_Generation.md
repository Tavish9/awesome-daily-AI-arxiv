# 🔍 3D_Generation Papers · 2026-11-15

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Ego2Flow: Benchmarking the Traffic-System Impact of Autonomous Driving on Maps Distilled from Real-World Roads](https://arxiv.org/abs/2611.17720)**  `arXiv:2611.17720`  `cs.RO` `cs.CV`  
  _Yu Dong, Weiying Shen, Hangyu Li, Shu Han, Hong Li, Xiangbo Gao, et al._
  <details open><summary>Abstract</summary>
  End-to-end autonomous driving is predominantly evaluated through ego-vehicle safety and task completion. Its deployment in urban traffic, however, creates sustained interactions among vehicles whose collective effects remain insufficiently evaluated. We introduce Ego2Flow, a closed-loop benchmark for assessing the traffic-system impact of autonomous driving on maps distilled from real-world cities. To construct realistic 3D urban environments for sustained closed-loop traffic simulation, we develop an agent-guided map distillation framework that integrates real-world maps and observations with complementary geographic information. Through an iterative feedback mechanism and a traffic information graph that jointly guide scene generation, the framework preserves lane topology, critical road geometry and decision-relevant visual conditions while simplifying nonessential details and completing unobserved regions. Using our proposed framework, we generate and publicly release six CARLA maps from the Argoverse 2 dataset, covering the corresponding real-world regions and enabling paired comparisons of driving behavior under real and simulated observations. On these maps, Ego2Flow evaluates how autonomous driving policies affect traffic efficiency, safety, stability and energy consumption across diverse road structures. Compared with existing construction methods, our framework achieves the lowest average displacement error between planning outputs from paired real and simulated observations. We further benchmark representative driving policies to characterize their system-level impact on urban traffic. Project Page:this https URL.
  </details>

- **[Foundation Model Driven Robotics: A Comprehensive Review](https://arxiv.org/abs/2507.10087)**  `arXiv:2507.10087`  `cs.RO`  
  _Muhammad Tayyab Khan, Ammar Waheed, Seung Ki Moon_
  <details open><summary>Abstract</summary>
  The rapid emergence of foundation models, particularly large language models and vision-language models, has introduced a transformative paradigm in robotics. The models offer powerful capabilities in semantic understanding, high-level reasoning, and cross-modal generalization, enabling significant advances in perception, planning, control, and human-robot interaction. This critical review provides a structured synthesis of recent developments and organizes applications into four directions: simulation-driven robotics, open-world operation, sim-to-real transfer, and adaptable robotic systems. Unlike existing surveys that emphasize isolated capabilities, this work highlights integrated, system-level strategies and evaluates their practical feasibility in real-world environments. Key enabling trends such as procedural scene generation, policy generalization, and multimodal reasoning are discussed alongside core bottlenecks, including limited embodiment, lack of multimodal data, safety risks, and computational constraints. Through this lens, this paper identifies both the architectural strengths and critical limitations of foundation model-based robotics, highlighting open challenges in real-time operation, grounding, resilience, and trust. The review concludes with a roadmap of proposed future research directions for bridging semantic reasoning and physical intelligence through more robust, interpretable, and embodied models.
  </details>

- **[SceneAgent: A Multi-Agent Framework for Portable Game Scene Generation](https://arxiv.org/abs/2611.17821)**  `arXiv:2611.17821`  `cs.CV` `cs.AI`  
  _Xingyi Li, Jiahao Yang, Yiqin Zhu, Jingwen Ye, Yang Sun, Weidong Zhang_
  <details open><summary>Abstract</summary>
  Moving a scene generator to a new game engine requires more than exporting its final output: planning, construction tools, and stored experience may also depend on the original backend. We present SceneAgent, a multi-agent framework for reusing the construction process and its experience across backends. A canonical SceneContext maintains the evolving world, while backend adapters isolate coordinate conventions, asset bindings, and export. Structured handoffs let fresh Builder sessions query this persistent state without inheriting the full construction transcript. Across generations, human-approved traces are distilled into asset-ID-free Layout skills and semantic Content skills that can be retrieved and recombined. We introduce GameSceneBench, comprising 69 indoor and outdoor prompts. Under a common asset and evaluation protocol, SceneAgent obtains human tie-adjusted preference scores of 78.2-89.4% against five baselines. Ablations show that reusable skills and the multi-agent protocol primarily improve prompt alignment and scene completeness, with additional runtime. Deployment in a second engine preserves the shared construction protocol and skill library while replacing backend integration components. Together, these results support separating persistent scene state, task-local reasoning, and reusable experience for portable scene construction.
  </details>

- **[Free-GVC: Toward Retraining-Free Extreme Generative Video Compression with Temporal Coherence](https://arxiv.org/abs/2602.09868)**  `arXiv:2602.09868`  `cs.CV`  
  _Xiaoyue Ling, Chuqin Zhou, Chunyi Li, Yunuo Chen, Yuan Tian, Guo Lu, et al._
  <details open><summary>Abstract</summary>
  Building on recent advances in video generation, generative video compression has emerged as a new paradigm for achieving visually pleasing reconstructions. However, existing methods exhibit limited exploitation of temporal correlations, causing noticeable flicker and degraded temporal coherence at ultra-low bitrates. In this paper, we propose Free-GVC, a retraining-free generative video compression framework that reformulates video coding as latent trajectory compression guided by a video diffusion prior. Our method operates at the group-of-pictures (GOP) level, encoding video segments into a compact latent space and progressively compressing them along the diffusion trajectory. To ensure perceptually consistent reconstruction across GOPs, we introduce an Adaptive Quality Control module that dynamically constructs an online rate-perception surrogate model to predict the optimal diffusion step for each GOP. In addition, an Inter-GOP Alignment module establishes frame overlap and performs latent fusion between adjacent groups, thereby mitigating flicker and enhancing temporal coherence. Experiments show that Free-GVC achieves an average of 93.29% BD-Rate reduction in DISTS over the recent neural codec DCVC-RT, and a user study further confirms its superior perceptual quality and temporal coherence at ultra-low bitrates.
  </details>
