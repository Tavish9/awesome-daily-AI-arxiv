# 🔍 3D_Generation Papers · 2025-10-20

[![Total Papers](https://img.shields.io/badge/Papers-5-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[MUG-V 10B: High-efficiency Training Pipeline for Large Video Generation Models](https://arxiv.org/abs/2510.17519)**  `arXiv:2510.17519`  `cs.CV` `cs.AI`  
  _Yongshun Zhang, Zhongyi Fan, Yonghang Zhang, Zhangzikang Li, Weifeng Chen, Zhongwei Feng, et al._
  <details open><summary>Abstract</summary>
  In recent years, large-scale generative models for visual content (\textit{e.g.,} images, videos, and 3D objects/scenes) have made remarkable progress. However, training large-scale video generation models remains particularly challenging and resource-intensive due to cross-modal text-video alignment, the long sequences involved, and the complex spatiotemporal dependencies. To address these challenges, we present a training framework that optimizes four pillars: (i) data processing, (ii) model architecture, (iii) training strategy, and (iv) infrastructure for large-scale video generation models. These optimizations delivered significant efficiency gains and performance improvements across all stages of data preprocessing, video compression, parameter scaling, curriculum-based pretraining, and alignment-focused post-training. Our resulting model, MUG-V 10B, matches recent state-of-the-art video generators overall and, on e-commerce-oriented video generation tasks, surpasses leading open-source baselines in human evaluations. More importantly, we open-source the complete stack, including model weights, Megatron-Core-based large-scale training code, and inference pipelines for video generation and enhancement. To our knowledge, this is the first public release of large-scale video generation training code that exploits Megatron-Core to achieve high training efficiency and near-linear multi-node scaling, details are available in \href{this https URL}{our webpage}.
  </details>

- **[Morpheus: Benchmarking Physical Reasoning of Video Generative Models with Real Physical Experiments](https://arxiv.org/abs/2504.02918)**  `arXiv:2504.02918`  `cs.CV`  
  _Chenyu Zhang, Daniil Cherniavskii, Antonios Tragoudaras, Antonios Vozikis, Thijmen Nijdam, Derck W. E. Prinzhorn, et al._
  <details open><summary>Abstract</summary>
  Recent advances in image and video generation raise hopes that these models possess world modeling capabilities, the ability to generate realistic, physically plausible videos. This could revolutionize applications in robotics, autonomous driving, and scientific simulation. However, before treating these models as world models, we must ask: Do they adhere to physical conservation laws? To answer this, we introduce Morpheus, a benchmark for evaluating video generation models on physical reasoning. It features 80 real-world videos capturing physical phenomena, guided by conservation laws. Since artificial generations lack ground truth, we assess physical plausibility using physics-informed metrics evaluated with respect to infallible conservation laws known per physical setting, leveraging advances in physics-informed neural networks and vision-language foundation models. Our findings reveal that even with advanced prompting and video conditioning, current models struggle to encode physical principles despite generating aesthetically pleasing videos. All data, leaderboard, and code are open-sourced at our project page.
  </details>

- **[Efficient Long-duration Talking Video Synthesis with Linear Diffusion Transformer under Multimodal Guidance](https://arxiv.org/abs/2411.16748)**  `arXiv:2411.16748`  `cs.CV`  
  _Haojie Zhang, Zhihao Liang, Ruibo Fu, Bingyan Liu, Zhengqi Wen, Xuefei Liu, et al._
  <details open><summary>Abstract</summary>
  Long-duration talking video synthesis faces enduring challenges in achieving high video quality, portrait and temporal consistency, and computational efficiency. As video length increases, issues such as visual degradation, identity inconsistency, temporal incoherence, and error accumulation become increasingly problematic, severely affecting the realism and reliability of the results. To address these challenges, we present LetsTalk, a diffusion transformer framework equipped with multimodal guidance and a novel memory bank mechanism, explicitly maintaining contextual continuity and enabling robust, high-quality, and efficient generation of long-duration talking videos. In particular, LetsTalk introduces a noise-regularized memory bank to alleviate error accumulation and sampling artifacts during extended video generation. To further improve efficiency and spatiotemporal consistency, LetsTalk employs a deep compression autoencoder and a spatiotemporal-aware transformer with linear attention for effective multimodal fusion. We systematically analyze three fusion schemes and show that combining deep (Symbiotic Fusion) for portrait features and shallow (Direct Fusion) for audio achieves superior visual realism and precise speech-driven motion, while preserving diversity of movements. Extensive experiments demonstrate that LetsTalk establishes new state-of-the-art in generation quality, producing temporally coherent and realistic talking videos with enhanced diversity and liveliness, and maintains remarkable efficiency with 8x fewer parameters than previous approaches.
  </details>

- **[From Preferences to Prejudice: The Role of Alignment Tuning in Shaping Social Bias in Video Diffusion Models](https://arxiv.org/abs/2510.17247)**  `arXiv:2510.17247`  `cs.CL` `cs.CV`  
  _Zefan Cai, Haoyi Qiu, Haozhe Zhao, Ke Wan, Jiachen Li, Jiuxiang Gu, et al._
  <details open><summary>Abstract</summary>
  Recent advances in video diffusion models have significantly enhanced text-to-video generation, particularly through alignment tuning using reward models trained on human preferences. While these methods improve visual quality, they can unintentionally encode and amplify social biases. To systematically trace how such biases evolve throughout the alignment pipeline, we introduce VideoBiasEval, a comprehensive diagnostic framework for evaluating social representation in video generation. Grounded in established social bias taxonomies, VideoBiasEval employs an event-based prompting strategy to disentangle semantic content (actions and contexts) from actor attributes (gender and ethnicity). It further introduces multi-granular metrics to evaluate (1) overall ethnicity bias, (2) gender bias conditioned on ethnicity, (3) distributional shifts in social attributes across model variants, and (4) the temporal persistence of bias within videos. Using this framework, we conduct the first end-to-end analysis connecting biases in human preference datasets, their amplification in reward models, and their propagation through alignment-tuned video diffusion models. Our results reveal that alignment tuning not only strengthens representational biases but also makes them temporally stable, producing smoother yet more stereotyped portrayals. These findings highlight the need for bias-aware evaluation and mitigation throughout the alignment process to ensure fair and socially responsible video generation.
  </details>

- **[A Markovian Framing of WaveFunctionCollapse for Procedurally Generating Aesthetically Complex Environments](https://arxiv.org/abs/2509.09919)**  `arXiv:2509.09919`  `cs.AI`  
  _Franklin Yiu, Mohan Lu, Nina Li, Kevin Joseph, Tianxu Zhang, Julian Togelius, et al._
  <details open><summary>Abstract</summary>
  Procedural content generation often requires satisfying both designer-specified objectives and adjacency constraints implicitly imposed by the underlying tile set. To address the challenges of jointly optimizing both constraints and objectives, we reformulate WaveFunctionCollapse (WFC) as a Markov Decision Process (MDP), enabling external optimization algorithms to focus exclusively on objective maximization while leveraging WFC's propagation mechanism to enforce constraint satisfaction. We empirically compare optimizing this MDP to traditional evolutionary approaches that jointly optimize global metrics and local tile placement. Across multiple domains with various difficulties, we find that joint optimization not only struggles as task complexity increases, but consistently underperforms relative to optimization over the WFC-MDP, underscoring the advantages of decoupling local constraint satisfaction from global objective optimization.
  </details>
