# 🔍 3D_Generation Papers · 2026-09-02

[![Total Papers](https://img.shields.io/badge/Papers-2-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[ContextAnyone: Context-Aware Diffusion for Character-Consistent Text-to-Video Generation](https://arxiv.org/abs/2512.07328)**  `arXiv:2512.07328`  `cs.CV` `cs.AI`  
  _Ziyang Mai, Yu-Wing Tai_
  <details open><summary>Abstract</summary>
  Text-to-video generation has advanced rapidly, yet preserving a character's holistic appearance from a single reference image remains challenging, particularly when the character undergoes large pose, motion, and scene changes. Existing reference-conditioned approaches primarily treat the reference image as a conditioning signal, which can weaken fine-grained appearance information as reference and noisy video tokens interact during denoising. We propose \textbf{ContextAnyone}, a context-aware diffusion framework that instead treats the reference as an explicitly preserved appearance anchor. Our key idea is to jointly reconstruct the reference image and generate the target video within a shared diffusion transformer, providing direct supervision for preserving identity and fine-grained appearance throughout denoising. To maintain the reference as a stable source of appearance information, we further introduce asymmetric information flow that allows video tokens to selectively access reference tokens while preventing noisy video features from propagating back to the reference branch. We complement this design with Gap-RoPE, which separates the positional representations of the reference and generated video tokens. Experiments on a benchmark constructed from OpenVid-HD demonstrate that ContextAnyone improves both identity and fine-grained appearance consistency over existing reference-conditioned baselines while maintaining motion characteristics close to the underlying text-to-video generator.
  </details>

- **[Thinking in Pictures: A Systematic Benchmark for Reasoning-driven Image Generation](https://arxiv.org/abs/2609.02864)**  `arXiv:2609.02864`  `cs.CV`  
  _Yutong Liu, Nan Huang, Xu Cao, James M. Rehg_
  <details open><summary>Abstract</summary>
  Recent advancements in unified generative models (UGMs) and world simulators have achieved unprecedented results in visual perception and synthesis. However, these models primarily rely on surface-level event alignment, leaving the capacity for high-level visual reasoning underexplored. True visual generative intelligence demands "Reasoning-to-Generation", an ability to infer latent rules from visual inputs and manifest solutions through precise, logically constrained visual outcomes. We introduce RIG-BENCH, a novel comprehensive benchmark that systematically evaluates Reasoning-driven Image Generation (RIG) across four cognitively demanding domains: Concept-based, Transformation-based, Pattern & Structure, and Scenario-based. Featuring 2000 curated samples, RIG-BENCH serves as a rigorous stress test for RIG. Our extensive evaluations of state-of-the-art UGMs and image/video generation models reveal a significant reasoning-generation gap, wherein models frequently produce locally plausible but globally illogical outputs. RIG-BENCH provides a vital diagnostic framework to guide the development of next-generation, logically grounded UGMs and world simulators.
  </details>
