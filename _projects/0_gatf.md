---
layout: page
title: "Geometry-Anchored Transport Framework for Exemplar-Free Class-Incremental Learning"
description: Training-time geometry anchoring for transporting Gaussian class statistics in EFCIL
img: assets/img/projects/gatf_thumb.png
importance: 0
category: research
---

<p align="center">
<img src="/assets/img/projects/gatf_main.png" alt="GATF overview" style="width: 100%; max-width: 1000px; height: auto; display: block; margin: 0.5rem auto 1.5rem auto; border-radius: 1.5% / 3.5%;">
</p>

This project studies how class-conditional Gaussian statistics should be transported across tasks in exemplar-free class-incremental learning. Existing methods typically follow a decoupled, post-hoc paradigm: the backbone is first updated with distillation, and an adapter is fitted afterwards to map old prototypes into the new feature space. Without geometric constraints during training, the backbone can distort the legacy feature manifold, and Mahalanobis-based evaluation amplifies transport errors along low-variance directions.

The **Geometry-Anchored Transport Framework** instead treats feature transport as a constraint during primary training. An **Analytic Geometric Anchor (AGA)**, derived in closed form via Mahalanobis-aligned generalized least squares, captures the dominant anisotropic drift. **Topology-Aware Evolution** anchors the legacy neighborhood structure during backbone optimization, while a residual MLP calibrates the remaining non-linear deformation against the analytic prior. Old-class Gaussians are then pushed forward through the learned adapter without a separate fine-tuning stage.

**Highlights**

- Accepted to **ECCV 2026**.
- Couples feature transport with representation learning instead of applying it after training.
- Combines a closed-form Mahalanobis-aligned anchor with topology-aware residual calibration, supported by margin-stability bounds.
- Achieves the best final accuracy on CIFAR-100, TinyImageNet, and ImageNet-100 (T=10 and T=20) among the compared exemplar-free methods; also evaluated on CUB-200.
- Paper: [arXiv:2606.25347](https://arxiv.org/abs/2606.25347)
- Code: [HXuSz11/GATF_ECCV2026](https://github.com/HXuSz11/GATF_ECCV2026)
