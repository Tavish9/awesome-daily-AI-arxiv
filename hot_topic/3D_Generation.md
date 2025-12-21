# 🔍 3D_Generation Papers · 2025-12-20

[![Total Papers](https://img.shields.io/badge/Papers-5-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[TurboDiffusion: Accelerating Video Diffusion Models by 100-200 Times](https://arxiv.org/abs/2512.16093)**  `arXiv:2512.16093`  `cs.CV` `cs.AI` `cs.LG`  
  _Jintao Zhang, Kaiwen Zheng, Kai Jiang, Haoxu Wang, Ion Stoica, Joseph E. Gonzalez, et al._
  <details open><summary>Abstract</summary>
  We introduce TurboDiffusion, a video generation acceleration framework that can speed up end-to-end diffusion generation by 100-200x while maintaining video quality. TurboDiffusion mainly relies on several components for acceleration: (1) Attention acceleration: TurboDiffusion uses low-bit SageAttention and trainable Sparse-Linear Attention (SLA) to speed up attention computation. (2) Step distillation: TurboDiffusion adopts rCM for efficient step distillation. (3) W8A8 quantization: TurboDiffusion quantizes model parameters and activations to 8 bits to accelerate linear layers and compress the model. In addition, TurboDiffusion incorporates several other engineering optimizations.We conduct experiments on the Wan2.2-I2V-14B-720P, Wan2.1-T2V-1.3B-480P, Wan2.1-T2V-14B-720P, and Wan2.1-T2V-14B-480P models. Experimental results show that TurboDiffusion achieves 100-200x speedup for video generation even on a single RTX 5090 GPU, while maintaining comparable video quality. The GitHub repository, which includes model checkpoints and easy-to-use code, is available atthis https URL.
  </details>

- **[Kling-Omni Technical Report](https://arxiv.org/abs/2512.16776)**  `arXiv:2512.16776`  `cs.CV`  
  _Kling Team, Jialu Chen, Yuanzheng Ci, Xiangyu Du, Zipeng Feng, Kun Gai, et al._
  <details open><summary>Abstract</summary>
  We present Kling-Omni, a generalist generative framework designed to synthesize high-fidelity videos directly from multimodal visual language inputs. Adopting an end-to-end perspective, Kling-Omni bridges the functional separation among diverse video generation, editing, and intelligent reasoning tasks, integrating them into a holistic system. Unlike disjointed pipeline approaches, Kling-Omni supports a diverse range of user inputs, including text instructions, reference images, and video contexts, processing them into a unified multimodal representation to deliver cinematic-quality and highly-intelligent video content creation. To support these capabilities, we constructed a comprehensive data system that serves as the foundation for multimodal video creation. The framework is further empowered by efficient large-scale pre-training strategies and infrastructure optimizations for inference. Comprehensive evaluations reveal that Kling-Omni demonstrates exceptional capabilities in in-context generation, reasoning-based editing, and multimodal instruction following. Moving beyond a content creation tool, we believe Kling-Omni is a pivotal advancement toward multimodal world simulators capable of perceiving, reasoning, generating and interacting with the dynamic and complex worlds.
  </details>

- **[Factorized Video Generation: Decoupling Scene Construction and Temporal Synthesis in Text-to-Video Diffusion Models](https://arxiv.org/abs/2512.16371)**  `arXiv:2512.16371`  `cs.CV`  
  _Mariam Hassan, Bastien Van Delft, Wuyang Li, Alexandre Alahi_
  <details open><summary>Abstract</summary>
  State-of-the-art Text-to-Video (T2V) diffusion models can generate visually impressive results, yet they still frequently fail to compose complex scenes or follow logical temporal instructions. In this paper, we argue that many errors, including apparent motion failures, originate from the model's inability to construct a semantically correct or logically consistent initial frame. We introduce Factorized Video Generation (FVG), a pipeline that decouples these tasks by decomposing the Text-to-Video generation into three specialized stages: (1) Reasoning, where a Large Language Model (LLM) rewrites the video prompt to describe only the initial scene, resolving temporal ambiguities; (2) Composition, where a Text-to-Image (T2I) model synthesizes a high-quality, compositionally-correct anchor frame from this new prompt; and (3) Temporal Synthesis, where a video model, finetuned to understand this anchor, focuses its entire capacity on animating the scene and following the prompt. Our decomposed approach sets a new state-of-the-art on the T2V CompBench benchmark and significantly improves all tested models on VBench2. Furthermore, we show that visual anchoring allows us to cut the number of sampling steps by 70% without any loss in performance, leading to a substantial speed-up in sampling. Factorized Video Generation offers a simple yet practical path toward more efficient, robust, and controllable video synthesis
  </details>

- **[Video Reality Test: Can AI-Generated ASMR Videos fool VLMs and Humans?](https://arxiv.org/abs/2512.13281)**  `arXiv:2512.13281`  `cs.CV`  
  _Jiaqi Wang, Weijia Wu, Yi Zhan, Rui Zhao, Ming Hu, James Cheng, et al._
  <details open><summary>Abstract</summary>
  Recent advances in video generation have produced vivid content that are often indistinguishable from real videos, making AI-generated video detection an emerging societal challenge. Prior AIGC detection benchmarks mostly evaluate video without audio, target broad narrative domains, and focus on classification solely. Yet it remains unclear whether state-of-the-art video generation models can produce immersive, audio-paired videos that reliably deceive humans and VLMs. To this end, we introduce Video Reality Test, an ASMR-sourced video benchmark suite for testing perceptual realism under tight audio-visual coupling, featuring the following dimensions: (i) Immersive ASMR video-audio sources. Built on carefully curated real ASMR videos, the benchmark targets fine-grained action-object interactions with diversity across objects, actions, and backgrounds. (ii) Peer-Review evaluation. An adversarial creator-reviewer protocol where video generation models act as creators aiming to fool reviewers, while VLMs serve as reviewers seeking to identify fakeness. Our experimental findings show: The best creator Veo3.1-Fast even fools most VLMs: the strongest reviewer (Gemini 2.5-Pro) achieves only 56% accuracy (random 50%), far below that of human experts (81.25%). Adding audio improves real-fake discrimination, yet superficial cues such as watermarks can still significantly mislead models. These findings delineate the current boundary of video generation realism and expose limitations of VLMs in perceptual fidelity and audio-visual consistency. Our code is available atthis https URL.
  </details>

- **[Live Avatar: Streaming Real-time Audio-Driven Avatar Generation with Infinite Length](https://arxiv.org/abs/2512.04677)**  `arXiv:2512.04677`  `cs.CV`  
  _Yubo Huang, Hailong Guo, Fangtai Wu, Shifeng Zhang, Shijie Huang, Qijun Gan, et al._
  <details open><summary>Abstract</summary>
  Existing diffusion-based video generation methods are fundamentally constrained by sequential computation and long-horizon inconsistency, limiting their practical adoption in real-time, streaming audio-driven avatar synthesis. We present Live Avatar, an algorithm-system co-designed framework that enables efficient, high-fidelity, and infinite-length avatar generation using a 14-billion-parameter diffusion model. Our approach introduces Timestep-forcing Pipeline Parallelism (TPP), a distributed inference paradigm that pipelines denoising steps across multiple GPUs, effectively breaking the autoregressive bottleneck and ensuring stable, low-latency real-time streaming. To further enhance temporal consistency and mitigate identity drift and color artifacts, we propose the Rolling Sink Frame Mechanism (RSFM), which maintains sequence fidelity by dynamically recalibrating appearance using a cached reference image. Additionally, we leverage Self-Forcing Distribution Matching Distillation to facilitate causal, streamable adaptation of large-scale models without sacrificing visual quality. Live Avatar demonstrates state-of-the-art performance, reaching 20 FPS end-to-end generation on 5 H800 GPUs, and, to the best of our knowledge, is the first to achieve practical, real-time, high-fidelity avatar generation at this scale. Our work establishes a new paradigm for deploying advanced diffusion models in industrial long-form video synthesis applications.
  </details>
