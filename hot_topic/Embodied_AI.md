# 🔍 Embodied_AI Papers · 2025-12-28

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[LIBERO-Plus: In-depth Robustness Analysis of Vision-Language-Action Models](https://arxiv.org/abs/2510.13626)**  `arXiv:2510.13626`  `cs.RO` `cs.CL` `cs.CV`  
  _Senyu Fei, Siyin Wang, Junhao Shi, Zihao Dai, Jikun Cai, Pengfang Qian, et al._
  <details open><summary>Abstract</summary>
  Visual-Language-Action (VLA) models report impressive success rates on robotic manipulation benchmarks, yet these results may mask fundamental weaknesses in robustness. We perform a systematic vulnerability analysis by introducing controlled perturbations across seven dimensions: objects layout, camera viewpoints, robot initial states, language instructions, light conditions, background textures and sensor noise. We comprehensively analyzed multiple state-of-the-art models and revealed consistent brittleness beneath apparent competence. Our analysis exposes critical weaknesses: models exhibit extreme sensitivity to perturbation factors, including camera viewpoints and robot initial states, with performance dropping from 95% to below 30% under modest perturbations. Surprisingly, models are largely insensitive to language variations, with further experiments revealing that models tend to ignore language instructions completely. Our findings challenge the assumption that high benchmark scores equate to true competency and highlight the need for evaluation practices that assess reliability under realistic variation.
  </details>

- **[StereoVLA: Enhancing Vision-Language-Action Models with Stereo Vision](https://arxiv.org/abs/2512.21970)**  `arXiv:2512.21970`  `cs.RO`  
  _Shengliang Deng, Mi Yan, Yixin Zheng, Jiayi Su, Wenhao Zhang, Xiaoguang Zhao, et al._
  <details open><summary>Abstract</summary>
  Stereo cameras closely mimic human binocular vision, providing rich spatial cues critical for precise robotic manipulation. Despite their advantage, the adoption of stereo vision in vision-language-action models (VLAs) remains underexplored. In this work, we present StereoVLA, a VLA model that leverages rich geometric cues from stereo vision. We propose a novel Geometric-Semantic Feature Extraction module that utilizes vision foundation models to extract and fuse two key features: 1) geometric features from subtle stereo-view differences for spatial perception; 2) semantic-rich features from the monocular view for instruction following. Additionally, we propose an auxiliary Interaction-Region Depth Estimation task to further enhance spatial perception and accelerate model convergence. Extensive experiments show that our approach outperforms baselines by a large margin in diverse tasks under the stereo setting and demonstrates strong robustness to camera pose variations.
  </details>

- **[Motus: A Unified Latent Action World Model](https://arxiv.org/abs/2512.13030)**  `arXiv:2512.13030`  `cs.CV` `cs.LG` `cs.RO`  
  _Hongzhe Bi, Hengkai Tan, Shenghao Xie, Zeyuan Wang, Shuhe Huang, Haitian Liu, et al._
  <details open><summary>Abstract</summary>
  While a general embodied agent must function as a unified system, current methods are built on isolated models for understanding, world modeling, and control. This fragmentation prevents unifying multimodal generative capabilities and hinders learning from large-scale, heterogeneous data. In this paper, we propose Motus, a unified latent action world model that leverages existing general pretrained models and rich, sharable motion information. Motus introduces a Mixture-of-Transformer (MoT) architecture to integrate three experts (i.e., understanding, video generation, and action) and adopts a UniDiffuser-style scheduler to enable flexible switching between different modeling modes (i.e., world models, vision-language-action models, inverse dynamics models, video generation models, and video-action joint prediction models). Motus further leverages the optical flow to learn latent actions and adopts a recipe with three-phase training pipeline and six-layer data pyramid, thereby extracting pixel-level "delta action" and enabling large-scale action pretraining. Experiments show that Motus achieves superior performance against state-of-the-art methods in both simulation (a +15% improvement over X-VLA and a +45% improvement over Pi0.5) and real-world scenarios(improved by +11~48%), demonstrating unified modeling of all functionalities and priors significantly benefits downstream robotic tasks.
  </details>
