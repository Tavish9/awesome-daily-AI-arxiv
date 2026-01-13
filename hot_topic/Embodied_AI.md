# 🔍 Embodied_AI Papers · 2026-01-12

[![Total Papers](https://img.shields.io/badge/Papers-7-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[CulinaryCut-VLAP: A Vision-Language-Action-Physics Framework for Food Cutting via a Force-Aware Material Point Method](https://arxiv.org/abs/2601.06451)**  `arXiv:2601.06451`  `cs.RO` `cs.CV`  
  _Hyunseo Koh, Chang-Yong Song, Youngjae Choi, Misa Viveiros, David Hyde, Heewon Kim_
  <details open><summary>Abstract</summary>
  Food cutting is a highly practical yet underexplored application at the intersection of vision and robotic manipulation. The task remains challenging because interactions between the knife and deformable materials are highly nonlinear and often entail large deformations, frequent contact, and topological change, which in turn hinder stable and safe large-scale data collection.To address these challenges, we propose a unified framework that couples a vision-language-action (VLA) dataset with a physically realistic cutting simulator built on the material point method (MPM). Our simulator adopts MLS-MPM as its computational core, reducing numerical dissipation and energy drift while preserving rotational and shear responses even under topology-changing cuts. During cutting, forces and stress distributions are estimated from impulse exchanges between particles and the grid, enabling stable tracking of transient contact forces and energy transfer.We also provide a benchmark dataset that integrates diverse cutting trajectories, multi-view visual observations, and fine-grained language instructions, together with force--torque and tool--pose labels to provide physically consistent training signals.These components realize a learning--evaluation loop that respects the core physics of cutting and establishes a safe, reproducible, and scalable foundation for advancing VLA models in deformable object manipulation.
  </details>

- **[PALM: Progress-Aware Policy Learning via Affordance Reasoning for Long-Horizon Robotic Manipulation](https://arxiv.org/abs/2601.07060)**  `arXiv:2601.07060`  `cs.RO`  
  _Yuanzhe Liu, Jingyuan Zhu, Yuchen Mo, Gen Li, Xu Cao, Jin Jin, et al._
  <details open><summary>Abstract</summary>
  Recent advancements in vision-language-action (VLA) models have shown promise in robotic manipulation, yet they continue to struggle with long-horizon, multi-step tasks. Existing methods lack internal reasoning mechanisms that can identify task-relevant interaction cues or track progress within a subtask, leading to critical execution errors such as repeated actions, missed steps, and premature termination. To address these challenges, we introduce PALM, a VLA framework that structures policy learning around interaction-centric affordance reasoning and subtask progress cues. PALM distills complementary affordance representations that capture object relevance, contact geometry, spatial placements, and motion dynamics, and serve as task-relevant anchors for visuomotor control. To further stabilize long-horizon execution, PALM predicts continuous within-subtask progress, enabling seamless subtask transitions. Across extensive simulation and real-world experiments, PALM consistently outperforms baselines, achieving a 91.8% success rate on LIBERO-LONG, a 12.5% improvement in average length on CALVIN ABC->D, and a 2x improvement over real-world baselines across three long-horizon generalization settings.
  </details>

- **[On-the-Fly VLA Adaptation via Test-Time Reinforcement Learning](https://arxiv.org/abs/2601.06748)**  `arXiv:2601.06748`  `cs.RO`  
  _Changyu Liu, Yiyang Liu, Taowen Wang, Qiao Zhuang, James Chenhao Liang, Wenhao Yang, et al._
  <details open><summary>Abstract</summary>
  Vision-Language-Action models have recently emerged as a powerful paradigm for general-purpose robot learning, enabling agents to map visual observations and natural-language instructions into executable robotic actions. Though popular, they are primarily trained via supervised fine-tuning or training-time reinforcement learning, requiring explicit fine-tuning phases, human interventions, or controlled data collection. Consequently, existing methods remain unsuitable for challenging simulated- or physical-world deployments, where robots must respond autonomously and flexibly to evolving environments. To address this limitation, we introduce a Test-Time Reinforcement Learning for VLAs (TT-VLA), a framework that enables on-the-fly policy adaptation during inference. TT-VLA formulates a dense reward mechanism that leverages step-by-step task-progress signals to refine action policies during test time while preserving the SFT/RL-trained priors, making it an effective supplement to current VLA models. Empirical results show that our approach enhances overall adaptability, stability, and task success in dynamic, previously unseen scenarios under simulated and real-world settings. We believe TT-VLA offers a principled step toward self-improving, deployment-ready VLAs.
  </details>

- **[A Vision-Language-Action Model with Visual Prompt for OFF-Road Autonomous Driving](https://arxiv.org/abs/2601.03519)**  `arXiv:2601.03519`  `cs.RO`  
  _Liangdong Zhang, Yiming Nie, Haoyang Li, Fanjie Kong, Baobao Zhang, Shunxin Huang, et al._
  <details open><summary>Abstract</summary>
  Efficient trajectory planning in off-road terrains presents a formidable challenge for autonomous vehicles, often necessitating complex multi-step pipelines. However, traditional approaches exhibit limited adaptability in dynamic environments. To address these limitations, this paper proposes OFF-EMMA, a novel end-to-end multimodal framework designed to overcome the deficiencies of insufficient spatial perception and unstable reasoning in visual-language-action (VLA) models for off-road autonomous driving scenarios. The framework explicitly annotates input images through the design of a visual prompt block and introduces a chain-of-thought with self-consistency (COT-SC) reasoning strategy to enhance the accuracy and robustness of trajectory planning. The visual prompt block utilizes semantic segmentation masks as visual prompts, enhancing the spatial understanding ability of pre-trained visual-language models for complex terrains. The COT- SC strategy effectively mitigates the error impact of outliers on planning performance through a multi-path reasoning mechanism. Experimental results on the RELLIS-3D off-road dataset demonstrate that OFF-EMMA significantly outperforms existing methods, reducing the average L2 error of the Qwen backbone model by 13.3% and decreasing the failure rate from 16.52% to 6.56%.
  </details>

- **[SparseOccVLA: Bridging Occupancy and Vision-Language Models via Sparse Queries for Unified 4D Scene Understanding and Planning](https://arxiv.org/abs/2601.06474)**  `arXiv:2601.06474`  `cs.CV` `cs.AI`  
  _Chenxu Dang, Jie Wang, Guang Li, Zhiwen Hou, Zihan You, Hangjun Ye, et al._
  <details open><summary>Abstract</summary>
  In autonomous driving, Vision Language Models (VLMs) excel at high-level reasoning , whereas semantic occupancy provides fine-grained details. Despite significant progress in individual fields, there is still no method that can effectively integrate both paradigms. Conventional VLMs struggle with token explosion and limited spatiotemporal reasoning, while semantic occupancy provides a unified, explicit spatial representation but is too dense to integrate efficiently with VLMs. To address these challenges and bridge the gap between VLMs and occupancy, we propose SparseOccVLA, a novel vision-language-action model that unifies scene understanding, occupancy forecasting, and trajectory planning powered by sparse occupancy queries. Starting with a lightweight Sparse Occupancy Encoder, SparseOccVLA generates compact yet highly informative sparse occupancy queries that serve as the single bridge between vision and language. These queries are aligned into the language space and reasoned by the LLM for unified scene understanding and future occupancy forecasting. Furthermore, we introduce an LLM-guided Anchor-Diffusion Planner featuring decoupled anchor scoring and denoising, as well as cross-model trajectory-condition fusion. SparseOccVLA achieves a 7% relative improvement in CIDEr over the state-of-the-art on OmniDrive-nuScenes, a 0.5 increase in mIoU score on Occ3D-nuScenes, and sets state-of-the-art open-loop planning metric on nuScenes benchmark, demonstrating its strong holistic capability.
  </details>

- **[Motion Focus Recognition in Fast-Moving Egocentric Video](https://arxiv.org/abs/2601.07154)**  `arXiv:2601.07154`  `cs.CV`  
  _Daniel Hong, James Tribble, Hao Wang, Chaoyi Zhou, Ashish Bastola, Siyu Huang, et al._
  <details open><summary>Abstract</summary>
  From Vision-Language-Action (VLA) systems to robotics, existing egocentric datasets primarily focus on action recognition tasks, while largely overlooking the inherent role of motion analysis in sports and other fast-movement scenarios. To bridge this gap, we propose a real-time motion focus recognition method that estimates the subject's locomotion intention from any egocentric video. Our approach leverages the foundation model for camera pose estimation and introduces system-level optimizations to enable efficient and scalable inference. Evaluated on a collected egocentric action dataset, our method achieves real-time performance with manageable memory consumption through a sliding batch inference strategy. This work makes motion-centric analysis practical for edge deployment and offers a complementary perspective to existing egocentric studies on sports and fast-movement activities.
  </details>

- **[FormGym: Doing Paperwork with Agents](https://arxiv.org/abs/2506.14079)**  `arXiv:2506.14079`  `cs.AI`  
  _Matthew Toles, Rattandeep Singh, Isaac Song Zhou Yu_
  <details open><summary>Abstract</summary>
  Completing paperwork is a challenging and time-consuming problem. Form filling is especially challenging in the pure-image domain without access to OCR, typeset PDF text, or a DOM. For computer agents, it requires multiple abilities, including multi-modal understanding, information retrieval, and tool-use. We present a novel form-filling benchmark consisting of 432 fields spread across 55 documents and 3 tasks, requiring knowledge of 236 features per user. We find that baseline VLAs achieve less than 1% accuracy in most cases, primarily due to poor localization ability. GUI agents also struggle, scoring between 10.6-68.0% despite high cost and latency. Therefore, we also contribute FieldFinder, a tool to assist LLMs in identifying where to place text on a form. With FieldFinder, all models achieve equal or better performance in all six study conditions, with a maximum increase from 2% to 56%.
  </details>
