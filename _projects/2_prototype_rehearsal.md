---
layout: page
title: "Revisiting Prototype Rehearsal for Exemplar-Free Continual Learning"
description: Manifold-aware boundary sampling with adaptive class-balanced loss
img: assets/img/projects/prototype_rehearsal_thumb.png
importance: 2
category: research
---

<p align="center">
<img src="/assets/img/projects/prototype_rehearsal_main.png" alt="Prototype rehearsal overview" style="width: 100%; max-width: 950px; height: auto; display: block; margin: 0.5rem auto 1.5rem auto; border-radius: 8px;">
</p>

This project revisits prototype rehearsal for exemplar-free class-incremental learning. We argue that prototype rehearsal is not fundamentally limited; rather, common implementations suffer from two issues: they treat prototypes as isolated class summaries and they ignore the hidden imbalance between a few synthetic old-class samples and many real current-task samples.

To address these issues, we introduce **Constrained Expansive Over-Sampling (CEOS)** and **Adaptive Class-Balanced (ACB) Loss**. CEOS generates boundary-aware synthetic features by interpolating old-class prototypes toward nearest enemy features while preserving class separation. ACB Loss dynamically reweights classes over time to reduce the temporal imbalance between prototype-based old-class supervision and current-task data.

**Highlights**

- Accepted to **CVPR 2026 Findings**.
- Restores the competitiveness of prototype rehearsal in exemplar-free CIL.
- Combines manifold-aware boundary sampling with time-aware class balancing.
- Code: [HXuSz11/ACB_CEOS_CVPR2026_Findings](https://github.com/HXuSz11/ACB_CEOS_CVPR2026_Findings)
