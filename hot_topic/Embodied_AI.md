# 🔍 Embodied_AI Papers · 2026-07-26

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[Addressing the Orchestration Gap in Generalist Robots via Physical Agency](https://arxiv.org/abs/2607.21725)**  `arXiv:2607.21725`  `cs.RO`  
  _Liane Galanti, Dhruv Shah, Tri Dao_
  <details open><summary>Abstract</summary>
  General-purpose robots need to reason about their actions, combining perception, world knowledge, planning, success detection, recovery, and low-level control. Today's state-of-the-art models attempt to combine all these capabilities into the learned policy via large-scale pre-training. Instead, we show that these capabilities can be decomposed into a general language-conditioned policy/control agent and a high-level agent manager/orchestrator. Rather than training policies to reason via pre-training, we build a closed-loop physical agent orchestrator that can do high-level planning, decompose the goal into achievable subgoals, command low-level motor commands, track and verify the outcome from low-level observations, and recover from failures. Our Physical Agency orchestrator (Pigey) can control existing vision-language-action (VLA) policies as well as parametrized skills to solve complex reasoning tasks in the real world, without any additional data collection or post-training. We evaluate Pigey extensively across simulation benchmarks and challenging real-world robotic manipulation tasks, and demonstrate significant performance improvements over existing generalist policies. On LIBERO-PRO, Pigey advances the state-of-the-art by over 4x (12.8% -> 53.3%) with no task-specific fine-tuning. On a real robot, Pigey lifts the frozen policy from near-zero to over 90% on reasoning-limited tasks. We call the difference between what frozen motor skills achieve alone and inside the agentic loop the orchestration gap.
  </details>

- **[SAFE-Pruner: Semantic Attention-Guided Future-Aware Token Pruning for Efficient Vision-Language-Action Manipulation](https://arxiv.org/abs/2605.29662)**  `arXiv:2605.29662`  `cs.CV` `cs.RO`  
  _Shilin Ma, Chubin Zhang, Changyuan Wang, Yuji Wang, Yue Wu, Zixuan Wang, et al._
  <details open><summary>Abstract</summary>
  Real-time inference of vision-language-action (VLA) models is essential for robotic control. While visual token pruning has shown strong potential for accelerating inference, most existing methods mainly base pruning decisions on shallow-layer cues and risk discarding visual information required by deep layers. To address this issue, we propose SAFE-Pruner, a plug-and-play pruning framework that incorporates attention cues of future layers into pruning decisions. Specifically, we identify semantic attention consistency, the tendency that VLA models concentrate their attention probability mass on the same semantic entity across control timesteps. Based on this observation, we design a forward-looking strategy to forecast the token saliency in deep layers, which prevents the premature removal of critical tokens and leads to more stable acceleration. We further introduce a reference timestep refresh strategy that triggers updates upon attention shifts, thereby improving forecasting accuracy and pruning reliability. Extensive experiments across diverse evaluation settings demonstrate that our method achieves up to 1.89x speedup with a minimal degradation in success rate of less than 1.5%, while outperforming state-of-the-art methods by up to 1.9%.
  </details>

- **[NVIDIA OmniDreams: Real-Time Generative World Model for Closed-Loop Autonomous Vehicle Simulation](https://arxiv.org/abs/2606.03159)**  `arXiv:2606.03159`  `cs.CV` `cs.AI` `cs.RO`  
  _NVIDIA, Aarti Basant, Amlan Kar, Despoina Paschalidou, Fangyin Wei, Francesco Ferroni, et al._
  <details open><summary>Abstract</summary>
  As autonomous vehicle capabilities advance, the safe evaluation of driving policies in long-tail scenarios remains a critical bottleneck. In closed-loop simulation, the driving policy model actively interacts with the environment, where its actions dynamically update the simulator state and directly influence the next set of generated sensor observations. While recent reconstruction-based neural simulators offer photorealism, they are fundamentally constrained by their initial captured data and struggle to generalize to highly dynamic or novel scenes. To overcome these limitations, we introduce OmniDreams, a foundation generative world model mid- and post-trained from the Cosmos diffusion model to autoregressively generate action-conditioned videos in real time. By leveraging the rich visual priors of Cosmos and mid- and post-training on 21k hours of driving scenarios, OmniDreams synthesizes complex, unobserved phenomena that are hard for traditional simulators to capture, such as extreme weather and unpredictable dynamic agent behaviors. Crucially, it autoregressively conditions its photorealistic sensor generation on past frames, the current simulator state, and immediate driving actions. Deployed in a closed-loop system with the Alpamayo 1 policy model and AlpaSim orchestrator, OmniDreams acts as a highly responsive, reactive environment, providing a scalable and comprehensive solution for training and evaluating next-generation autonomous driving policies. We additionally show preliminary results indicating that a world-action model (WAM) post-trained from OmniDreams achieves strong performance on the Physical AI Autonomous Vehicles NuRec dataset, surpassing the VLA-based Alpamayo 1.5 research policy model while using only 1/5 the total parameters. These results highlight the potential for a real-time world model like OmniDreams to also serve as a backbone for policy architectures.
  </details>
