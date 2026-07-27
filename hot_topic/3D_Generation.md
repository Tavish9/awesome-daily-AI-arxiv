# 🔍 3D_Generation Papers · 2026-07-26

[![Total Papers](https://img.shields.io/badge/Papers-5-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[AgentHOI: Multi-Agent Reasoning for Human-Object-Interaction Video Generation via Implicit Representation Alignment](https://arxiv.org/abs/2607.22241)**  `arXiv:2607.22241`  `cs.CV`  
  _Ziyao Huang, Shunkai Li, Juan Cao, Chenyu Li, Youliang Zhang, Zixiang Zhou, et al._
  <details open><summary>Abstract</summary>
  Recent advances in video diffusion models have spurred interest in human-object interaction (HOI) video generation, which demands fine-grained control over interaction logic beyond single-subject animation. However, existing HOI methods rely heavily on explicit motion control, limiting scalability and generalization across diverse objects and interactions. In this study, we propose AgentHOI, a text-driven HOI video generation following a thinking-before-generation framework that bridges the gap between high-level textual intent and physical execution through multi-agent reasoning over perception, interaction, and motion planning. Building upon the generated interaction plans, we further strengthen text-driven motion understanding. We introduce an implicit text-motion alignment strategy that distills text-to-motion priors into the video diffusion model, enabling robust HOI synthesis without explicit motion inputs at inference. Experiments show that AgentHOI significantly improves interaction naturalness, object appearance preservation, and adherence to complex textual instructions across challenging object-centric scenarios such as wearing and riding. The code is available atthis https URL.
  </details>

- **[Closing the Loop: Training-Free Revisit Consistency for Autoregressive Generative Rendering](https://arxiv.org/abs/2607.21848)**  `arXiv:2607.21848`  `cs.CV`  
  _Wenchao Ma, Changran Liu, Sharon X. Huang, Haomiao Jiang_
  <details open><summary>Abstract</summary>
  Recent conditional video generation models have shown promising potentials to transform 3D engine renderings, such as depth maps and untextured geometry, into photorealistic videos for gaming and immersive content creation. These applications require long-horizon auto-regressive generation that continuously synthesizes new frames while preserving a persistent 3D world. Auto-regressive generators synthesize video chunk by chunk with a bounded KV cache, so when the camera revisits a location after its context has been evicted, the model often regenerates inconsistent appearance, even though the conditioning renderings (e.g., depth) remain perfectly aligned with the underlyingthis http URLaddress this revisit inconsistency without any post-training by exploiting correspondences the 3D engine already provides: temporal correspondence retrieves pose-matched historical latent chunks into the KV cache as loop-closure memory, while spatial correspondence from camera pose and depth reprojection biases token-level attention toward geometrically corresponding regions of the retrieved chunks. We demonstrate our method on loop-closure trajectories mined from TartanAir and TartanGround dataset to mirror complicate real-world application scenarios, where it outperforms existing training-free baselines on revisit consistency without losing overall video quality. Project Page:this https URL
  </details>

- **[Self Gradient Forcing: Native Long Video Extrapolation](https://arxiv.org/abs/2607.20368)**  `arXiv:2607.20368`  `cs.CV`  
  _Junhao Zhuang, Shiyi Zhang, Yuxuan Bian, Yaowei Li, Yawen Luo, Yijun Liu, et al._
  <details open><summary>Abstract</summary>
  Recent autoregressive video diffusion methods are increasingly built upon Self Forcing, where the student is trained on histories produced by its own rollout rather than ground-truth video contexts. This reduces exposure bias, but the historical key-value cache is still used by future frames only as frozen rollout state. As a result, future losses cannot supervise how earlier generated latents should be written into more useful keys and values for later video-latent generation. We call this the historical context-gradient gap. We propose Self Gradient Forcing (SGF), a two-pass training strategy that restores this missing supervision signal without backpropagating through the full serial rollout. Pass 1 performs a no-gradient autoregressive rollout matching inference and, at a sampled denoising exit step, records both the self-generated context and the noisy latents fed to the model. Pass 2 performs parallel context-gradient reconstruction for the recorded exit step. The generated context is used as stop-gradient clean-latent input, while the model recomputes the context KV representations and future-to-context causal attention. Thus, SGF provides the missing memory-writing supervision within the native autoregressive training objective, using losses on future video latents to train the model to encode context into more effective causal memory. Across extensive long-horizon frame-wise and chunk-wise experiments under different initializations, SGF achieves stronger native long-video extrapolation than Self Forcing, especially in subject identity, background/layout consistency, and temporal stability. Remarkably, using only a 5-second training window, SGF can extrapolate to videos lasting several minutes. Code and models will be released to advance research on autoregressive video generation.
  </details>

- **[Delving into Latent Spectral Biasing of Video VAEs for Superior Diffusability](https://arxiv.org/abs/2512.05394)**  `arXiv:2512.05394`  `cs.CV`  
  _Shizhan Liu, Xinran Deng, Zhuoyi Yang, Jiayan Teng, Xiaotao Gu, Jie Tang_
  <details open><summary>Abstract</summary>
  Latent diffusion models pair VAEs with diffusion backbones, and the structure of VAE latents strongly influences the difficulty of diffusion training. However, existing video VAEs typically focus on reconstruction fidelity, overlooking latent structure. We present a statistical analysis of video VAE latent spaces and identify two spectral properties essential for diffusion training: a spatio-temporal frequency spectrum biased toward low frequencies, and a channel-wise eigenspectrum dominated by a few modes. To induce these properties, we propose two lightweight, backbone-agnostic regularizers: Local Correlation Regularization and Latent Masked Reconstruction. Experiments show that our Spectral-Structured VAE (SSVAE) achieves a $3\times$ speedup in text-to-video generation convergence and a 10\% gain in video reward, outperforming strong open-source VAEs. The code is available atthis https URL.
  </details>

- **[HunyuanVideo-HOMA: Generic Human-Object Interaction in Multimodal Driven Human Animation](https://arxiv.org/abs/2506.08797)**  `arXiv:2506.08797`  `cs.CV`  
  _Ziyao Huang, Zixiang Zhou, Juan Cao, Yifeng Ma, Yi Chen, Zejing Rao, et al._
  <details open><summary>Abstract</summary>
  To address key limitations in human-object interaction (HOI) video generation -- specifically the reliance on curated motion data, limited generalization to novel objects/scenarios, and restricted accessibility -- we introduce HunyuanVideo-HOMA, a weakly conditioned multimodal-driven framework. HunyuanVideo-HOMA enhances controllability and reduces dependency on precise inputs through sparse, decoupled motion guidance. It encodes appearance and motion signals into the dual input space of a multimodal diffusion transformer (MMDiT), fusing them within a shared context space to synthesize temporally consistent and physically plausible interactions. To optimize training, we integrate a parameter-space HOI adapter initialized from pretrained MMDiT weights, preserving prior knowledge while enabling efficient adaptation, and a facial cross-attention adapter for anatomically accurate audio-driven lip synchronization. Extensive experiments confirm state-of-the-art performance in interaction naturalness and generalization under weak supervision. Finally, HunyuanVideo-HOMA demonstrates versatility in text-conditioned generation and interactive object manipulation, supported by a user-friendly demo interface. The project page is atthis https URL.
  </details>
