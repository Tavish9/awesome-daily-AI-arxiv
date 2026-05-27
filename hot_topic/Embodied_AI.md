# 🔍 Embodied_AI Papers · 2026-05-26

[![Total Papers](https://img.shields.io/badge/Papers-4-2688EB)]()
[![Last Updated](https://img.shields.io/badge/dynamic/json?url=https://api.github.com/repos/tavish9/awesome-daily-AI-arxiv/commits/main&query=%24.commit.author.date&label=updated&color=orange)]()

---

## 📌 Filter by Category
**Keywords**: `VLA` `Vision-Language-Action`  
**Filter**: `None`

---

## 📚 Paper List

- **[FineVLA: Fine-Grained Instruction Alignment for Steerable Vision-Language-Action Policies](https://arxiv.org/abs/2605.27284)**  `arXiv:2605.27284`  `cs.RO` `cs.AI`  
  _Xintong Hu, Xuhong Huang, Jinyu Zhang, Yutong Yao, Yuchong Sun, Qiuyue Wang, et al._
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models are increasingly expected to not only complete robot tasks, but also follow human instructions about how those tasks should be executed. However, existing robot datasets usually pair trajectories with coarse goal-level language, leaving execution-critical details such as active arm, approach direction, and contact region unspecified. This limits steerable policy learning and robotic video understanding. We introduce FineVLA, an open framework for action-aligned fine-grained VLA supervision. The framework includes: (1) a data construction tool that unifies 972,247 trajectories across 85K tasks from 10 open-source robot datasets and builds FineVLA-Data, a human-verified dataset of 47,159 fine-grained trajectories; (2) a held-out benchmark with 500 videos, 10,816 atomic facts, and 1,030 VQA questions; (3) a robotics-specialized VLM annotator for scalable fine-grained annotation; and (4) a steerable VLA policy trained with controlled mixtures of fine-grained and raw goal-level instructions. Our experiments yield three findings. First, fine-grained supervision does not sacrifice goal-level success: FG-only improves over Raw-only by +1.4 to +8.1 success-rate points across settings. Second, fine-grained and raw instructions are complementary, following a consistent inverted-U trend peaking at FG:Raw = 1:2 to 1:1. The best mixed setting reaches 86.8%/82.5% in RoboTwin simulation and 62.7/100 in real-world dual-arm manipulation (vs. 49.9 Raw-only). Third, fine-grained supervision improves steerable control: the largest real-world gains appear on pose (+23), color (+18), and approach direction (+18)--factors where goal-level instructions provide no guidance. Overall, fine-grained language should augment goal-level instructions: specifying how to execute alongside what to achieve. Project page:this https URL
  </details>

- **[RoboMME: Benchmarking and Understanding Memory for Robotic Generalist Policies](https://arxiv.org/abs/2603.04639)**  `arXiv:2603.04639`  `cs.RO` `cs.AI`  
  _Yinpei Dai, Hongze Fu, Jayjun Lee, Yuejiang Liu, Haoran Zhang, Jianing Yang, et al._
  <details open><summary>Abstract</summary>
  Memory is critical for long-horizon and history-dependent robotic manipulation. Such tasks often involve counting repeated actions or manipulating objects that become temporarily occluded. Recent vision-language-action (VLA) models have begun to incorporate memory mechanisms; however, their evaluations remain confined to narrow, non-standardized settings. This limits systematic understanding, comparison, and progress measurement. To address these challenges, we introduce RoboMME: a large-scale standardized benchmark for evaluating and advancing VLA models in long-horizon, history-dependent scenarios. Our benchmark comprises 16 manipulation tasks constructed under a carefully designed taxonomy that evaluates temporal, spatial, object, and procedural memory. We further develop a suite of 14 memory-augmented VLA variants built on the {\pi}0.5 backbone to systematically explore different memory representations across multiple integration strategies. Experimental results show that the effectiveness of memory representations is highly task-dependent, with each design offering distinct advantages and limitations across different tasks. Videos and code can be found at our websitethis https URL.
  </details>

- **[Can VLA Models Learn from Real-World Data Continually without Forgetting?](https://arxiv.org/abs/2605.26820)**  `arXiv:2605.26820`  `cs.RO`  
  _Jiarun Zhu, Yijun Hong, Xiaoquan Sun, Zetian Xu, Mingqi Yuan, Zhiyong Wang, et al._
  <details open><summary>Abstract</summary>
  Vision-language-action (VLA) models provide a promising foundation for general-purpose robotics. However, their successful deployment in real-world scenarios requires the ability to continually acquire new skills while retaining previously learned behaviors. While pioneering research has studied the continual learning of VLA models in narrowly simulated environments, this challenge remains largely unexplored under realistic conditions. To address this limitation, we construct a real-world continual learning dataset comprising four sequential manipulation tasks, spanning rigid-object pick-and-place, contact-rich pressing, and deformable-object folding. Using this dataset, we conduct comprehensive experiments and find that VLA models suffer significant catastrophic forgetting when continually learning from heterogeneous real-world demonstrations. We then systematically evaluate experience replay and uncover key implementation factors that govern its success. In summary, this work provides the first empirical study of real-world continual VLA learning and offers practical guidance for deploying long-lived robot policies.
  </details>

- **[Bridging the Semantic-Action Gap in Visual Token Pruning for Efficient VLA Inference](https://arxiv.org/abs/2511.16449)**  `arXiv:2511.16449`  `cs.CV` `cs.AI`  
  _Ziyan Liu, Yeqiu Chen, Hongyi Cai, Tao Lin, Shuo Yang, Zheng Liu, et al._
  <details open><summary>Abstract</summary>
  Vision-Language-Action (VLA) models have shown great potential for embodied AI by integrating visual perception, language understanding, and action execution. In real-time deployment, these models must process continuous visual streams, incurring substantial computational overhead. Visual token pruning -- a mainstream technique for accelerating Vision-Language Models (VLMs) by retaining salient tokens while discarding redundant ones -- offers a natural candidate solution to this challenge. However, directly applying VLM-oriented pruning methods to VLA inference can cause severe degradation in manipulation performance. Our analysis attributes this degradation to a key mismatch: VLA inference exhibits distinct attention patterns between the vision-language prefill stage and the action-decode stage, so pruning based only on context-prefill semantic salience is biased toward semantic cues and may remove action-critical visual tokens. Motivated by this observation, we propose VLA-Pruner, an effective plug-and-play token pruning method grounded in the visual requirements of VLA inference, further exploiting the temporal continuity of robot manipulation. Specifically, VLA-Pruner estimates visual-token importance from both semantic prefilling and temporally smoothed action relevance, and then applies a Combine-then-Filter strategy to retain compact, non-redundant tokens under the compute budget. Experiments show that VLA-Pruner outperforms state-of-the-art approaches across multiple VLA architectures, achieving up to 1.99x speedup with comparable manipulation quality.
  </details>
