# 🔍 Embodied_AI Papers · 2025-10-26

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[SutureBot: A Precision Framework & Benchmark For Autonomous End-to-End Suturing](https://arxiv.org/abs/2510.20965)**  `arXiv:2510.20965`  `cs.RO` `cs.LG`  
  _Jesse Haworth, Juo-Tung Chen, Nigel Nelson, Ji Woong Kim, Masoud Moghani, Chelsea Finn, et al._
  <details open><summary>Abstract</summary>
  Robotic suturing is a prototypical long-horizon dexterous manipulation task, requiring coordinated needle grasping, precise tissue penetration, and secure knot tying. Despite numerous efforts toward end-to-end autonomy, a fully autonomous suturing pipeline has yet to be demonstrated on physical hardware. We introduce SutureBot: an autonomous suturing benchmark on the da Vinci Research Kit (dVRK), spanning needle pickup, tissue insertion, and knot tying. To ensure repeatability, we release a high-fidelity dataset comprising 1,890 suturing demonstrations. Furthermore, we propose a goal-conditioned framework that explicitly optimizes insertion-point precision, improving targeting accuracy by 59\%-74\% over a task-only baseline. To establish this task as a benchmark for dexterous imitation learning, we evaluate state-of-the-art vision-language-action (VLA) models, including $\pi_0$, GR00T N1, OpenVLA-OFT, and multitask ACT, each augmented with a high-level task-prediction policy. Autonomous suturing is a key milestone toward achieving robotic autonomy in surgery. These contributions support reproducible evaluation and development of precision-focused, long-horizon dexterous manipulation policies necessary for end-to-end suturing. Dataset is available at:this https URL
  </details>

- **[LIBERO-Plus: In-depth Robustness Analysis of Vision-Language-Action Models](https://arxiv.org/abs/2510.13626)**  `arXiv:2510.13626`  `cs.RO` `cs.CL` `cs.CV`  
  _Senyu Fei, Siyin Wang, Junhao Shi, Zihao Dai, Jikun Cai, Pengfang Qian, et al._
  <details open><summary>Abstract</summary>
  Visual-Language-Action (VLA) models report impressive success rates on robotic manipulation benchmarks, yet these results may mask fundamental weaknesses in robustness. We perform a systematic vulnerability analysis by introducing controlled perturbations across seven dimensions: objects layout, camera viewpoints, robot initial states, language instructions, light conditions, background textures and sensor noise. We comprehensively analyzed multiple state-of-the-art models and revealed consistent brittleness beneath apparent competence. Our analysis exposes critical weaknesses: models exhibit extreme sensitivity to perturbation factors, including camera viewpoints and robot initial states, with performance dropping from 95% to below 30% under modest perturbations. Surprisingly, models are largely insensitive to language variations, with further experiments revealing that models tend to ignore language instructions completely. Our findings challenge the assumption that high benchmark scores equate to true competency and highlight the need for evaluation practices that assess reliability under realistic variation.
  </details>

- **[RESample: A Robust Data Augmentation Framework via Exploratory Sampling for Robotic Manipulation](https://arxiv.org/abs/2510.17640)**  `arXiv:2510.17640`  `cs.RO` `cs.AI` `cs.LG`  
  _Yuquan Xue, Guanxing Lu, Zhenyu Wu, Chuanrui Zhang, Bofang Jia, Zhengyi Gu, et al._
  <details open><summary>Abstract</summary>
  Vision-Language-Action models (VLAs) have demonstrated remarkable performance on complex robotic manipulation tasks through imitation learning. However, existing imitation learning datasets contain only successful trajectories and lack failure or recovery data, especially for out-of-distribution (OOD) states where the robot deviates from the main policy due to minor perturbations or errors, leading VLA models to struggle with states deviating from the training distribution. To this end, we propose an automated OOD data augmentation framework named RESample through exploratory sampling. Specifically, we first leverage offline reinforcement learning to obtain an action-value network that accurately identifies sub-optimal actions under the current manipulation policy. We further sample potential OOD states from trajectories via rollout, and design an exploratory sampling mechanism that adaptively incorporates these action proxies into the training dataset to ensure efficiency. Subsequently, our framework explicitly encourages the VLAs to recover from OOD states and enhances their robustness against distributional shifts. We conduct extensive experiments on the LIBERO benchmark as well as real-world robotic manipulation tasks, demonstrating that RESample consistently improves the stability and generalization ability of VLA models.
  </details>

- **[Scalable Vision-Language-Action Model Pretraining for Robotic Manipulation with Real-Life Human Activity Videos](https://arxiv.org/abs/2510.21571)**  `arXiv:2510.21571`  `cs.RO` `cs.AI` `cs.CV` `cs.LG`  
  _Qixiu Li, Yu Deng, Yaobo Liang, Lin Luo, Lei Zhou, Chengtang Yao, et al._
  <details open><summary>Abstract</summary>
  This paper presents a novel approach for pretraining robotic manipulation Vision-Language-Action (VLA) models using a large corpus of unscripted real-life video recordings of human hand activities. Treating human hand as dexterous robot end-effector, we show that "in-the-wild" egocentric human videos without any annotations can be transformed into data formats fully aligned with existing robotic V-L-A training data in terms of task granularity and labels. This is achieved by the development of a fully-automated holistic human activity analysis approach for arbitrary human hand videos. This approach can generate atomic-level hand activity segments and their language descriptions, each accompanied with framewise 3D hand motion and camera motion. We process a large volume of egocentric videos and create a hand-VLA training dataset containing 1M episodes and 26M frames. This training data covers a wide range of objects and concepts, dexterous manipulation tasks, and environment variations in real life, vastly exceeding the coverage of existing robot data. We design a dexterous hand VLA model architecture and pretrain the model on this dataset. The model exhibits strong zero-shot capabilities on completely unseen real-world observations. Additionally, fine-tuning it on a small amount of real robot action data significantly improves task success rates and generalization to novel objects in real robotic experiments. We also demonstrate the appealing scaling behavior of the model's task performance with respect to pretraining data scale. We believe this work lays a solid foundation for scalable VLA pretraining, advancing robots toward truly generalizable embodied intelligence.
  </details>
