---
layout: page
title: "Adaptive Distillation via Online Drift Projection"
description: Class-adaptive preservation for exemplar-free class-incremental learning
img: assets/img/projects/odp_thumb.png
importance: 4
category: research
published: false
---

![ODP overview](/assets/img/projects/odp_main.png)

**Note:** This file is marked `published: false` because the project may still be under anonymous review. Remove `published: false` only when it is safe to make this page public.

This project studies heterogeneous representation drift in prototype-based exemplar-free class-incremental learning. Instead of applying uniform preservation strength to all old classes, Online Drift Projection estimates class-wise drift by projecting stored old-class prototypes into the current feature space.

The projected prototype displacement gives an exemplar-free drift signal for each old class. The method converts this signal into drift-weighted distillation, strengthening preservation for high-drift classes while relaxing constraints on stable classes. This class-adaptive view improves the stability-plasticity trade-off under strict exemplar-free constraints.

**Highlights**

- Introduces online drift projection for estimating class-wise representation drift.
- Uses projected prototype displacement as an exemplar-free drift proxy.
- Applies drift-weighted distillation to focus preservation on high-drift classes.
- Evaluated on CIFAR-100, TinyImageNet, ImageNet-100, and CUB-200.
