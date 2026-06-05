---
layout: page
title: "Failure-Aware Residual Adaptation for Class-Incremental Learning"
description: Failure-localized residual correction for PEFT-based continual learning
img: assets/img/projects/fara_thumb.png
importance: 3
category: research
published: true
---

![FARA overview](/assets/img/projects/fara_main.png)

**Note:** This file is marked `published: false` because the project may still be under anonymous review. Remove `published: false` only when it is safe to make this page public.

FARA studies parameter-efficient class-incremental learning with frozen pre-trained vision models. Rather than uniformly enlarging task-level adapters, FARA identifies residual failure regions left by the primary adaptation path and allocates a separate correction stream to those empirically mined failures.

For each task, the method trains a primary adapter on the full task data, mines held-out mistakes through two-fold self-evaluation, and trains a failure adapter only on the residual failure cases. Failure-aware classifier alignment then uses both dominant class statistics and failure-specific statistics, while inference applies uncertainty-gated failure correction only when primary predictions are unreliable.

**Highlights**

- Studies failure-localized correction in PEFT-based class-incremental learning.
- Separates primary adaptation from residual failure correction.
- Uses failure mining, failure-aware classifier alignment, and uncertainty-gated correction.
- Evaluated on CIFAR-100, ImageNet-R, ImageNet-A, and CUB-200.
