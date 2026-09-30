---
layout: page
permalink: /teaching/
title: teaching
description: Courses and teaching materials.
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
    <div class="course-title">Caracterización de Materiales</div>
    <p class="course-description">
      Fundamentos y técnicas para la caracterización estructural, morfológica y óptica de materiales.
    </p>
    <div class="course-status">Material del curso</div>
  </div>

  <div class="course-card">
    <div class="course-title">Laboratorio de Oscilaciones y Ondas</div>
    <p class="course-description">
      Prácticas experimentales sobre oscilaciones, ondas, resonancia y fenómenos ondulatorios.
    </p>
    <div class="course-status">Material del curso</div>
  </div>

  <div class="course-card">
    <div class="course-title">Propiedades Ópticas de los Materiales</div>
    <p class="course-description">
      Interacción luz-materia y propiedades ópticas de materiales.
    </p>
    <div class="course-status">Material del curso</div>
  </div>

  <div class="course-card">
    <div class="course-title">Termodinámica</div>
    <p class="course-description">
      Termodinámica macroscópica, procesos, leyes fundamentales, entropía y ciclos.
    </p>
    <div class="course-status">Material del curso</div>
  </div>

  <div class="course-card">
    <div class="course-title">Termodinámica Experimental</div>
    <p class="course-description">
      Prácticas experimentales relacionadas con calor, temperatura y procesos termodinámicos.
    </p>
    <div class="course-status">Material del curso</div>
  </div>

</div>
