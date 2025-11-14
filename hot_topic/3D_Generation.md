# 🔍 3D_Generation Papers · 2025-11-13

[![Total Papers](https://img.shields.io/badge/Papers-3-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `Video Generation` `Scene Generation` `Content Generation`  
**Filter**: `2D`

---

## 📚 Paper List

- **[Text-to-Scene with Large Reasoning Models](https://arxiv.org/abs/2509.26091)**  `arXiv:2509.26091`  `cs.CV` `cs.LG`  
  _Frédéric Berdoz, Luca A. Lanzendörfer, Nick Tuninga, Roger Wattenhofer_
  <details open><summary>Abstract</summary>
  Prompt-driven scene synthesis allows users to generate complete 3D environments from textual descriptions. Current text-to-scene methods often struggle with complex geometries and object transformations, and tend to show weak adherence to complex instructions. We address these limitations by introducing Reason-3D, a text-to-scene model powered by large reasoning models (LRMs). Reason-3D integrates object retrieval using captions covering physical, functional, and contextual attributes. Reason-3D then places the selected objects based on implicit and explicit layout constraints, and refines their positions with collision-aware spatial reasoning. Evaluated on instructions ranging from simple to complex indoor configurations, Reason-3D significantly outperforms previous methods in human-rated visual fidelity, adherence to constraints, and asset retrieval quality. Beyond its contribution to the field of text-to-scene generation, our work showcases the advanced spatial reasoning abilities of modern LRMs. Additionally, we release the codebase to further the research in object retrieval and placement with LRMs.
  </details>

- **[PAN: A World Model for General, Interactable, and Long-Horizon World Simulation](https://arxiv.org/abs/2511.09057)**  `arXiv:2511.09057`  `cs.CV` `cs.AI` `cs.CL` `cs.LG`  
  _PAN Team Institute of Foundation Models, Jiannan Xiang, Yi Gu, Zihan Liu, Zeyu Feng, Qiyue Gao, et al._
  <details open><summary>Abstract</summary>
  A world model enables an intelligent agent to imagine, predict, and reason about how the world evolves in response to its actions, and accordingly to plan and strategize. While recent video generation models produce realistic visual sequences, they typically operate in the prompt-to-full-video manner without causal control, interactivity, or long-horizon consistency required for purposeful reasoning. Existing world modeling efforts, on the other hand, often focus on restricted domains (e.g., physical, game, or 3D-scene dynamics) with limited depth and controllability, and struggle to generalize across diverse environments and interaction formats. In this work, we introduce PAN, a general, interactable, and long-horizon world model that predicts future world states through high-quality video simulation conditioned on history and natural language actions. PAN employs the Generative Latent Prediction (GLP) architecture that combines an autoregressive latent dynamics backbone based on a large language model (LLM), which grounds simulation in extensive text-based knowledge and enables conditioning on language-specified actions, with a video diffusion decoder that reconstructs perceptually detailed and temporally coherent visual observations, to achieve a unification between latent space reasoning (imagination) and realizable world dynamics (reality). Trained on large-scale video-action pairs spanning diverse domains, PAN supports open-domain, action-conditioned simulation with coherent, long-term dynamics. Extensive experiments show that PAN achieves strong performance in action-conditioned world simulation, long-horizon forecasting, and simulative reasoning compared to other video generators and world models, taking a step towards general world models that enable predictive simulation of future world states for reasoning and acting.
  </details>

- **[Regular Games -- an Automata-Based General Game Playing Language](https://arxiv.org/abs/2511.10593)**  `arXiv:2511.10593`  `cs.AI`  
  _Radosław Miernik, Marek Szykuła, Jakub Kowalski, Jakub Cieśluk, Łukasz Galas, Wojciech Pawlik_
  <details open><summary>Abstract</summary>
  We propose a new General Game Playing (GGP) system called Regular Games (RG). The main goal of RG is to be both computationally efficient and convenient for game design. The system consists of several languages. The core component is a low-level language that defines the rules by a finite automaton. It is minimal with only a few mechanisms, which makes it easy for automatic processing (by agents, analysis, optimization, etc.). The language is universal for the class of all finite turn-based games with imperfect information. Higher-level languages are introduced for game design (by humans or Procedural Content Generation), which are eventually translated to a low-level language. RG generates faster forward models than the current state of the art, beating other GGP systems (Regular Boardgames, Ludii) in terms of efficiency. Additionally, RG's ecosystem includes an editor with LSP, automaton visualization, benchmarking tools, and a debugger of game description transformations.
  </details>
