---
layout: page
title: projects
permalink: /projects/
description: Selected research projects.
nav: true
nav_order: 3
---

<style>
.projects-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.75rem;
  margin-top: 1.5rem;
}

@media (min-width: 992px) {
  .projects-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}

.project-card-custom {
  display: flex;
  flex-direction: column;
  border: 1px solid var(--global-divider-color);
  border-radius: 12px;
  overflow: hidden;
  background: var(--global-bg-color);
  color: var(--global-text-color);
  text-decoration: none;
  transition: transform 0.15s ease, box-shadow 0.15s ease;
  height: 100%;
}

.project-card-custom:hover {
  transform: translateY(-4px);
  text-decoration: none;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
}

.project-card-custom img {
  width: 100%;
  height: 210px;
  object-fit: contain;
  background: #ffffff;
  padding: 0.75rem;
  border-bottom: 1px solid var(--global-divider-color);
}

.project-card-body {
  padding: 1rem 1.1rem 1.15rem 1.1rem;
}

.project-card-body h3 {
  font-size: 1.05rem;
  line-height: 1.35;
  margin-bottom: 0.55rem;
  color: var(--global-theme-color);
}

.project-card-body p {
  font-size: 0.92rem;
  line-height: 1.5;
  margin-bottom: 0.7rem;
  color: var(--global-text-color);
}

.project-tag {
  display: inline-block;
  font-size: 0.75rem;
  font-weight: 600;
  padding: 0.18rem 0.48rem;
  border-radius: 999px;
  border: 1px solid var(--global-divider-color);
  margin-bottom: 0.65rem;
}
</style>

<div class="projects-grid">

<a class="project-card-custom" href="/projects/1_bicyc/">
<img src="/assets/img/projects/bicyc_thumb.png" alt="BiCyc project thumbnail">
<div class="project-card-body">
<div class="project-tag">ICLR 2026</div>
<h3>Two-Way Is Better Than One: Bidirectional Alignment with Cycle Consistency</h3>
<p>Bidirectional projector alignment with cycle consistency for exemplar-free class-incremental learning.</p>
</div>
</a>

<a class="project-card-custom" href="/projects/2_prototype_rehearsal/">
<img src="/assets/img/projects/prototype_rehearsal_thumb.png" alt="Prototype rehearsal project thumbnail">
<div class="project-card-body">
<div class="project-tag">CVPR 2026 Findings</div>
<h3>Revisiting Prototype Rehearsal for Exemplar-Free Continual Learning</h3>
<p>Manifold-aware boundary sampling with adaptive class-balanced loss for prototype rehearsal.</p>
</div>
</a>

<a class="project-card-custom" href="/projects/3_fara_hidden_draft/">
<img src="/assets/img/projects/fara_thumb.png" alt="FARA project thumbnail">
<div class="project-card-body">
<div class="project-tag">PEFT-CIL</div>
<h3>Failure-Aware Residual Adaptation for Class-Incremental Learning</h3>
<p>Failure-localized residual correction for parameter-efficient continual learning with frozen vision backbones.</p>
</div>
</a>

<a class="project-card-custom" href="/projects/4_odp_hidden_draft/">
<img src="/assets/img/projects/odp_thumb.png" alt="ODP project thumbnail">
<div class="project-card-body">
<div class="project-tag">EFCIL</div>
<h3>Adaptive Distillation via Online Drift Projection</h3>
<p>Class-wise drift estimation and drift-weighted distillation for exemplar-free class-incremental learning.</p>
</div>
</a>

</div>
