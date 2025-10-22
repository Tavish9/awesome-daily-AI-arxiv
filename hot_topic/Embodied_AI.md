# 🔍 Embodied_AI Papers · 2025-10-21

[![Total Papers](https://img.shields.io/badge/Papers-7-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[VLA-Cache: Efficient Vision-Language-Action Manipulation via Adaptive Token Caching](https://arxiv.org/abs/2502.02175)**  `arXiv:2502.02175`  `cs.RO` `cs.CV` `cs.LG`  
  _Siyu Xu, Yunke Wang, Chenghao Xia, Dihao Zhu, Tao Huang, Chang Xu_
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models have demonstrated strong multi-modal reasoning capabilities, enabling direct action generation from visual perception and language instructions in an end-to-end manner. However, their substantial computational cost poses a challenge for real-time robotic control, where rapid decision-making is essential. This paper introduces VLA-Cache, a training-free inference acceleration method that reduces computational overhead by adaptively caching and reusing static visual tokens across frames. Exploiting the temporal continuity in robotic manipulation, VLA-Cache identifies minimally changed tokens between adjacent frames and reuses their cached key-value representations, thereby circumventing redundant computations. Additionally, to maintain action precision, VLA-Cache selectively re-computes task-relevant tokens that are environmentally sensitive, ensuring the fidelity of critical visual information. To further optimize efficiency, we introduce a layer adaptive token reusing strategy that dynamically adjusts the reuse ratio based on attention concentration across decoder layers, prioritizing critical tokens for recomputation. Extensive experiments on two simulation platforms (LIBERO and SIMPLER) and a real-world robotic system demonstrate that VLA-Cache achieves up to 1.7x speedup in CUDA latency and a 15% increase in control frequency, with negligible loss on task success rate. The code and videos can be found at our project page:this https URL.
  </details>

- **[DiffVLA++: Bridging Cognitive Reasoning and End-to-End Driving through Metric-Guided Alignment](https://arxiv.org/abs/2510.17148)**  `arXiv:2510.17148`  `cs.RO` `cs.CV`  
  _Yu Gao, Anqing Jiang, Yiru Wang, Heng Yuwen, Wang Shuo, Sun Hao, et al._
  <details open><summary>Abstract</summary>
  Conventional end-to-end (E2E) driving models are effective at generating physically plausible trajectories, but often fail to generalize to long-tail scenarios due to the lack of essential world knowledge to understand and reason about surrounding environments. In contrast, Vision-Language-Action (VLA) models leverage world knowledge to handle challenging cases, but their limited 3D reasoning capability can lead to physically infeasible actions. In this work we introduce DiffVLA++, an enhanced autonomous driving framework that explicitly bridges cognitive reasoning and E2E planning through metric-guided alignment. First, we build a VLA module directly generating semantically grounded driving trajectories. Second, we design an E2E module with a dense trajectory vocabulary that ensures physical feasibility. Third, and most critically, we introduce a metric-guided trajectory scorer that guides and aligns the outputs of the VLA and E2E modules, thereby integrating their complementary strengths. The experiment on the ICCV 2025 Autonomous Grand Challenge leaderboard shows that DiffVLA++ achieves EPDMS of 49.12.
  </details>

- **[Learning to See and Act: Task-Aware View Planning for Robotic Manipulation](https://arxiv.org/abs/2508.05186)**  `arXiv:2508.05186`  `cs.RO` `cs.CV`  
  _Yongjie Bai, Zhouxia Wang, Yang Liu, Weixing Chen, Ziliang Chen, Mingtong Dai, et al._
  <details open><summary>Abstract</summary>
  Recent vision-language-action (VLA) models for multi-task robotic manipulation commonly rely on static viewpoints and shared visual encoders, which limit 3D perception and cause task interference, hindering robustness and generalization. In this work, we propose Task-Aware View Planning (TAVP), a framework designed to overcome these challenges by integrating active view planning with task-specific representation learning. TAVP employs an efficient exploration policy, accelerated by a novel pseudo-environment, to actively acquire informative views. Furthermore, we introduce a Mixture-of-Experts (MoE) visual encoder to disentangle features across different tasks, boosting both representation fidelity and task generalization. By learning to see the world in a task-aware way, TAVP generates more complete and discriminative visual representations, demonstrating significantly enhanced action prediction across a wide array of manipulation challenges. Extensive experiments on RLBench tasks show that our proposed TAVP model achieves superior performance over state-of-the-art fixed-view approaches. Visual results and code are provided at:this https URL.
  </details>

- **[NEBULA: Do We Evaluate Vision-Language-Action Agents Correctly?](https://arxiv.org/abs/2510.16263)**  `arXiv:2510.16263`  `cs.RO` `cs.AI` `cs.CV`  
  _Jierui Peng, Yanyan Zhang, Yicheng Duan, Tuo Liang, Vipin Chaudhary, Yu Yin_
  <details open><summary>Abstract</summary>
  The evaluation of Vision-Language-Action (VLA) agents is hindered by the coarse, end-task success metric that fails to provide precise skill diagnosis or measure robustness to real-world perturbations. This challenge is exacerbated by a fragmented data landscape that impedes reproducible research and the development of generalist models. To address these limitations, we introduce NEBULA, a unified ecosystem for single-arm manipulation that enables diagnostic and reproducible evaluation. NEBULA features a novel dual-axis evaluation protocol that combines fine-grained capability tests for precise skill diagnosis with systematic stress tests that measure robustness. A standardized API and a large-scale, aggregated dataset are provided to reduce fragmentation and support cross-dataset training and fair comparison. Using NEBULA, we demonstrate that top-performing VLAs struggle with key capabilities such as spatial reasoning and dynamic adaptation, which are consistently obscured by conventional end-task success metrics. By measuring both what an agent can do and when it does so reliably, NEBULA provides a practical foundation for robust, general-purpose embodied agents.
  </details>

- **[MoTVLA: A Vision-Language-Action Model with Unified Fast-Slow Reasoning](https://arxiv.org/abs/2510.18337)**  `arXiv:2510.18337`  `cs.RO`  
  _Wenhui Huang, Changhe Chen, Han Qi, Chen Lv, Yilun Du, Heng Yang_
  <details open><summary>Abstract</summary>
  Integrating visual-language instructions into visuomotor policies is gaining momentum in robot learning for enhancing open-world generalization. Despite promising advances, existing approaches face two challenges: limited language steerability when no generated reasoning is used as a condition, or significant inference latency when reasoning isthis http URLthis work, we introduce MoTVLA, a mixture-of-transformers (MoT)-based vision-language-action (VLA) model that integrates fast-slow unified reasoning with behavior policy learning. MoTVLA preserves the general intelligence of pre-trained VLMs (serving as the generalist) for tasks such as perception, scene understanding, and semantic planning, while incorporating a domain expert, a second transformer that shares knowledge with the pretrained VLM, to generate domain-specific fast reasoning (e.g., robot motion decomposition), thereby improving policy execution efficiency. By conditioning the action expert on decomposed motion instructions, MoTVLA can learn diverse behaviors and substantially improve language steerability. Extensive evaluations across natural language processing benchmarks, robotic simulation environments, and real-world experiments confirm the superiority of MoTVLA in both fast-slow reasoning and manipulation task performance.
  </details>

- **[RoboChallenge: Large-scale Real-robot Evaluation of Embodied Policies](https://arxiv.org/abs/2510.17950)**  `arXiv:2510.17950`  `cs.RO`  
  _Adina Yakefu, Bin Xie, Chongyang Xu, Enwen Zhang, Erjin Zhou, Fan Jia, et al._
  <details open><summary>Abstract</summary>
  Testing on real machines is indispensable for robotic control algorithms. In the context of learning-based algorithms, especially VLA models, demand for large-scale evaluation, i.e. testing a large number of models on a large number of tasks, is becoming increasingly urgent. However, doing this right is highly non-trivial, especially when scalability and reproducibility is taken into account. In this report, we describe our methodology for constructing RoboChallenge, an online evaluation system to test robotic control algorithms, and our survey of recent state-of-the-art VLA models using our initial benchmark Table30.
  </details>

- **[Goal-VLA: Image-Generative VLMs as Object-Centric World Models Empowering Zero-shot Robot Manipulation](https://arxiv.org/abs/2506.23919)**  `arXiv:2506.23919`  `cs.RO`  
  _Haonan Chen, Jingxiang Guo, Bangjun Wang, Tianrui Zhang, Xuchuan Huang, Boren Zheng, et al._
  <details open><summary>Abstract</summary>
  Generalization remains a fundamental challenge in robotic manipulation. To tackle this challenge, recent Vision-Language-Action (VLA) models build policies on top of Vision-Language Models (VLMs), seeking to transfer their open-world semantic knowledge. However, their zero-shot capability lags significantly behind the base VLMs, as the instruction-vision-action data is too limited to cover diverse scenarios, tasks, and robot embodiments. In this work, we present Goal-VLA, a zero-shot framework that leverages Image-Generative VLMs as world models to generate desired goal states, from which the target object pose is derived to enable generalizable manipulation. The key insight is that object state representation is the golden interface, naturally separating a manipulation system into high-level and low-level policies. This representation abstracts away explicit action annotations, allowing the use of highly generalizable VLMs while simultaneously providing spatial cues for training-free low-level control. To further improve robustness, we introduce a Reflection-through-Synthesis process that iteratively validates and refines the generated goal image before execution. Both simulated and real-world experiments demonstrate that our \name achieves strong performance and inspiring generalizability in manipulation tasks. Supplementary materials are available atthis https URL.
  </details>
