# Awesome Robot Diffusion [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) <!-- omit in toc -->
A curated list of recent robot learning papers incorporating diffusion models for manipulation, navigation, planning etc.

<!-- <p align="center">
<img src="https://makeavideo.studio/assets/overview.webp" width="240px"/>
<img src="https://makeavideo.studio/assets/A_teddy_bear_painting_a_portrait.webp" width="240px"/>    
</p>

<p align="center">
<img src="https://tuneavideo.github.io/assets/teaser.gif" width="480px"/>  
</p>

<p align="center">
<img src="https://github.com/ChenyangQiQi/FateZero/blob/main/docs/gif_results/17_car_posche_01_concat_result.gif?raw=true" width="240px"/>
<img src="https://github.com/ChenyangQiQi/FateZero/blob/main/docs/gif_results/3_sunflower_vangogh_conat_result.gif?raw=true" width="240px"/>    
</p>

<p align="center">
(Source: <a href="https://makeavideo.studio/">Make-A-Video</a>, <a href="https://tuneavideo.github.io/">Tune-A-Video</a>, and <a href="https://fate-zero-edit.github.io/">Fate/Zero</a>.)
</p> -->

## Table of Contents <!-- omit in toc -->
- [Benchmarks](#benchmarks)
- [Diffusion Policy](#diffusion-policy)
- [Diffusion Generation Models in Robot Learning](#diffusion-generation-models-in-robot-learning)
- [Robot Learning Utilizing Diffusion Model Properties](#robot-learning-utilizing-diffusion-model-properties)


### Benchmarks

+ [Learning Complex Dexterous Manipulation with Deep Reinforcement Learning and Demonstrations](https://arxiv.org/abs/1709.10087) (RSS 2018)
  [![Star](https://img.shields.io/github/stars/aravindr93/hand_dapg.svg?style=social&label=Star)](https://github.com/aravindr93/hand_dapg)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/1709.10087)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/deeprl-dexterous-manipulation)

+ [Meta-World: A Benchmark and Evaluation for Multi-Task and Meta Reinforcement Learning](https://arxiv.org/abs/1910.10897) (CoRL 2020)
  [![Star](https://img.shields.io/github/stars/Farama-Foundation/Metaworld.svg?style=social&label=Star)](https://github.com/Farama-Foundation/Metaworld)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/1910.10897)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://meta-world.github.io/)

+ [Bridge data: Boosting generalization of robotic skills with cross-domain datasets](https://arxiv.org/abs/2109.13396) (RSS 2022)
  [![Star](https://img.shields.io/github/stars/yanlai00/bridge_data_imitation_learning.svg?style=social&label=Star)](https://github.com/yanlai00/bridge_data_imitation_learning)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2109.13396)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/bridgedata)

<!-- + [DexMV: Imitation Learning for Dexterous Manipulation from Human Videos](https://arxiv.org/abs/2108.05877) (ECCV 2022)
  [![Star](https://img.shields.io/github/stars/yzqin/dexmv-sim.svg?style=social&label=Star)](https://github.com/yzqin/dexmv-sim)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2108.05877)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://yzqin.github.io/dexmv/) -->

+ [Towards Human-Level Bimanual Dexterous Manipulation with Reinforcement Learning](https://arxiv.org/pdf/2206.08686) (NeurIPS 2022 Datasets and Benchmarks Track)
  [![Star](https://img.shields.io/github/stars/PKU-MARL/DexterousHands.svg?style=social&label=Star)](https://github.com/PKU-MARL/DexterousHands)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2206.08686)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://pku-marl.github.io/DexterousHands/)

+ [Dexart: Benchmarking generalizable dexterous manipulation with articulated objects](https://arxiv.org/abs/2305.05706) (CVPR 2023)
  [![Star](https://img.shields.io/github/stars/Kami-code/dexart-release.svg?style=social&label=Star)](https://github.com/Kami-code/dexart-release)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.05706)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://www.chenbao.tech/dexart/)

+ [BridgeData V2: A Dataset for Robot Learning at Scale](https://arxiv.org/abs/2305.05706) (CoRL 2023)
  [![Star](https://img.shields.io/github/stars/rail-berkeley/bridge_data_v2.svg?style=social&label=Star)](https://github.com/rail-berkeley/bridge_data_v2)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.12952)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://rail-berkeley.github.io/bridgedata/)

+ [CALVIN: A Benchmark for Language-conditioned Policy Learning for Long-horizon Robot Manipulation Tasks](https://arxiv.org/abs/2112.03227) (RAL 2022)
  [![Star](https://img.shields.io/github/stars/mees/calvin.svg?style=social&label=Star)](https://github.com/mees/calvin)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2112.03227)
  [![Website](https://img.shields.io/badge/Website-9cf)](http://calvin.cs.uni-freiburg.de/)

+ [RLBench: The Robot Learning Benchmark & Learning Environment](https://arxiv.org/abs/1909.12271) (RAL 2020)
  [![Star](https://img.shields.io/github/stars/stepjam/RLBench.svg?style=social&label=Star)](https://github.com/stepjam/RLBench)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/1909.12271)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/rlbench/home)

+ [LIBERO: Benchmarking Knowledge Transfer in Lifelong Robot Learning](https://arxiv.org/abs/2306.03310) (NeurIPS 2023 Dataset and Benchmark Track)
  [![Star](https://img.shields.io/github/stars/Lifelong-Robot-Learning/LIBERO.svg?style=social&label=Star)](https://github.com/Lifelong-Robot-Learning/LIBERO)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.03310)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://libero-project.github.io/intro.html)


MuJoCo Manipulus


Visual Pusher

Panda Arm

<!-- Dexdeform: Dexterous deformable object manipulation with human demonstrations and differentiable physics (To be checked) -->

Concealed Backdoor Attack on Diffusion Models for Smart Devices with Non-standard Gaussian Distribution Noise


### Diffusion Policy
#### Manipulation
+ [Imitating Human Behaviour with Diffusion Models](https://arxiv.org/abs/2301.10677) (ICLR 2023)
  [![Star](https://img.shields.io/github/stars/microsoft/Imitating-Human-Behaviour-w-Diffusion.svg?style=social&label=Star)](https://github.com/microsoft/Imitating-Human-Behaviour-w-Diffusion)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2301.10677)
  <!-- [![Website](https://img.shields.io/badge/Website-9cf)](https://pypi.org/project/fvmd/1.0.0/) -->

+ [Diffusion policy: Visuomotor policy learning via action diffusion](https://arxiv.org/abs/2303.04137) (RSS 2023)
  [![Star](https://img.shields.io/github/stars/real-stanford/diffusion_policy.svg?style=social&label=Star)](https://github.com/real-stanford/diffusion_policy)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.04137)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://diffusion-policy.cs.columbia.edu/)

+ [Goal-conditioned imitation learning using score-based diffusion policies](https://arxiv.org/abs/2304.02532) (RSS 2023)
  [![Star](https://img.shields.io/github/stars/intuitive-robots/beso.svg?style=social&label=Star)](https://github.com/intuitive-robots/beso)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.02532)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://intuitive-robots.github.io/beso-website/)

+ [Scaling Up and Distilling Down: Language-Guided Robot Skill Acquisition](https://www.sciencedirect.com/science/article/abs/pii/S0950705124008244) (CoRL 2023)
  [![Star](https://img.shields.io/github/stars/real-stanford/scalingup.svg?style=social&label=Star)](https://github.com/real-stanford/scalingup)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://www.cs.columbia.edu/~huy/scalingup/)

+ [ChainedDiffuser: Unifying Trajectory Diffusion and Keypose Prediction for Robotic Manipulation](https://openreview.net/forum?id=W0zgY2mBTA8) (CoRL 2023)
  [![Star](https://img.shields.io/github/stars/zhouxian/act3d-chained-diffuser.svg?style=social&label=Star)](https://github.com/zhouxian/act3d-chained-diffuser)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://chained-diffuser.github.io/)

+ [Generative Skill Chaining: Long-Horizon Skill Planning with Diffusion Models](https://arxiv.org/pdf/2401.03360) (CoRL 2023)
  [![Star](https://img.shields.io/github/stars/generative-skill-chaining/gsc-code.svg?style=social&label=Star)](https://github.com/generative-skill-chaining/gsc-code)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2401.03360)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://generative-skill-chaining.github.io/)

+ [PlayFusion: Skill Acquisition via Diffusion from Language-Annotated Play](https://arxiv.org/pdf/2312.04549) (CoRL 2023)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2312.04549)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://play-fusion.github.io/)

+ [Memory-Consistent Neural Networks for Imitation Learning](https://arxiv.org/abs/2310.06171) (ICLR 2024)
  [![Star](https://img.shields.io/github/stars/kaustubhsridhar/MCNN.svg?style=social&label=Star)](https://github.com/kaustubhsridhar/MCNN)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.06171)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/mcnn-imitation)

+ [EDMP: Ensemble-of-costs-guided Diffusion for Motion Planning](https://arxiv.org/abs/2309.11414) (ICRA 2024)
  [![Star](https://img.shields.io/github/stars/vishal-2000/EDMP.svg?style=social&label=Star)](https://github.com/vishal-2000/EDMP)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.11414)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://ensemble-of-costs-diffusion.github.io/)

+ [Diffskill: Improving Reinforcement Learning Through Diffusion-Based Skill Denoiser for Robotic Manipulation](https://www.sciencedirect.com/science/article/abs/pii/S0950705124008244) (Knowledge-Based Systems 2024)

+ [Consistency policy: Accelerated visuomotor policies via consistency distillation](https://arxiv.org/abs/2405.07503) (RSS 2024)
  [![Star](https://img.shields.io/github/stars/Aaditya-Prasad/Consistency-Policy.svg?style=social&label=Star)](https://github.com/Aaditya-Prasad/Consistency-Policy/)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.07503)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://consistency-policy.github.io/)

ManiCM: Real-time 3D Diffusion Policy via Consistency Model for Robotic Manipulation (3D, consistency model, efficiency)

+ [Track2Act: Predicting Point Tracks from Internet Videos enables Generalizable Robot Manipulation](https://arxiv.org/abs/2405.01527) (ECCV 2024)
  [![Star](https://img.shields.io/github/stars/homangab/Track-2-Act.svg?style=social&label=Star)](https://github.com/homangab/Track-2-Act/)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.01527)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://homangab.github.io/track2act/)

+ [Differentiable Robot Rendering](https://arxiv.org/abs/2410.13851) (CoRL 2024)
  [![Star](https://img.shields.io/github/stars/cvlab-columbia/drrobot.svg?style=social&label=Star)](https://github.com/cvlab-columbia/drrobot)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.13851)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://drrobot.cs.columbia.edu/)

+ [Sparse Diffusion Policy: A Sparse, Reusable, and Flexible Policy for Robot Learning](https://arxiv.org/abs/2407.01531) (CoRL 2024)
  [![Star](https://img.shields.io/github/stars/AnthonyHuo/SDP.svg?style=social&label=Star)](https://github.com/AnthonyHuo/SDP)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.01531)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://forrest-110.github.io/sparse_diffusion_policy/)

+ [3D Diffuser Actor: Policy Diffusion with 3D Scene Representations](https://arxiv.org/abs/2402.10885) (CoRL 2024)
  [![Star](https://img.shields.io/github/stars/nickgkan/3d_diffuser_actor.svg?style=social&label=Star)](https://github.com/nickgkan/3d_diffuser_actor)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.10885)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://3d-diffuser-actor.github.io/)

+ [3D Diffusion Policy: Generalizable Visuomotor Policy Learning via Simple 3D Representations](https://arxiv.org/abs/2403.03954) (RSS 2024)
  [![Star](https://img.shields.io/github/stars/YanjieZe/3D-Diffusion-Policy.svg?style=social&label=Star)](https://github.com/YanjieZe/3D-Diffusion-Policy)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.03954)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://3d-diffusion-policy.github.io/)

+ [RISE: 3D Perception Makes Real-World Robot Imitation Simple and Effective](https://arxiv.org/abs/2404.12281) (IROS 2024)
  [![Star](https://img.shields.io/github/stars/rise-policy/rise.svg?style=social&label=Star)](https://github.com/rise-policy/rise)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.12281)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://rise-policy.github.io/)

+ [Vision-Language-Affordance-based Robot Manipulation with Flow Matching](https://arxiv.org/abs/2409.01083) (Sep 2024)
  [![Star](https://img.shields.io/github/stars/HRI-EU/flow-matching-policy.svg?style=social&label=Star)](https://github.com/HRI-EU/flow-matching-policy)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2409.01083)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://hri-eu.github.io/flow-matching-policy/)

Flow Matching Imitation Learning for Multi-Support Manipulation (Flow matching)

FlowPolicy: Enabling Fast and Robust 3D Flow-based Policy via Consistency Flow Matching for Robot Manipulation

ACTIONFLOW: Equivariant, Accurate, and Efficient Policies with Spatially Symmetric Flow Matching

Fast and Robust Visuomotor Riemannian Flow Matching Policy

+ [Diffusion-VLA: Scaling Robot Foundation Models via Unified Diffusion and Autoregression](https://arxiv.org/pdf/2412.03293) (Dec 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2412.03293)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://diffusion-vla.github.io/)

Vision-Language-Action Model and Diffusion Policy Switching Enables Dexterous Control of an Anthropomorphic Hand (Combining openVLA and diffusion policy)

TinyVLA: Towards Fast, Data-Efficient Vision-Language-Action Models for Robotic Manipulation

+ [RDT-1B: a Diffusion Foundation Model for Bimanual Manipulation](https://arxiv.org/abs/2410.07864) (Dec 2024) (uses diffusion transformer)
  [![Star](https://img.shields.io/github/stars/thu-ml/RoboticsDiffusionTransformer.svg?style=social&label=Star)](https://github.com/thu-ml/RoboticsDiffusionTransformer)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.07864)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://rdt-robotics.github.io/rdt-robotics/)

+ [XSkill: Cross Embodiment Skill Discovery](https://arxiv.org/abs/2307.09955) (CoRL 2023)
  [![Star](https://img.shields.io/github/stars/real-stanford/xskill.svg?style=social&label=Star)](https://github.com/real-stanford/xskill)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.09955)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://xskill.cs.columbia.edu/)

+ [SkillDiffuser: Interpretable Hierarchical Planning via Skill Abstractions in Diffusion-Based Task Execution](https://arxiv.org/abs/2312.11598) (CVPR 2024)
  [![Star](https://img.shields.io/github/stars/Liang-ZX/skilldiffuser.svg?style=social&label=Star)](https://github.com/Liang-ZX/skilldiffuser)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.11598)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://skilldiffuser.github.io/)

+ [Hierarchical Diffusion Policy for Kinematics-Aware Multi-Task Robotic Manipulation](https://arxiv.org/abs/2403.03890) (CVPR 2024)
  [![Star](https://img.shields.io/github/stars/dyson-ai/hdp.svg?style=social&label=Star)](https://github.com/dyson-ai/hdp)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.038908)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://yusufma03.github.io/projects/hdp/)

+ [Efficient Diffusion Transformer Policies with Mixture of Expert Denoisers for Multitask Learning](https://arxiv.org/abs/2412.12953) (Dec 2024)
  [![Star](https://img.shields.io/github/stars/intuitive-robots/MoDE_Diffusion_Policy.svg?style=social&label=Star)](https://github.com/intuitive-robots/MoDE_Diffusion_Policy)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.12953)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://mbreuss.github.io/MoDE_Diffusion_Policy/)



Is Conditional Generative Modeling all you need for Decision-Making? (Decision Diffuser)


+ [Waypoint-Based Imitation Learning for Robotic Manipulation](https://arxiv.org/abs/2307.14326) (CoRL 2023)
  [![Star](https://img.shields.io/github/stars/lucys0/awe.svg?style=social&label=Star)](https://github.com/lucys0/awe)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.14326)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://lucys0.github.io/awe/)


+ [RoLD: Robot Latent Diffusion for Multi-task Policy Modeling](https://arxiv.org/abs/2403.07312v3) ()
  [![Star](https://img.shields.io/github/stars/AlbertTan404/RoLD.svg?style=social&label=Star)](https://github.com/AlbertTan404/RoLD)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.07312v3)


+ [UMI on Legs: Making Manipulation Policies Mobile with Manipulation-Centric Whole-body Controllers](https://arxiv.org/abs/2407.10353) (CoRL 2024)
  [![Star](https://img.shields.io/github/stars/real-stanford/umi-on-legs.svg?style=social&label=Star)](https://github.com/real-stanford/umi-on-legs)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.10353)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://umi-on-legs.github.io/)

Robust Imitation Learning for Mobile Manipulator Focusing on Task-Related Viewpoints and Regions (mobile manipulation)

M2Diffuser: Diffusion-based Trajectory Optimization for Mobile Manipulation in 3D Scenes (mobile manipulation)

Pushing the Limits of Cross-Embodiment Learning for Manipulation and Navigation (a unified cross-embodiment model for both manipulation and navigation, but executed separately)


Provable Guarantees for Generative Behavior Cloning: Bridging Low-Level Stability and High-Level Behavior (Highly Theoretical)

Cold Diffusion on the Replay Buffer: Learning to Plan from Known Good States

Scaling Diffusion Policy in Transformer to 1 Billion Parameters for Robotic Manipulation

SplatSim: Zero-Shot Sim2Real Transfer of RGB Manipulation Policies Using Gaussian Splatting (Sim2Real)

---

Movement Primitive Diffusion: Learning Gentle Robotic Manipulation of Deformable Objects (Deformable)

SculptDiff: Learning Robotic Clay Sculpting from Humans with Goal Conditioned Diffusion Policy (3D deformable objects)

RoPotter: Toward Robotic Pottery and Deformable Object Manipulation with Structural Priors (3D deformable, pottery)

Garment Diffusion Models for Robot-Assisted Dressing

---

PianoMime: Learning a Generalist, Dexterous Piano Player from Internet Demonstrations

Learning Playing Piano with Bionic-Constrained Diffusion Policy for Anthropomorphic Hand

---

Learning Visuotactile Skills with Two Multifingered Hands

Adaptive Compliance Policy: Learning Approximate Compliance for Diffusion Guided Control (considering compliance / forces during manipulation)

ForceMimic: Force-Centric Imitation Learning with Force-Motion Capture System for Contact-Rich Manipulation (forces centric)

Learning Diffusion Policies from Demonstrations For Compliant Contact-rich Manipulation (considering compliance / forces)

VITaL Pretraining: Visuo-Tactile Pretraining for Tactile and Non-Tactile Manipulation Policies (force, tactile)

TacDiffusion: Force-domain Diffusion Policy for Precise Tactile Manipulation (force, tactile)

3D-ViTac: Learning Fine-Grained Manipulation with Visuo-Tactile Sensing (Include tactile)

Admittance Visuomotor Policy Learning for General-Purpose Contact-Rich Manipulations (force, contact-rich)

FoAR: Force-Aware Reactive Policy for Contact-Rich Robotic Manipulatio (force, contact)

Canonical Representation and Force-Based Pretraining of 3D Tactile for Dexterous Visuo-Tactile Policy Learning (tactile, force)

---

CAGE: Causal Attention Enables Data-Efficient Generalizable Robotic Manipulation (single task generalization)

+ [Planning-Guided Diffusion Policy Learning for Generalizable Contact-Rich Bimanual Manipulation](https://arxiv.org/abs/2412.02676) (Sep 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.02676)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://glide-manip.github.io/)
  <!-- [![Star](https://img.shields.io/github/stars/HRI-EU/flow-matching-policy.svg?style=social&label=Star)](https://github.com/HRI-EU/flow-matching-policy) -->

+ [GenDP: 3D Semantic Fields for Category-Level Generalizable Diffusion Policy](https://arxiv.org/abs/2410.17488) (CoRL 2024)
  [![Star](https://img.shields.io/github/stars/WangYixuan12/gendp.svg?style=social&label=Star)](https://github.com/WangYixuan12/gendp)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.17488)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://robopil.github.io/GenDP/)

+ [Equivariant Diffusion Policy](https://arxiv.org/abs/2407.01812) (CoRL 2024)
  [![Star](https://img.shields.io/github/stars/pointW/equidiff.svg?style=social&label=Star)](https://github.com/pointW/equidiff)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.01812)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://equidiff.github.io/)

+ [EquiBot: SIM (3)-Equivariant Diffusion Policy for Generalizable and Data Efficient Learning](https://arxiv.org/abs/2407.01479) (CoRL 2024)
  [![Star](https://img.shields.io/github/stars/yjy0625/equibot.svg?style=social&label=Star)](https://github.com/yjy0625/equibot)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.01479)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://equi-bot.github.io/)

Diffusion-EDFs: Bi-equivariant Denoising Generative Modeling on SE(3) for Visual Robotic Manipulation

DISCO: Language-Guided Manipulation with Diffusion Policies and Constrained Inpainting (zero-shot language-guided diffusion polic)

Learning Generalizable 3D Manipulation With 10 Demonstrations (3D, few-shot generalizability)

JUICER: Data-Efficient Imitation Learning for Robotic Assembly (learn from small human demonstrations)

Diffusion-PbD: Generalizable Robot Programming by Demonstration with Diffusion Features (learn from single demonstration)

ET-SEED: Efficient Trajectory-Level SE(3) Equivariant Diffusion Policy (learn from few demonstrations)

Imitation Learning with Limited Actions via Diffusion Planners and Deep Koopman Controllers (learn from few demonstrations)

---

Language-Guided Object-Centric Diffusion Policy for Collision-Aware Robotic Manipulation (3D, object centric, single task generalization)

Affordance-Centric Policy Learning: Sample Efficient and Generalisable Robot Policy Learning using Affordance-Centric Task Frames (object centric)

Motion Before Action: Diffusing Object Motion as Manipulation Condition (object motion)

SPOT: SE(3) Pose Trajectory Diffusion for Object-Centric Manipulation (Tracking object pose)

G3Flow: Generative 3D Semantic Flow for Pose-aware and Generalizable Object Manipulation (object centric)

---

C3DM: Constrained-Context Conditional Diffusion Models for Imitation Learning (tackle spurious correlation, distraction free)

From Imitation to Refinement – Residual RL for Precise Assembly (distribution shifts)

+ [Adaptive Online Replanning with Diffusion Models](https://arxiv.org/abs/2310.09629) (NeurIPS 2023)
  [![Star](https://img.shields.io/github/stars/rainbow979/replandiffuser.svg?style=social&label=Star)](https://github.com/rainbow979/replandiffuser)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.09629)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vis-www.cs.umass.edu/replandiffuser/)

Unpacking Failure Modes of Generative Policies: Runtime Monitoring of Consistency and Progress (out-of-distribution scenarios, detect failures)

Subgoal Diffuser: Coarse-to-fine Subgoal Generation to Guide Model Predictive Control for Robot Manipulation (long horizon, subgoal)

Goal-Reaching Policy Learning from Non-Expert Observations via Effective Subgoal Guidance (Diffusion sub-goals generation)

Failure Prediction from Limited Hardware Demonstrations (failure prediction)

---

MaIL: Improving Imitation Learning with Mamba (using Mamba)

Mamba Policy: Towards Efficient 3D Diffusion Policy with Hybrid Selective State Models (Mamba)

Crossway Diffusion: Improving Diffusion-based Visuomotor Policy via Self-supervised Learning

The Ingredients for Robotic Diffusion Transformers

Diffusion Transformer Policy

Discrete Policy: Learning Disentangled Action Space for Multi-Task Robotic Manipulation

<!-- Legibility Diffuser: Offline Imitation for Intent Expressive Motion (legible motion) -->


Diffusion Co-Policy for Synergistic Human-Robot Collaborative Tasks

Maximizing Alignment with Minimal Feedback: Efficiently Learning Rewards for Visuomotor Robot Policy Alignment (human preference alignment)

Task-based dialogue policy learning based on diffusion models (dialogue guidance, to be check)



INSTANT POLICY: IN-CONTEXT IMITATION LEARNING VIA GRAPH DIFFUSION (graph diffusion)

FlowBotHD: History-Aware Diffuser Handling Ambiguities in Articulated Objects Manipulation (ambiguity)

Diffusion Policy Attacker: Crafting Adversarial Attacks for Diffusion-based Policies (adversarial attack)

Towards Effective Utilization of Mixed-Quality Demonstrations in Robotic Manipulation via Segment-Level Selection and Optimization (demo data selection and filter)

Multimodal Diffusion Transformer: Learning Versatile Behavior from Multimodal Goals (learning from multimodal goal specifications with few language annotations)

Learning Diverse Robot Striking Motions with Diffusion Models and Kinematically Constrained Gradient Guidance (agile tasks)

Cutting Sequence Diffuser: Sim-to-Real Transferable Planning for Object Shaping by Grinding (grinding through grinding belt)

Hierarchical Diffusion Policy: manipulation trajectory generation via contact guidance (DP with contact guidance)

Implicit Contact Diffuser: Sequential Contact Reasoning with Latent Point Cloud Diffusion (contact)

Diff-Control: A Stateful Diffusion-based Policy for Imitation Learning (control net)


+ [Composable Part-Based Manipulation](https://arxiv.org/abs/2405.05876) (CoRL 2023)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.05876)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://cpmcorl2023.github.io/)

FREE FROM BELLMAN COMPLETENESS: TRAJECTORY STITCHING VIA MODEL-BASED RETURN-CONDITIONED SUPERVISED LEARNING

One-Shot Imitation under Mismatched Execution

LANGUAGE CONTROL DIFFUSION: EFFICIENTLY SCALING THROUGH SPACE, TIME, AND TASKS

SDP: Spiking Diffusion Policy for Robotic Manipulation with Learnable Channel-Wise Membrane Thresholds

#### Locomotion

+ [Generalizable Humanoid Manipulation with Improved 3D Diffusion Policies](https://arxiv.org/abs/2410.10803) (Oct 2024)
  [![Star](https://img.shields.io/github/stars/YanjieZe/Improved-3D-Diffusion-Policy.svg?style=social&label=Star)](https://github.com/YanjieZe/Improved-3D-Diffusion-Policy)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2410.10803)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://humanoid-manipulation.github.io/)

Diffusion-based learning of contact plans for agile locomotion

DIDI: Diffusion-Guided Diversity for Offline Behavioral Generation (To be checked)

Preference Aligned Diffusion Planner for Quadrupedal Locomotion Control (out-of-distribution issue)

The Role of Domain Randomization in Training Diffusion Policies for Whole-Body Humanoid Control

---
Reorientation / Pose estimation

StructDiffusion: Language-Guided Creation of Physically-Valid Structures using Unseen Objects (using diffusion model to generate correct pose for 3D objects)

+ [Shelving, stacking, hanging: Relational pose diffusion for multi-modal rearrangement](https://arxiv.org/abs/2307.04751) (CoRL 2023)
  [![Star](https://img.shields.io/github/stars/anthonysimeonov/rpdiff.svg?style=social&label=Star)](https://github.com/anthonysimeonov/rpdiff)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.04751)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://anthonysimeonov.github.io/rpdiff-multi-modal/)

DiffusionNOCS: Managing Symmetry and Uncertainty in Sim2Real Multi-Modal Category-level Pose Estimation (pose estimation)

Precise Pick-and-Place using Score-Based Diffusion Networks (pose prediction, coarse to fine)

+ [Reorientdiff: Diffusion model based reorientation for object manipulation](https://arxiv.org/abs/2303.12700) (ICRA 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.12700)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://umishra.me/ReorientDiff/)

DAP: Diffusion-based Affordance Prediction for Multi-modality Storage (storage problem to be accurate)

+ [Se(3)-diffusionfields: Learning cost functions for joint grasp and motion optimization through diffusion](https://arxiv.org/abs/2209.03855) (ICRA 2023)
  [![Star](https://img.shields.io/github/stars/robotgradient/grasp_diffusion.svg?style=social&label=Star)](https://github.com/robotgradient/grasp_diffusion)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2209.03855)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/se3dif)

#### Dexterous Manipulation


ViViDex: Learning Vision-based Dexterous Manipulation from Human Videos (learn from video, grasping)

Vision-Language-Action Model and Diffusion Policy Switching Enables Dexterous Control of an Anthropomorphic Hand (Combining openVLA and diffusion policy)

+ [Learning score-based grasping primitive for human-assisting dexterous grasping](https://arxiv.org/abs/2309.06038) (NeurIPS 2023)
  [![Star](https://img.shields.io/github/stars/tianhaowuhz/human-assisting-dex-grasp.svg?style=social&label=Star)](https://github.com/tianhaowuhz/human-assisting-dex-grasp/)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.06038)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/graspgf)


+ [DexDiffuser: Generating Dexterous Grasps with Diffusion Models](https://arxiv.org/abs/2402.02989) (Feb 2024)
  [![Star](https://img.shields.io/github/stars/YuLiHN/DexDiffuser.svg?style=social&label=Star)](https://github.com/YuLiHN/DexDiffuser)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.02989)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://yulihn.github.io/DexDiffuser_page/)

+ [Dexterous Functional Pre-Grasp Manipulation with Diffusion Policy](https://arxiv.org/abs/2403.12421) (Mar 2024)
  [![Star](https://img.shields.io/github/stars/tianhaowuhz/DexFunPreGrasp.svg?style=social&label=Star)](https://github.com/tianhaowuhz/DexFunPreGrasp)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.12421)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://unidexfpm.github.io/)

DexGrasp-Diffusion: Diffusion-based Unified Functional Grasp Synthesis Method for Multi-Dexterous Robotic Hands

Grasp Diffusion Network: Learning Grasp Generators from Partial Point Clouds with Diffusion Models in SO(3) × R3


#### Navigation

<!-- + [Diffusion Forcing: Next-token Prediction Meets Full-Sequence Diffusion](https://arxiv.org/abs/2407.01392) (NeurIPS 2024)
  [![Star](https://img.shields.io/github/stars/buoyancy99/diffusion-forcing.svg?style=social&label=Star)](https://github.com/buoyancy99/diffusion-forcing)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.01392)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://boyuan.space/diffusion-forcing/) -->

NoMaD: Goal Masked Diffusion Policies for Navigation and Exploration

DiPPeR: Diffusion-based 2D Path Planner applied on Legged Robots

LDP: A Local Diffusion Planner for Efficient Robot Navigation and Collision Avoidance

DTG : Diffusion-based Trajectory Generation for Mapless Global Navigation

DARE: Diffusion Policy for Autonomous Robot Exploration

FloNa: Floor Plan Guided Embodied Visual Navigation

Learning Wheelchair Tennis Navigation from Broadcast Videos with Domain Knowledge Transfer and Diffusion Motion Planning

FlowNav: Learning Efficient Navigation Policies via Conditional Flow Matching (flow matching)

Diffusion Meets Options: Hierarchical Generative Skill Composition for Temporally-Extended Tasks (Replanning)

#### Task and Motion Planning

LTLDoG: Satisfying Temporally-Extended Symbolic Constraints for Safe Diffusion-based Planning

SafeDiffuser: Safe Planning with Diffusion Probabilistic Models

DiffusionSeeder: Seeding Motion Optimization with Diffusion for Rapid Motion Planning (motion planning)

Potential Based Diffusion Motion Planning

RAIL: Reachability-Aided Imitation Learning for Safe Policy Execution (collision free, hard constraints)

Sampling Constrained Trajectories Using Composable Diffusion Models (Trajectory optimization with constraints present)

DiMSam: Diffusion Models as Samplers for Task and Motion Planning under Partial Observability (With constraint)

Motion Planning Diffusion: Learning and Adapting Robot Motion Planning with Diffusion Models
(Motion Planning Diffusion: Learning and Planning of Robot Motions with Diffusion Models)

#### Others

DroneDiffusion: Robust Quadrotor Dynamics Learning with Diffusion Models (Drones)

### Diffusion Generation Models in Robot Learning
+ DALL-E-Bot: [DALL-E-Bot: Introducing Web-Scale Diffusion Models to Robotics](https://arxiv.org/abs/2210.02438) (RA-Letters 2023)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2210.02438)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://www.robot-learning.uk/dall-e-bot)
  <!-- [![Star](https://img.shields.io/github/stars/ErinZhang1998/dmd_diffusion.svg?style=social&label=Star)](https://github.com/ErinZhang1998/dmd_diffusion) -->

+ UniPi: [Learning Universal Policies via Text-Guided Video Generation](https://arxiv.org/abs/2302.00111) (NeurIPS 2023)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.00111)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://universal-policy.github.io/unipi/)

+ AVDC: [Learning to Act from Actionless Videos through Dense Correspondences](https://arxiv.org/abs/2310.08576) (ICLR 2024)
  [![Star](https://img.shields.io/github/stars/flow-diffusion/AVDC.svg?style=social&label=Star)](https://github.com/flow-diffusion/AVDC)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.08576)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://flow-diffusion.github.io/)

+ UniSim: [UniSim: Learning Interactive Real-World Simulators](https://arxiv.org/abs/2310.06114) (ICLR 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.06114)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://universal-simulator.github.io/unisim/)
  <!-- [![Star](https://img.shields.io/github/stars/ErinZhang1998/dmd_diffusion.svg?style=social&label=Star)](https://github.com/ErinZhang1998/dmd_diffusion) -->


+ HiP: [Compositional Foundation Models for Hierarchical Planning](https://arxiv.org/abs/2309.08587) (NeurIPS 2023)
  [![Star](https://img.shields.io/github/stars/anuragajay/hip.svg?style=social&label=Star)](https://github.com/anuragajay/hip)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.08587)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://hierarchical-planning-foundation-model.github.io/)

+ DMD: [Diffusion Meets DAgger: Supercharging Eye-in-hand Imitation Learning](https://arxiv.org/abs/2402.17768) (Feb 2024)
  [![Star](https://img.shields.io/github/stars/ErinZhang1998/dmd_diffusion.svg?style=social&label=Star)](https://github.com/ErinZhang1998/dmd_diffusion)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.17768)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/diffusion-meets-dagger)

+ VLP: [Video language planning](https://arxiv.org/abs/2310.10625) (ICLR 2024)
  [![Star](https://img.shields.io/github/stars/video-language-planning/vlp_code.svg?style=social&label=Star)](https://github.com/video-language-planning/vlp_code)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.10625)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://video-language-planning.github.io/)
  
+ Dreamitate: [Dreamitate: Real-World Visuomotor Policy Learning via Video Generation](https://arxiv.org/abs/2406.16862) (CoRL 2024)
  [![Star](https://img.shields.io/github/stars/cvlab-columbia/dreamitate.svg?style=social&label=Star)](https://github.com/cvlab-columbia/dreamitate)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.16862)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://dreamitate.cs.columbia.edu/)

+ ARDuP: [ARDuP: Active Region Video Diffusion for Universal Policies](https://arxiv.org/abs/2406.13301) (Jun 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.13301)

+ This&That: [This&That: Language-Gesture Controlled Video Generation for Robot Planning](https://arxiv.org/abs/2407.05530) (July 2024)
  [![Star](https://img.shields.io/github/stars/cfeng16/this-and-that.svg?style=social&label=Star)](https://github.com/cfeng16/this-and-that)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.05530)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://cfeng16.github.io/this-and-that/)

+ RoboDreamer: [RoboDreamer: Learning Compositional World Models for Robot Imagination](https://arxiv.org/abs/2404.12377) (ICML 2024)
  [![Star](https://img.shields.io/github/stars/rainbow979/robodreamer.svg?style=social&label=Star)](https://github.com/rainbow979/robodreamer)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.12377)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://robovideo.github.io/)

+ CLOVER: [Closed-Loop Visuomotor Control with Generative Expectation for Robotic Manipulation](https://arxiv.org/abs/2409.09016) (NeurIPS 2024)
  [![Star](https://img.shields.io/github/stars/OpenDriveLab/CLOVER.svg?style=social&label=Star)](https://github.com/OpenDriveLab/CLOVER)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2409.09016)
  <!-- [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/diffusion-meets-dagger) -->

+ SOAR: [Autonomous Improvement of Instruction Following Skills via Foundation Models](https://arxiv.org/abs/2407.20635) (CoRL 2024)
  [![Star](https://img.shields.io/github/stars/rail-berkeley/soar.svg?style=social&label=Star)](https://github.com/rail-berkeley/soar)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.20635)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://auto-improvement.github.io/)

#### [unread]

+ Cacti: [Cacti: A framework for scalable multi-task multi-scene visual imitation learning](https://arxiv.org/abs/2212.05711) (CoRL 2022 Workshop PRL)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.05711)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://cacti-framework.github.io/)

+ GenAug: [GenAug: Retargeting behaviors to unseen situations via Generative Augmentation](https://arxiv.org/abs/2302.06671)
  [![Star](https://img.shields.io/github/stars/genaug/genaug.svg?style=social&label=Star)](https://github.com/genaug/genaug)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.06671)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://genaug.github.io/)

ViNT: A foundation model for visual navigation (navigation, sub goal image generation)

GR-MG: Leveraging Partially-Annotated Data via Multi-Modal Goal-Conditioned Policy (generate goal image)

Generative Image as Action Models

Scaling Robot Learning with Semantically Imagined Experience

Large-Scale Actionless Video Pre-Training via Discrete Diffusion for Efficient Policy Learning

Diffusion model is an effective planner and data synthesizer for multi-task reinforcement learning

3D-VLA: A 3D Vision-Language-Action Generative World Model

Learning Visual Parkour from Generated Images

GHIL-Glue: Hierarchical Control with Filtered Subgoal Images

VidMan: Exploiting Implicit Dynamics from Video Diffusion Model for Effective Robot Manipulation (inverse dynamics, distillation from video to action generation)

IMAGINATION POLICY: Using Generative Point Cloud Models for Learning Manipulation Policies (3D generation, goal-conditioned)

Embodiment-agnostic Action Planning via Object-Part Scene Flow (generate object part flow)

Imagine2Servo: Intelligent Visual Servoing with Diffusion-Driven Goal Generation for Robotic Tasks (generate image subgoal)

#### World models in robotics:

IRASim: Learning Interactive Real-Robot Action Simulators arXiv 2024.6

Structured World Models from Human Videos RSS 2023

HARP: Autoregressive Latent Video Prediction with High-Fidelity Image Generator ICIP 2022

DayDreamer: World Models for Physical Robot Learning CoRL 2022

#### Other work studying data generation in robotics (Not using diffusion)

MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations


### Robot Learning Utilizing Diffusion Model Properties
PoCo: Policy Composition from and for Heterogeneous Robot Learning (To be checked)

Diffusion Forcing: Next-token Prediction Meets Full-Sequence Diffusion (To be checked)

Pre-trained Text-to-Image Diffusion Models Are Versatile Representation Learners for Control

Imitation Learning from Purified Demonstrations (using forward & reverse diffusion process to purify imperfect demonstrations)

Human-Agent Joint Learning for Efficient Robot Manipulation Skill Acquisition (a diffusion-model-based assistive agent to learn how to assist humans in collecting data in a shared control manner)

P3-PO: Prescriptive Point Priors for Visuo-Spatial Generalization of Robot Policies (using DIFT for point correspondence)

+ [Adaptive Online Replanning with Diffusion Models](https://arxiv.org/abs/2310.09629) (NeurIPS 2023)
  [![Star](https://img.shields.io/github/stars/rainbow979/replandiffuser.svg?style=social&label=Star)](https://github.com/rainbow979/replandiffuser)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.09629)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vis-www.cs.umass.edu/replandiffuser/)

+ [Diffusion reward: Learning rewards via conditional video diffusion](https://arxiv.org/abs/2312.14134) (ECCV 2024)
  [![Star](https://img.shields.io/github/stars/TEA-Lab/diffusion_reward.svg?style=social&label=Star)](https://github.com/TEA-Lab/diffusion_reward)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.14134)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://diffusion-reward.github.io/)

