---
layout: page
title: "Two-Way Is Better Than One: Bidirectional Alignment with Cycle Consistency"
description: Bidirectional projector alignment for exemplar-free class-incremental learning
img: assets/img/projects/bicyc_thumb.png
importance: 1
category: research
---

![BiCyc overview](/assets/img/projects/bicyc_main.png)

**BiCyc** studies prototype drift in exemplar-free class-incremental learning. Instead of learning only a one-way post-hoc projection from old features to new features, this project jointly learns two maps, old→new and new→old, with a cycle-consistency objective so that prototype transport and representation learning co-evolve during incremental training.

The key idea is to reduce accumulated transport error between feature spaces. The old→new map transports stored Gaussian prototypes into the current representation space, while the new→old map provides backward alignment. Cycle consistency regularizes the two maps toward near-inverse behavior, helping preserve geometry and reduce forgetting.

**Highlights**

- Accepted to **ICLR 2026**.
- Introduces bidirectional projector alignment with cycle consistency for EFCIL.
- Reduces prototype drift and improves old-class retention across CIFAR-100, TinyImageNet, ImageNet-100, and CUB-200.
- Code: [HXuSz11/BiCyc_ICLR2026](https://github.com/HXuSz11/BiCyc_ICLR2026)
