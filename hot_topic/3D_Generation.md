# 🔍 3D_Generation Papers · 2025-11-05

[![Total Papers](https://img.shields.io/badge/Papers-6-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Generative View Stitching](https://arxiv.org/abs/2510.24718)**  `arXiv:2510.24718`  `cs.CV` `cs.LG`  
  _Chonghyuk Song, Michal Stary, Boyuan Chen, George Kopanas, Vincent Sitzmann_
  <details open><summary>Abstract</summary>
  Autoregressive video diffusion models are capable of long rollouts that are stable and consistent with history, but they are unable to guide the current generation with conditioning from the future. In camera-guided video generation with a predefined camera trajectory, this limitation leads to collisions with the generated scene, after which autoregression quickly collapses. To address this, we propose Generative View Stitching (GVS), which samples the entire sequence in parallel such that the generated scene is faithful to every part of the predefined camera trajectory. Our main contribution is a sampling algorithm that extends prior work on diffusion stitching for robot planning to video generation. While such stitching methods usually require a specially trained model, GVS is compatible with any off-the-shelf video model trained with Diffusion Forcing, a prevalent sequence diffusion framework that we show already provides the affordances necessary for stitching. We then introduce Omni Guidance, a technique that enhances the temporal consistency in stitching by conditioning on both the past and future, and that enables our proposed loop-closing mechanism for delivering long-range coherence. Overall, GVS achieves camera-guided video generation that is stable, collision-free, frame-to-frame consistent, and closes loops for a variety of predefined camera paths, including Oscar Reutersvärd's Impossible Staircase. Results are best viewed as videos atthis https URL.
  </details>

- **[Reg-DPO: SFT-Regularized Direct Preference Optimization with GT-Pair for Improving Video Generation](https://arxiv.org/abs/2511.01450)**  `arXiv:2511.01450`  `cs.CV` `cs.AI`  
  _Jie Du, Xinyu Gong, Qingshan Tan, Wen Li, Yangming Cheng, Weitao Wang, et al._
  <details open><summary>Abstract</summary>
  Recent studies have identified Direct Preference Optimization (DPO) as an efficient and reward-free approach to improving video generation quality. However, existing methods largely follow image-domain paradigms and are mainly developed on small-scale models (approximately 2B parameters), limiting their ability to address the unique challenges of video tasks, such as costly data construction, unstable training, and heavy memory consumption. To overcome these limitations, we introduce a GT-Pair that automatically builds high-quality preference pairs by using real videos as positives and model-generated videos as negatives, eliminating the need for any external annotation. We further present Reg-DPO, which incorporates the SFT loss as a regularization term into the DPO loss to enhance training stability and generation fidelity. Additionally, by combining the FSDP framework with multiple memory optimization techniques, our approach achieves nearly three times higher training capacity than using FSDP alone. Extensive experiments on both I2V and T2V tasks across multiple datasets demonstrate that our method consistently outperforms existing approaches, delivering superior video generation quality.
  </details>

- **[A Survey on Text-Driven 360-Degree Panorama Generation](https://arxiv.org/abs/2502.14799)**  `arXiv:2502.14799`  `cs.CV` `cs.AI`  
  _Hai Wang, Xiaoyu Xiang, Weihao Xia, Jing-Hao Xue_
  <details open><summary>Abstract</summary>
  The advent of text-driven 360-degree panorama generation, enabling the synthesis of 360-degree panoramic images directly from textual descriptions, marks a transformative advancement in immersive visual content creation. This innovation significantly simplifies the traditionally complex process of producing such content. Recent progress in text-to-image diffusion models has accelerated the rapid development in this emerging field. This survey presents a comprehensive review of text-driven 360-degree panorama generation, offering an in-depth analysis of state-of-the-art algorithms. We extend our analysis to two closely related domains: text-driven 360-degree 3D scene generation and text-driven 360-degree panoramic video generation. Furthermore, we critically examine current limitations and propose promising directions for future research. A curated project page with relevant resources and research papers is available atthis https URL.
  </details>

- **[UniAVGen: Unified Audio and Video Generation with Asymmetric Cross-Modal Interactions](https://arxiv.org/abs/2511.03334)**  `arXiv:2511.03334`  `cs.CV`  
  _Guozhen Zhang, Zixiang Zhou, Teng Hu, Ziqiao Peng, Youliang Zhang, Yi Chen, et al._
  <details open><summary>Abstract</summary>
  Due to the lack of effective cross-modal modeling, existing open-source audio-video generation methods often exhibit compromised lip synchronization and insufficient semantic consistency. To mitigate these drawbacks, we propose UniAVGen, a unified framework for joint audio and video generation. UniAVGen is anchored in a dual-branch joint synthesis architecture, incorporating two parallel Diffusion Transformers (DiTs) to build a cohesive cross-modal latent space. At its heart lies an Asymmetric Cross-Modal Interaction mechanism, which enables bidirectional, temporally aligned cross-attention, thus ensuring precise spatiotemporal synchronization and semantic consistency. Furthermore, this cross-modal interaction is augmented by a Face-Aware Modulation module, which dynamically prioritizes salient regions in the interaction process. To enhance generative fidelity during inference, we additionally introduce Modality-Aware Classifier-Free Guidance, a novel strategy that explicitly amplifies cross-modal correlation signals. Notably, UniAVGen's robust joint synthesis design enables seamless unification of pivotal audio-video tasks within a single model, such as joint audio-video generation and continuation, video-to-audio dubbing, and audio-driven video synthesis. Comprehensive experiments validate that, with far fewer training samples (1.3M vs. 30.1M), UniAVGen delivers overall advantages in audio-video synchronization, timbre consistency, and emotion consistency.
  </details>

- **[Unified Long Video Inpainting and Outpainting via Overlapping High-Order Co-Denoising](https://arxiv.org/abs/2511.03272)**  `arXiv:2511.03272`  `cs.CV`  
  _Shuangquan Lyu, Steven Mao, Yue Ma_
  <details open><summary>Abstract</summary>
  Generating long videos remains a fundamental challenge, and achieving high controllability in video inpainting and outpainting is particularly demanding. To address both of these challenges simultaneously and achieve controllable video inpainting and outpainting for long video clips, we introduce a novel and unified approach for long video inpainting and outpainting that extends text-to-video diffusion models to generate arbitrarily long, spatially edited videos with high fidelity. Our method leverages LoRA to efficiently fine-tune a large pre-trained video diffusion model like Alibaba's Wan 2.1 for masked region video synthesis, and employs an overlap-and-blend temporal co-denoising strategy with high-order solvers to maintain consistency across long sequences. In contrast to prior work that struggles with fixed-length clips or exhibits stitching artifacts, our system enables arbitrarily long video generation and editing without noticeable seams or drift. We validate our approach on challenging inpainting/outpainting tasks including editing or adding objects over hundreds of frames and demonstrate superior performance to baseline methods like Wan 2.1 model and VACE in terms of quality (PSNR/SSIM), and perceptual realism (LPIPS). Our method enables practical long-range video editing with minimal overhead, achieved a balance between parameter efficient and superior performance.
  </details>

- **[MagCache: Fast Video Generation with Magnitude-Aware Cache](https://arxiv.org/abs/2506.09045)**  `arXiv:2506.09045`  `cs.CV`  
  _Zehong Ma, Longhui Wei, Feng Wang, Shiliang Zhang, Qi Tian_
  <details open><summary>Abstract</summary>
  Existing acceleration techniques for video diffusion models often rely on uniform heuristics or time-embedding variants to skip timesteps and reuse cached features. These approaches typically require extensive calibration with curated prompts and risk inconsistent outputs due to prompt-specific overfitting. In this paper, we introduce a novel and robust discovery: a unified magnitude law observed across different models and prompts. Specifically, the magnitude ratio of successive residual outputs decreases monotonically, steadily in most timesteps while rapidly in the last several steps. Leveraging this insight, we introduce a Magnitude-aware Cache (MagCache) that adaptively skips unimportant timesteps using an error modeling mechanism and adaptive caching strategy. Unlike existing methods requiring dozens of curated samples for calibration, MagCache only requires a single sample for calibration. Experimental results show that MagCache achieves 2.10x-2.68x speedups on Open-Sora, CogVideoX, Wan 2.1, and HunyuanVideo, while preserving superior visual fidelity. It significantly outperforms existing methods in LPIPS, SSIM, and PSNR, under similar computational budgets.
  </details>
