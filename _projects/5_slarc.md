---
layout: page
title: "SLARC: Shrinkage-Controlled Low-Rank Alignment and Regularized Classification"
description: Constrained mean alignment and regularized Gaussian classification for EFCIL with pre-trained models
img: assets/img/projects/slarc_thumb.png
importance: 3
category: research
---

<p align="center">
<img src="/assets/img/projects/slarc_main.png" alt="SLARC overview" style="width: 100%; max-width: 1000px; height: auto; display: block; margin: 0.5rem auto 1.5rem auto; border-radius: 8px;">
</p>

This project studies exemplar-free class-incremental learning with continually adapted pre-trained vision transformers. When LoRA-style adapters keep changing the representation, stored class means and covariances describe an earlier feature space, yet the old images needed to recompute them are gone. SLARC addresses two questions: how much of an estimated correction should be applied to old-class means, and how much class-specific covariance structure the classifier should retain.

**Constrained mean alignment** fits an identity-centered, low-rank affine residual in a subspace that keeps the principal feature directions and the observed mean displacement. Fits from disjoint image halves are compared at the cached old-class means, and the whole update is shrunk when they disagree. **Regularized Gaussian classification** combines retained class covariances with pooled and spherical estimates, selecting the regularization from validation scores archived at class introduction, without storing old images or individual features.

**Highlights**

- Submitted to **ICLR 2027**.
- Plug-and-play on top of different hosts, including E²-LoRA, SLCA, and TUNA.
- Improves E²-LoRA's final accuracy by 0.70–4.08 percentage points across four ten-task benchmarks.
- Evaluated on CIFAR-100, ImageNet-R, ImageNet-A, and Cars-196.
