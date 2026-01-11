# 🔍 3D_Generation Papers · 2026-01-10

[![Total Papers](https://img.shields.io/badge/Papers-5-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[RoboVIP: Multi-View Video Generation with Visual Identity Prompting Augments Robot Manipulation](https://arxiv.org/abs/2601.05241)**  `arXiv:2601.05241`  `cs.CV` `cs.AI` `cs.RO`  
  _Boyang Wang, Haoran Zhang, Shujie Zhang, Jinkun Hao, Mingda Jia, Qi Lv, et al._
  <details open><summary>Abstract</summary>
  The diversity, quantity, and quality of manipulation data are critical for training effective robot policies. However, due to hardware and physical setup constraints, collecting large-scale real-world manipulation data remains difficult to scale across diverse environments. Recent work uses text-prompt conditioned image diffusion models to augment manipulation data by altering the backgrounds and tabletop objects in the visual observations. However, these approaches often overlook the practical need for multi-view and temporally coherent observations required by state-of-the-art policy models. Further, text prompts alone cannot reliably specify the scene setup. To provide the diffusion model with explicit visual guidance, we introduce visual identity prompting, which supplies exemplar images as conditioning inputs to guide the generation of the desired scene setup. To this end, we also build a scalable pipeline to curate a visual identity pool from large robotics datasets. Using our augmented manipulation data to train downstream vision-language-action and visuomotor policy models yields consistent performance gains in both simulation and real-robot settings.
  </details>

- **[Plenoptic Video Generation](https://arxiv.org/abs/2601.05239)**  `arXiv:2601.05239`  `cs.CV`  
  _Xiao Fu, Shitao Tang, Min Shi, Xian Liu, Jinwei Gu, Ming-Yu Liu, et al._
  <details open><summary>Abstract</summary>
  Camera-controlled generative video re-rendering methods, such as ReCamMaster, have achieved remarkable progress. However, despite their success in single-view setting, these works often struggle to maintain consistency across multi-view scenarios. Ensuring spatio-temporal coherence in hallucinated regions remains challenging due to the inherent stochasticity of generative models. To address it, we introduce PlenopticDreamer, a framework that synchronizes generative hallucinations to maintain spatio-temporal memory. The core idea is to train a multi-in-single-out video-conditioned model in an autoregressive manner, aided by a camera-guided video retrieval strategy that adaptively selects salient videos from previous generations as conditional inputs. In addition, Our training incorporates progressive context-scaling to improve convergence, self-conditioning to enhance robustness against long-range visual degradation caused by error accumulation, and a long-video conditioning mechanism to support extended video generation. Extensive experiments on the Basic and Agibot benchmarks demonstrate that PlenopticDreamer achieves state-of-the-art video re-rendering, delivering superior view synchronization, high-fidelity visuals, accurate camera control, and diverse view transformations (e.g., third-person to third-person, and head-view to gripper-view in robotic manipulation). Project page:this https URL
  </details>

- **[PackCache: A Training-Free Acceleration Method for Unified Autoregressive Video Generation via Compact KV-Cache](https://arxiv.org/abs/2601.04359)**  `arXiv:2601.04359`  `cs.CV`  
  _Kunyang Li, Mubarak Shah, Yuzhang Shang_
  <details open><summary>Abstract</summary>
  A unified autoregressive model is a Transformer-based framework that addresses diverse multimodal tasks (e.g., text, image, video) as a single sequence modeling problem under a shared token space. Such models rely on the KV-cache mechanism to reduce attention computation from O(T^2) to O(T); however, KV-cache size grows linearly with the number of generated tokens, and it rapidly becomes the dominant bottleneck limiting inference efficiency and generative length. Unified autoregressive video generation inherits this limitation. Our analysis reveals that KV-cache tokens exhibit distinct spatiotemporal properties: (i) text and conditioning-image tokens act as persistent semantic anchors that consistently receive high attention, and (ii) attention to previous frames naturally decays with temporal distance. Leveraging these observations, we introduce PackCache, a training-free KV-cache management method that dynamically compacts the KV cache through three coordinated mechanisms: condition anchoring that preserves semantic references, cross-frame decay modeling that allocates cache budget according to temporal distance, and spatially preserving position embedding that maintains coherent 3D structure under cache removal. In terms of efficiency, PackCache accelerates end-to-end generation by 1.7-2.2x on 48-frame long sequences, showcasing its strong potential for enabling longer-sequence video generation. Notably, the final four frames - the portion most impacted by the progressively expanding KV-cache and thus the most expensive segment of the clip - PackCache delivers a 2.6x and 3.7x acceleration on A40 and H200, respectively, for 48-frame videos.
  </details>

- **[ReHyAt: Recurrent Hybrid Attention for Video Diffusion Transformers](https://arxiv.org/abs/2601.04342)**  `arXiv:2601.04342`  `cs.CV`  
  _Mohsen Ghafoorian, Amirhossein Habibian_
  <details open><summary>Abstract</summary>
  Recent advances in video diffusion models have shifted towards transformer-based architectures, achieving state-of-the-art video generation but at the cost of quadratic attention complexity, which severely limits scalability for longer sequences. We introduce ReHyAt, a Recurrent Hybrid Attention mechanism that combines the fidelity of softmax attention with the efficiency of linear attention, enabling chunk-wise recurrent reformulation and constant memory usage. Unlike the concurrent linear-only SANA Video, ReHyAt's hybrid design allows efficient distillation from existing softmax-based models, reducing the training cost by two orders of magnitude to ~160 GPU hours, while being competitive in the quality. Our light-weight distillation and finetuning pipeline provides a recipe that can be applied to future state-of-the-art bidirectional softmax-based models. Experiments on VBench and VBench-2.0, as well as a human preference study, demonstrate that ReHyAt achieves state-of-the-art video quality while reducing attention cost from quadratic to linear, unlocking practical scalability for long-duration and on-device video generation. Project page is available atthis https URL.
  </details>

- **[When Models Outthink Their Safety: Unveiling and Mitigating Self-Jailbreak in Large Reasoning Models](https://arxiv.org/abs/2510.21285)**  `arXiv:2510.21285`  `cs.AI` `cs.CL`  
  _Yingzhi Mao, Chunkang Zhang, Junxiang Wang, Xinyan Guan, Boxi Cao, Yaojie Lu, et al._
  <details open><summary>Abstract</summary>
  Large Reasoning Models (LRMs) achieve strong performance on complex multi-step reasoning, yet they still exhibit severe safety failures such as harmful content generation. Existing methods often apply coarse-grained constraints over the entire reasoning trajectories, which can undermine reasoning capability while failing to address the root causes of unsafe behavior. In this work, we uncover a previously underexplored failure mode in LRMs, termed Self-Jailbreak, where models initially recognize the harmful intent of a query, but override this judgment during subsequent reasoning steps, ultimately generating unsafe outputs. Such a phenomenon reveals that LRMs are capable of recognizing harm, while safety failures primarily arise from reasoning steps. Motivated by this finding, we propose \emph{Chain-of-Guardrail} (CoG), a trajectory-level training framework that mitigates Self-Jailbreak via targeted, step-level interventions while maintaining reasoning ability. Experiments across multiple safety and reasoning benchmarks indicate that CoG achieves a favorable balance between safety and reasoning performance compared with existing approaches.
  </details>
