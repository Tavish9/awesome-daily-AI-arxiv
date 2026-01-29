# 🔍 3D_Generation Papers · 2026-01-28

[![Total Papers](https://img.shields.io/badge/Papers-7-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[FAIRT2V: Training-Free Debiasing for Text-to-Video Diffusion Models](https://arxiv.org/abs/2601.20791)**  `arXiv:2601.20791`  `cs.CV` `cs.AI`  
  _Haonan Zhong, Wei Song, Tingxu Han, Maurice Pagnucco, Jingling Xue, Yang Song_
  <details open><summary>Abstract</summary>
  Text-to-video (T2V) diffusion models have achieved rapid progress, yet their demographic biases, particularly gender bias, remain largely unexplored. We present FairT2V, a training-free debiasing framework for text-to-video generation that mitigates encoder-induced bias without finetuning. We first analyze demographic bias in T2V models and show that it primarily originates from pretrained text encoders, which encode implicit gender associations even for neutral prompts. We quantify this effect with a gender-leaning score that correlates with bias in generated videos.Based on this insight, FairT2V mitigates demographic bias by neutralizing prompt embeddings via anchor-based spherical geodesic transformations while preserving semantics. To maintain temporal coherence, we apply debiasing only during early identity-forming steps through a dynamic denoising schedule. We further propose a video-level fairness evaluation protocol combining VideoLLM-based reasoning with human verification. Experiments on the modern T2V model Open-Sora show that FairT2V substantially reduces demographic bias across occupations with minimal impact on video quality.
  </details>

- **[Advancing Open-source World Models](https://arxiv.org/abs/2601.20540)**  `arXiv:2601.20540`  `cs.CV`  
  _Robbyant Team, Zelin Gao, Qiuyu Wang, Yanhong Zeng, Jiapeng Zhu, Ka Leong Cheng, et al._
  <details open><summary>Abstract</summary>
  We present LingBot-World, an open-sourced world simulator stemming from video generation. Positioned as a top-tier world model, LingBot-World offers the following features. (1) It maintains high fidelity and robust dynamics in a broad spectrum of environments, including realism, scientific contexts, cartoon styles, and beyond. (2) It enables a minute-level horizon while preserving contextual consistency over time, which is also known as "long-term memory". (3) It supports real-time interactivity, achieving a latency of under 1 second when producing 16 frames per second. We provide public access to the code and model in an effort to narrow the divide between open-source and closed-source technologies. We believe our release will empower the community with practical applications across areas like content creation, gaming, and robot learning.
  </details>

- **[Latent Temporal Discrepancy as Motion Prior: A Loss-Weighting Strategy for Dynamic Fidelity in T2V](https://arxiv.org/abs/2601.20504)**  `arXiv:2601.20504`  `cs.CV`  
  _Meiqi Wu, Bingze Song, Ruimin Lin, Chen Zhu, Xiaokun Feng, Jiahong Wu, et al._
  <details open><summary>Abstract</summary>
  Video generation models have achieved notable progress in static scenarios, yet their performance in motion video generation remains limited, with quality degrading under drastic dynamic changes. This is due to noise disrupting temporal coherence and increasing the difficulty of learning dynamic regions. {Unfortunately, existing diffusion models rely on static loss for all scenarios, constraining their ability to capture complex dynamics.} To address this issue, we introduce Latent Temporal Discrepancy (LTD) as a motion prior to guide loss weighting. LTD measures frame-to-frame variation in the latent space, assigning larger penalties to regions with higher discrepancy while maintaining regular optimization for stable regions. This motion-aware strategy stabilizes training and enables the model to better reconstruct high-frequency dynamics. Extensive experiments on the general benchmark VBench and the motion-focused VMBench show consistent gains, with our method outperforming strong baselines by 3.31% on VBench and 3.58% on VMBench, achieving significant improvements in motion quality.
  </details>

- **[Efficient Autoregressive Video Diffusion with Dummy Head](https://arxiv.org/abs/2601.20499)**  `arXiv:2601.20499`  `cs.CV`  
  _Hang Guo, Zhaoyang Jia, Jiahao Li, Bin Li, Yuanhao Cai, Jiangshan Wang, et al._
  <details open><summary>Abstract</summary>
  The autoregressive video diffusion model has recently gained considerable research interest due to its causal modeling and iterative denoising. In this work, we identify that the multi-head self-attention in these models under-utilizes historical frames: approximately 25% heads attend almost exclusively to the current frame, and discarding their KV caches incurs only minor performance degradation. Building upon this, we propose Dummy Forcing, a simple yet effective method to control context accessibility across different heads. Specifically, the proposed heterogeneous memory allocation reduces head-wise context redundancy, accompanied by dynamic head programming to adaptively classify head types. Moreover, we develop a context packing technique to achieve more aggressive cache compression. Without additional training, our Dummy Forcing delivers up to 2.0x speedup over the baseline, supporting video generation at 24.3 FPS with less than 0.5% quality drop. Project page is available atthis https URL.
  </details>

- **[TPGDiff: Hierarchical Triple-Prior Guided Diffusion for Image Restoration](https://arxiv.org/abs/2601.20306)**  `arXiv:2601.20306`  `cs.CV`  
  _Yanjie Tu, Qingsen Yan, Axi Niu, Jiacong Tang_
  <details open><summary>Abstract</summary>
  All-in-one image restoration aims to address diverse degradation types using a single unified model. Existing methods typically rely on degradation priors to guide restoration, yet often struggle to reconstruct content in severely degraded regions. Although recent works leverage semantic information to facilitate content generation, integrating it into the shallow layers of diffusion models often disrupts spatial structures (\emph{e.g.}, blurring artifacts). To address this issue, we propose a Triple-Prior Guided Diffusion (TPGDiff) network for unified image restoration. TPGDiff incorporates degradation priors throughout the diffusion trajectory, while introducing structural priors into shallow layers and semantic priors into deep layers, enabling hierarchical and complementary prior guidance for image reconstruction. Specifically, we leverage multi-source structural cues as structural priors to capture fine-grained details and guide shallow layers representations. To complement this design, we further develop a distillation-driven semantic extractor that yields robust semantic priors, ensuring reliable high-level guidance at deep layers even under severe degradations. Furthermore, a degradation extractor is employed to learn degradation-aware priors, enabling stage-adaptive control of the diffusion process across all timesteps. Extensive experiments on both single- and multi-degradation benchmarks demonstrate that TPGDiff achieves superior performance and generalization across diverse restoration scenarios. Our project page is:this https URL.
  </details>

- **[Artifact-Aware Evaluation for High-Quality Video Generation](https://arxiv.org/abs/2601.20297)**  `arXiv:2601.20297`  `cs.CV`  
  _Chen Zhu, Jiashu Zhu, Yanxun Li, Meiqi Wu, Bingze Song, Chubin Chen, et al._
  <details open><summary>Abstract</summary>
  With the rapid advancement of video generation techniques, evaluating and auditing generated videos has become increasingly crucial. Existing approaches typically offer coarse video quality scores, lacking detailed localization and categorization of specific artifacts. In this work, we introduce a comprehensive evaluation protocol focusing on three key aspects affecting human perception: Appearance, Motion, and Camera. We define these axes through a taxonomy of 10 prevalent artifact categories reflecting common generative failures observed in video generation. To enable robust artifact detection and categorization, we introduce GenVID, a large-scale dataset of 80k videos generated by various state-of-the-art video generation models, each carefully annotated for the defined artifact categories. Leveraging GenVID, we develop DVAR, a Dense Video Artifact Recognition framework for fine-grained identification and classification of generative artifacts. Extensive experiments show that our approach significantly improves artifact detection accuracy and enables effective filtering of low-quality content.
  </details>

- **[TwinFlow: Realizing One-step Generation on Large Models with Self-adversarial Flows](https://arxiv.org/abs/2512.05150)**  `arXiv:2512.05150`  `cs.CV`  
  _Zhenglin Cheng, Peng Sun, Jianguo Li, Tao Lin_
  <details open><summary>Abstract</summary>
  Recent advances in large multi-modal generative models have demonstrated impressive capabilities in multi-modal generation, including image and video generation. These models are typically built upon multi-step frameworks like diffusion and flow matching, which inherently limits their inference efficiency (requiring 40-100 Number of Function Evaluations (NFEs)). While various few-step methods aim to accelerate the inference, existing solutions have clear limitations. Prominent distillation-based methods, such as progressive and consistency distillation, either require an iterative distillation procedure or show significant degradation at very few steps (< 4-NFE). Meanwhile, integrating adversarial training into distillation (e.g., DMD/DMD2 and SANA-Sprint) to enhance performance introduces training instability, added complexity, and high GPU memory overhead due to the auxiliary trained models. To this end, we propose TwinFlow, a simple yet effective framework for training 1-step generative models that bypasses the need of fixed pretrained teacher models and avoids standard adversarial networks during training, making it ideal for building large-scale, efficient models. On text-to-image tasks, our method achieves a GenEval score of 0.83 in 1-NFE, outperforming strong baselines like SANA-Sprint (a GAN loss-based framework) and RCGM (a consistency-based framework). Notably, we demonstrate the scalability of TwinFlow by full-parameter training on Qwen-Image-20B and transform it into an efficient few-step generator. With just 1-NFE, our approach matches the performance of the original 100-NFE model on both the GenEval and DPG-Bench benchmarks, reducing computational cost by $100\times$ with minor quality degradation. Project page is available atthis https URL.
  </details>
