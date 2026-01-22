# 🔍 3D_Generation Papers · 2026-01-21

[![Total Papers](https://img.shields.io/badge/Papers-6-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[LaVR: Scene Latent Conditioned Generative Video Trajectory Re-Rendering using Large 4D Reconstruction Models](https://arxiv.org/abs/2601.14674)**  `arXiv:2601.14674`  `cs.CV` `cs.LG`  
  _Mingyang Xie, Numair Khan, Tianfu Wang, Naina Dhingra, Seonghyeon Nam, Haitao Yang, et al._
  <details open><summary>Abstract</summary>
  Given a monocular video, the goal of video re-rendering is to generate views of the scene from a novel camera trajectory. Existing methods face two distinct challenges. Geometrically unconditioned models lack spatial awareness, leading to drift and deformation under viewpoint changes. On the other hand, geometrically-conditioned models depend on estimated depth and explicit reconstruction, making them susceptible to depth inaccuracies and calibration errors.We propose to address these challenges by using the implicit geometric knowledge embedded in the latent space of a large 4D reconstruction model to condition the video generation process. These latents capture scene structure in a continuous space without explicit reconstruction. Therefore, they provide a flexible representation that allows the pretrained diffusion prior to regularize errors more effectively. By jointly conditioning on these latents and source camera poses, we demonstrate that our model achieves state-of-the-art results on the video re-rendering task. Project webpage isthis https URL
  </details>

- **[Rethinking Video Generation Model for the Embodied World](https://arxiv.org/abs/2601.15282)**  `arXiv:2601.15282`  `cs.CV` `cs.AI` `cs.RO`  
  _Yufan Deng, Zilin Pan, Hongyu Zhang, Xiaojie Li, Ruoqing Hu, Yufei Ding, et al._
  <details open><summary>Abstract</summary>
  Video generation models have significantly advanced embodied intelligence, unlocking new possibilities for generating diverse robot data that capture perception, reasoning, and action in the physical world. However, synthesizing high-quality videos that accurately reflect real-world robotic interactions remains challenging, and the lack of a standardized benchmark limits fair comparisons and progress. To address this gap, we introduce a comprehensive robotics benchmark, RBench, designed to evaluate robot-oriented video generation across five task domains and four distinct embodiments. It assesses both task-level correctness and visual fidelity through reproducible sub-metrics, including structural consistency, physical plausibility, and action completeness. Evaluation of 25 representative models highlights significant deficiencies in generating physically realistic robot behaviors. Furthermore, the benchmark achieves a Spearman correlation coefficient of 0.96 with human evaluations, validating its effectiveness. While RBench provides the necessary lens to identify these deficiencies, achieving physical realism requires moving beyond evaluation to address the critical shortage of high-quality training data. Driven by these insights, we introduce a refined four-stage data pipeline, resulting in RoVid-X, the largest open-source robotic dataset for video generation with 4 million annotated video clips, covering thousands of tasks and enriched with comprehensive physical property annotations. Collectively, this synergistic ecosystem of evaluation and data establishes a robust foundation for rigorous assessment and scalable training of video models, accelerating the evolution of embodied AI toward general intelligence.
  </details>

- **[Walk through Paintings: Egocentric World Models from Internet Priors](https://arxiv.org/abs/2601.15284)**  `arXiv:2601.15284`  `cs.CV`  
  _Anurag Bagchi, Zhipeng Bao, Homanga Bharadhwaj, Yu-Xiong Wang, Pavel Tokmakov, Martial Hebert_
  <details open><summary>Abstract</summary>
  What if a video generation model could not only imagine a plausible future, but the correct one, accurately reflecting how the world changes with each action? We address this question by presenting the Egocentric World Model (EgoWM), a simple, architecture-agnostic method that transforms any pretrained video diffusion model into an action-conditioned world model, enabling controllable future prediction. Rather than training from scratch, we repurpose the rich world priors of Internet-scale video models and inject motor commands through lightweight conditioning layers. This allows the model to follow actions faithfully while preserving realism and strong generalization. Our approach scales naturally across embodiments and action spaces, ranging from 3-DoF mobile robots to 25-DoF humanoids, where predicting egocentric joint-angle-driven dynamics is substantially more challenging. The model produces coherent rollouts for both navigation and manipulation tasks, requiring only modest fine-tuning. To evaluate physical correctness independently of visual appearance, we introduce the Structural Consistency Score (SCS), which measures whether stable scene elements evolve consistently with the provided actions. EgoWM improves SCS by up to 80 percent over prior state-of-the-art navigation world models, while achieving up to six times lower inference latency and robust generalization to unseen environments, including navigation inside paintings.
  </details>

- **[StableWorld: Towards Stable and Consistent Long Interactive Video Generation](https://arxiv.org/abs/2601.15281)**  `arXiv:2601.15281`  `cs.CV`  
  _Ying Yang, Zhengyao Lv, Tianlin Pan, Haofan Wang, Binxin Yang, Hubery Yin, et al._
  <details open><summary>Abstract</summary>
  In this paper, we explore the overlooked challenge of stability and temporal consistency in interactive video generation, which synthesizes dynamic and controllable video worlds through interactive behaviors such as camera movements and text prompts. Despite remarkable progress in world modeling, current methods still suffer from severe instability and temporal degradation, often leading to spatial drift and scene collapse during long-horizon interactions. To better understand this issue, we initially investigate the underlying causes of instability and identify that the major source of error accumulation originates from the same scene, where generated frames gradually deviate from the initial clean state and propagate errors to subsequent frames. Building upon this observation, we propose a simple yet effective method, \textbf{StableWorld}, a Dynamic Frame Eviction Mechanism. By continuously filtering out degraded frames while retaining geometrically consistent ones, StableWorld effectively prevents cumulative drift at its source, leading to more stable and temporal consistency of interactive generation. Promising results on multiple interactive video models, \eg, Matrix-Game, Open-Oasis, and Hunyuan-GameCraft, demonstrate that StableWorld is model-agnostic and can be applied to different interactive video generation frameworks to substantially improve stability, temporal consistency, and generalization across diverse interactive scenarios.
  </details>

- **[Human detectors are surprisingly powerful reward models](https://arxiv.org/abs/2601.14037)**  `arXiv:2601.14037`  `cs.CV`  
  _Kumar Ashutosh, XuDong Wang, Xi Yin, Kristen Grauman, Adam Polyak, Ishan Misra, et al._
  <details open><summary>Abstract</summary>
  Video generation models have recently achieved impressive visual fidelity and temporal coherence. Yet, they continue to struggle with complex, non-rigid motions, especially when synthesizing humans performing dynamic actions such as sports, dance, etc. Generated videos often exhibit missing or extra limbs, distorted poses, or physically implausible actions. In this work, we propose a remarkably simple reward model, HuDA, to quantify and improve the human motion in generated videos. HuDA integrates human detection confidence for appearance quality, and a temporal prompt alignment score to capture motion realism. We show this simple reward function that leverages off-the-shelf models without any additional training, outperforms specialized models finetuned with manually annotated data. Using HuDA for Group Reward Policy Optimization (GRPO) post-training of video models, we significantly enhance video generation, especially when generating complex human motions, outperforming state-of-the-art models like Wan 2.1, with win-rate of 73%. Finally, we demonstrate that HuDA improves generation quality beyond just humans, for instance, significantly improving generation of animal videos and human-object interactions.
  </details>

- **[Sora as a World Model? A Complete Survey on Text-to-Video Generation](https://arxiv.org/abs/2403.05131)**  `arXiv:2403.05131`  `cs.AI` `cs.CV`  
  _Fachrina Dewi Puspitasari, Chaoning Zhang, Joseph Cho, Adnan Haider, Noor Ul Eman, Omer Amin, et al._
  <details open><summary>Abstract</summary>
  The evolution of video generation from text, from animating MNIST to simulating the world with Sora, has progressed at a breakneck speed. Here, we systematically discuss how far text-to-video generation technology supports essential requirements in world modeling. We curate 250+ studies on text-based video synthesis and world modeling. We then observe that recent models increasingly support spatial, action, and strategic intelligences in world modeling through adherence to completeness, consistency, invention, as well as human interaction and control. We conclude that text-to-video generation is adept at world modeling, although homework in several aspects, such as the diversity-consistency trade-offs, remains to be addressed.
  </details>
