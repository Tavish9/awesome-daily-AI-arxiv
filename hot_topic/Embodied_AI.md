# 🔍 Embodied_AI Papers · 2026-04-29

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[FASTER: Rethinking Real-Time Flow VLAs](https://arxiv.org/abs/2603.19199)**  `arXiv:2603.19199`  `cs.RO` `cs.CV`  
  _Yuxiang Lu, Zhe Liu, Xianzhe Fan, Zhenya Yang, Jinghua Hou, Junyi Li, et al._
  <details open><summary>Abstract</summary>
  Real-time execution is crucial for deploying Vision-Language-Action (VLA) models in the physical world. Existing asynchronous inference methods primarily optimize trajectory smoothness, but neglect the critical latency in reacting to environmental changes. By rethinking the notion of reaction in action chunking policies, this paper presents a systematic analysis of the factors governing reaction time. We show that reaction time follows a uniform distribution determined jointly by the Time to First Action (TTFA) and the execution horizon. Moreover, we reveal that the standard practice of applying a constant schedule in flow-based VLAs can be inefficient and forces the system to complete all sampling steps before any movement can start, forming the bottleneck in reaction latency. To overcome this issue, we propose Fast Action Sampling for ImmediaTE Reaction (FASTER). By introducing a Horizon-Aware Schedule, FASTER adaptively prioritizes near-term actions during flow sampling, compressing the denoising of the immediate reaction by tenfold (e.g., in $\pi_{0.5}$ and X-VLA) into a single step, while preserving the quality of long-horizon trajectory. Coupled with a streaming client-server pipeline, FASTER substantially reduces the effective reaction latency on real robots, especially when deployed on consumer-grade GPUs. Real-world experiments, including a highly dynamic table tennis task, prove that FASTER unlocks unprecedented real-time responsiveness for generalist policies, enabling rapid generation of accurate and smooth trajectories.
  </details>

- **[Open-H-Embodiment: A Large-Scale Dataset for Enabling Foundation Models in Medical Robotics](https://arxiv.org/abs/2604.21017)**  `arXiv:2604.21017`  `cs.RO` `cs.AI`  
  _Open-H-Embodiment Consortium, Nigel Nelson, Juo-Tung Chen, Jesse Haworth, Xinhao Chen, Lukas Zbinden, et al._
  <details open><summary>Abstract</summary>
  Autonomous medical robots hold promise to improve patient outcomes, reduce provider workload, democratize access to care, and enable superhuman precision. However, autonomous medical robotics has been limited by a fundamental data problem: existing medical robotic datasets are small, single-embodiment, and rarely shared openly, restricting the development of foundation models that the field needs to advance. We introduce Open-H-Embodiment, the largest open dataset of medical robotic video with synchronized kinematics to date, spanning more than 49 institutions and multiple robotic platforms including the CMR Versius, Intuitive Surgical's da Vinci, da Vinci Research Kit (dVRK), Rob Surgical BiTrack, Virtual Incision's MIRA, Moon Surgical Maestro, and a variety of custom systems, spanning surgical manipulation, robotic ultrasound, and endoscopy procedures. We demonstrate the research enabled by this dataset through two foundation models. GR00T-H is the first open foundation vision-language-action model for medical robotics, which is the only evaluated model to achieve full end-to-end task completion on a structured suturing benchmark (25% of trials vs. 0% for all others) and achieves 64% average success across a 29-step ex vivo suturing sequence. We also train Cosmos-H-Surgical-Simulator, the first action-conditioned world model to enable multi-embodiment surgical simulation from a single checkpoint, spanning nine robotic platforms and supporting in silico policy evaluation and synthetic data generation for the medical domain. These results suggest that open, large-scale medical robot data collection can serve as critical infrastructure for the research community, enabling advances in robot learning, world modeling, and beyond.
  </details>

- **[STARRY: Spatial-Temporal Action-Centric World Modeling for Robotic Manipulation](https://arxiv.org/abs/2604.26848)**  `arXiv:2604.26848`  `cs.RO`  
  _Yuxuan Tian, Yurun Jin, Bin Yu, Yukun Shi, Hao Wu, Chi Harold Liu, et al._
  <details open><summary>Abstract</summary>
  Robotic manipulation critically requires reasoning about future spatial-temporal interactions, yet existing VLA policies and world-model-enhanced policies do not fully model action-relevant spatial-temporal interaction structure. We propose STARRY, a world-model-enhanced action-generation policy that aligns spatial-temporal prediction with action generation. STARRY jointly denoises future spatial-temporal latents and action sequences, and introduces Geometry-Aware Selective Attention Modulation to convert predicted depth and end-effector geometry into token-aligned weights for selective action-attention modulation. On RoboTwin 2.0, STARRY achieves 93.82% / 93.30% average success under Clean and Randomized settings. Real-world experiments further improve average success from 42.5% to 70.8% over $\pi_{0.5}$, demonstrating the effectiveness of action-centric spatial-temporal world modeling for spatial-temporally demanding robotic action generation.
  </details>

- **[Walk With Me: Long-Horizon Social Navigation for Human-Centric Outdoor Assistance](https://arxiv.org/abs/2604.26839)**  `arXiv:2604.26839`  `cs.RO`  
  _Lingfeng Zhang, Xiaoshuai Hao, Xizhou Bu, Yingbo Tang, Hongsheng Li, Jinghui Lu, et al._
  <details open><summary>Abstract</summary>
  Assisting humans in open-world outdoor environments requires robots to translate high-level natural-language intentions into safe, long-horizon, and socially compliant navigation behavior. Existing map-based methods rely on costly pre-built HD maps, while learning-based policies are mostly limited to indoor and short-horizon settings. To bridge this gap, we propose Walk with Me, a map-free framework for long-horizon social navigation from high-level human instructions. Walk with Me leverages GPS context and lightweight candidate points-of-interest from a public map API for semantic destination grounding and waypoint proposal. A High-Level Vision-Language Model grounds abstract instructions into concrete destinations and plans coarse waypoint sequences. During execution, an observation-aware routing mechanism determines whether the Low-Level Vision-Language-Action policy can handle the current situation or whether explicit safety reasoning from the High-Level VLM is needed. Routine segments are executed by the Low-Level VLA, while complex situations such as crowded crossings trigger high-level reasoning and stop-and-wait behavior when unsafe. By combining semantic intent grounding, map-free long-horizon planning, safety-aware reasoning, and low-level action generation, Walk with Me enables practical outdoor social navigation for human-centric assistance.
  </details>
