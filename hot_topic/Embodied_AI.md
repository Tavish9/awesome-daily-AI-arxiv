# 🔍 Embodied_AI Papers · 2026-05-05

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[RLDX-1 Technical Report](https://arxiv.org/abs/2605.03269)**  `arXiv:2605.03269`  `cs.RO` `cs.AI` `cs.LG`  
  _Dongyoung Kim, Huiwon Jang, Myungkyu Koo, Suhyeok Jang, Taeyoung Kim, Beomjun Kim, et al._
  <details open><summary>Abstract</summary>
  While Vision-Language-Action models (VLAs) have shown remarkable progress toward human-like generalist robotic policies through the versatile intelligence (i.e. broad scene understanding and language-conditioned generalization) inherited from pre-trained Vision-Language Models, they still struggle with complex real-world tasks requiring broader functional capabilities (e.g. motion awareness, memory-aware decision making, and physical sensing). To address this, we introduce RLDX-1, a general-purpose robotic policy for dexterous manipulation built on the Multi-Stream Action Transformer (MSAT), an architecture that unifies these capabilities by integrating heterogeneous modalities through modality-specific streams with cross-modal joint self-attention. RLDX-1 further combines this architecture with system-level design choices, including synthesizing training data for rare manipulation scenarios, learning procedures specialized for human-like manipulation, and inference optimizations for real-time deployment. Through empirical evaluation, we show that RLDX-1 consistently outperforms recent frontier VLAs (e.g. $\pi_{0.5}$ and GR00T N1.6) across both simulation benchmarks and real-world tasks that require broad functional capabilities beyond general versatility. In particular, RLDX-1 shows superiority in ALLEX humanoid tasks by achieving success rates of 86.8% while $\pi_{0.5}$ and GR00T N1.6 achieve around 40%, highlighting the ability of RLDX-1 to control a high-DoF humanoid robot under diverse functional demands. Together, these results position RLDX-1 as a promising step toward reliable VLAs for complex, contact-rich, and dynamic real-world dexterous manipulation.
  </details>

- **[AhaRobot: A Low-Cost Open-Source Bimanual Mobile Manipulator for Embodied AI](https://arxiv.org/abs/2503.10070)**  `arXiv:2503.10070`  `cs.RO` `cs.AI` `cs.LG`  
  _Haiqin Cui, Yifu Yuan, Yan Zheng, Jianye Hao_
  <details open><summary>Abstract</summary>
  Scaling Vision-Language-Action models for embodied manipulation demands large volumes of diverse manipulation data, yet the high cost of commercial mobile manipulators and teleoperation interfaces that are difficult to deploy at scale remain key bottlenecks. We present AhaRobot, a low-cost, fully open-source bimanual mobile manipulator tailored for Embodied-AI. The system contributes: (1) a SCARA-like dual-arm hardware design that reduces motor torque demands while maintaining a large vertical reachable workspace, (2) an optimized control stack that improves precision via dual-motor backlash mitigation and static-friction compensation through dithering, and (3) RoboPilot, a teleoperation interface featuring a novel 26-faced marker handle for precise, long-horizon remote data collection. Experimental results show that our hardware-control co-design achieves 0.7 mm repeatability at a total hardware cost of only $1,000. The proposed 26-faced handle reduces tracking error by 80% over a 6-faced baseline and improves data-collection efficiency by 30%, while robustly handling singularities and supporting extremely long-horizon tasks in fully remote settings. Despite its low cost, AhaRobot enables imitation learning of complex household behaviors involving bimanual coordination, upper-body mobility, and contact-rich interaction, with data quality comparable to VR-based collection. All software, CAD files, and documentation are available atthis https URL.
  </details>

- **[Can Explicit Physical Feasibility Benefit VLA Learning? An Empirical Study](https://arxiv.org/abs/2604.17896)**  `arXiv:2604.17896`  `cs.LG` `cs.AI` `cs.RO`  
  _Yubai Wei, Chen Wu, Hashem Haghbayan_
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models map multimodal inputs directly to robot actions and are typically trained through large-scale imitation learning. While this paradigm has shown strong performance, prevailing VLA training procedures do not explicitly supervise hard physical constraints such as obstacle avoidance or kinematic feasibility. As a result, the geometric structure underlying physically feasible behavior must be inferred only implicitly from demonstrations. In this paper, we study whether introducing explicit feasibility supervision can provide effective structured guidance for VLA policies. We formulate a simple geometry-grounded feasibility objective and integrate it into the training stage of a diffusion-based VLA policy. To evaluate this idea systematically, we use obstacle-aware manipulation as a controlled probe of geometry-dependent physical feasibility. Empirical results show that augmenting VLA training with feasibility supervision improves both physical reliability and overall task performance, while also enhancing learning efficiency in the low-data regime. These findings indicate that explicit feasibility signals can effectively complement imitation-based VLA learning, highlighting their potential for developing more reliable VLA policies.
  </details>
