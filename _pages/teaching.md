---
layout: page
permalink: /teaching/
title: Teaching
description:
nav: true
nav_order: 6
---

<style>
.teaching-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1rem;
  margin-top: 1.5rem;
}

.course-card {
  border: 1px solid var(--global-divider-color);
  border-radius: 8px;
  padding: 1.25rem;
  background: var(--global-card-bg-color);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.course-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 14px rgba(0,0,0,0.08);
}

.course-title {
  font-size: 1.15rem;
  font-weight: 700;
  margin-bottom: 0.35rem;
  color: var(--global-theme-color);
}

.course-description {
  font-size: 0.92rem;
  line-height: 1.45;
  margin: 0;
}

.course-status {
  margin-top: 0.8rem;
  font-size: 0.82rem;
  opacity: 0.7;
}

@media (max-width: 700px) {
  .teaching-grid {
    grid-template-columns: 1fr;
  }
}
</style>

## Courses

<div class="teaching-grid">

  <div class="course-card">
    <div class="course-title">Materials Characterization</div>
    <p class="course-description">
      Fundamentals and techniques for the structural, morphological, and optical characterization of materials.
    </p>
    <div class="course-status">Course materials</div>
  </div>

  <div class="course-card">
    <div class="course-title">Oscillations and Waves Laboratory</div>
    <p class="course-description">
      Experimental studies of oscillations, waves, resonance, and related wave phenomena.
    </p>
    <div class="course-status">Course materials</div>
  </div>

  <div class="course-card">
    <div class="course-title">Optical Properties of Materials</div>
    <p class="course-description">
      Light-matter interaction and the optical response of materials.
    </p>
    <div class="course-status">Course materials</div>
  </div>

  <div class="course-card">
    <div class="course-title">Thermodynamics</div>
    <p class="course-description">
      Macroscopic thermodynamics, fundamental laws, thermodynamic processes, entropy, and cycles.
    </p>
    <div class="course-status">Course materials</div>
  </div>

  <div class="course-card">
    <div class="course-title">Experimental Thermodynamics</div>
    <p class="course-description">
      Experimental studies of heat, temperature, thermal properties, and thermodynamic processes.
    </p>
    <div class="course-status">Course materials</div>
  </div>

<div class="course-card">
    <div class="course-title">Thermodynamics</div>
    <p class="course-description">
      Macroscopic.
    </p>
    <div class="course-status">Course materials</div>
  </div>

</div>
