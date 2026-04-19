# 🔍 3D_Generation Papers · 2026-04-18

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[AnimationBench: Are Video Models Good at Character-Centric Animation?](https://arxiv.org/abs/2604.15299)**  `arXiv:2604.15299`  `cs.CV`  
  _Leyi Wu, Pengjun Fang, Kai Sun, Yazhou Xing, Yinwei Wu, Songsong Wang, et al._
  <details open><summary>Abstract</summary>
  Video generation has advanced rapidly, with recent methods producing increasingly convincing animated results. However, existing benchmarks-largely designed for realistic videos-struggle to evaluate animation-style generation with its stylized appearance, exaggerated motion, and character-centric consistency. Moreover, they also rely on fixed prompt sets and rigid pipelines, offering limited flexibility for open-domain content and custom evaluation needs. To address this gap, we introduce AnimationBench, the first systematic benchmark for evaluating animation image-to-video generation. AnimationBench operationalizes the Twelve Basic Principles of Animation and IP Preservation into measurable evaluation dimensions, together with Broader Quality Dimensions including semantic consistency, motion rationality, and camera motion consistency. The benchmark supports both a standardized close-set evaluation for reproducible comparison and a flexible open-set evaluation for diagnostic analysis, and leverages visual-language models for scalable assessment. Extensive experiments show that AnimationBench aligns well with human judgment and exposes animation-specific quality differences overlooked by realism-oriented benchmarks, leading to more informative and discriminative evaluation of state-of-the-art I2V models.
  </details>

- **[How to Correctly Make Mistakes: A Framework for Constructing and Benchmarking Mistake Aware Egocentric Procedural Videos](https://arxiv.org/abs/2604.15134)**  `arXiv:2604.15134`  `cs.CV`  
  _Olga Loginova, Frank Keller_
  <details open><summary>Abstract</summary>
  Reliable procedural monitoring in video requires exposure to naturally occurring human errors and the recoveries that follow. In egocentric recordings, mistakes are often partially occluded by hands and revealed through subtle object state changes, while existing procedural datasets provide limited and inconsistent mistake and correction traces. We present PIE-V (Psychologically Inspired Error injection for Videos), a framework for constructing and benchmarking mistake-aware egocentric procedural videos by augmenting clean keystep procedures with controlled, human-plausible deviations. PIE-V combines a psychology-informed error planner conditioned on procedure phase and semantic step load, a correction planner that models recovery behavior, an LLM writer that performs cascade-consistent rewrites, and an LLM judge that validates procedural coherence and repairs failures. For video segment edits, PIE-V synthesizes replacement clips with text-guided video generation and stitches them into the episode to preserve visual plausibility. Applied to 17 tasks and 50 Ego-Exo4D scenarios, PIE-V injects 102 mistakes and generates 27 recovery corrections. For benchmarking, we introduce a unified taxonomy and a human rubric with nine metrics that cover step-level and procedure-level quality, including plausibility, procedure logic with annotator confidence, state change coherence, and grounding between text and video. Using this protocol, we audit several existing resources and compare PIE-V against a freeform LLM generation baseline under the same criteria. Together, the framework and rubric support post-completion verification for egocentric procedural mistake detection and correction.
  </details>

- **[Prompt-to-Gesture: Measuring the Capabilities of Image-to-Video Deictic Gesture Generation](https://arxiv.org/abs/2604.14953)**  `arXiv:2604.14953`  `cs.CV`  
  _Hassan Ali, Doreen Jirak, Luca Müller, Stefan Wermter_
  <details open><summary>Abstract</summary>
  Gesture recognition research, unlike NLP, continues to face acute data scarcity, with progress constrained by the need for costly human recordings or image processing approaches that cannot generate authentic variability in the gestures themselves. Recent advancements in image-to-video foundation models have enabled the generation of photorealistic, semantically rich videos guided by natural language. These capabilities open up new possibilities for creating effort-free synthetic data, raising the critical question of whether video Generative AI models can augment and complement traditional human-generated gesture data. In this paper, we introduce and analyze prompt-based video generation to construct a realistic deictic gestures dataset and rigorously evaluate its effectiveness for downstream tasks. We propose a data generation pipeline that produces deictic gestures from a small number of reference samples collected from human participants, providing an accessible approach that can be leveraged both within and beyond the machine learning community. Our results demonstrate that the synthetic gestures not only align closely with real ones in terms of visual fidelity but also introduce meaningful variability and novelty that enrich the original data, further supported by superior performance of various deep models using a mixed dataset. These findings highlight that image-to-video techniques, even in their early stages, offer a powerful zero-shot approach to gesture synthesis with clear benefits for downstream tasks.
  </details>
