---
layout: page
permalink: /student-supervision/
title: Student Supervision
nav: true
nav_order: 9
---

<style>

.student-intro {
  margin-bottom: 2rem;
}

.student-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.5rem;
  margin-top: 1.5rem;
}

.student-card {
  display: grid;
  grid-template-columns: 180px 1fr;
  gap: 1.5rem;
  align-items: start;

  border: 1px solid var(--global-divider-color);
  border-radius: 10px;
  padding: 1.25rem;

  background: var(--global-card-bg-color);

  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.student-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 14px rgba(0,0,0,0.08);
}

.student-photo img {
  width: 180px;
  height: 220px;
  object-fit: cover;
  border-radius: 8px;
}

.student-name {
  font-size: 1.35rem;
  font-weight: 700;
  color: var(--global-theme-color);
  margin-bottom: 0.3rem;
}

.student-title {
  font-size: 1.05rem;
  font-weight: 600;
  margin-bottom: 0.9rem;
}

.student-abstract {
  font-size: 0.95rem;
  line-height: 1.55;
  margin-bottom: 0.9rem;
  text-align: justify;
}

.student-keywords {
  font-size: 0.9rem;
}

.student-keywords strong {
  font-weight: 600;
}

@media (max-width: 700px) {

  .student-card {
    grid-template-columns: 1fr;
  }

  .student-photo img {
    width: 160px;
    height: 200px;
  }

}

</style>

<div class="student-grid">
<!-- ====================================================== -->
<!-- STUDENT 1 --> Osmar Gil Salas
<!-- ====================================================== -->

<div class="student-card">

  <div class="student-photo">
    <img src="/assets/img/students/osmar-gil-salas.jpg" alt="Osmar Gil Salas">
  </div>

  <div>

    <div class="student-name">
      Osmar Gil Salas
    </div>

    <div class="student-title">
      Estudio numérico de plasmones superficiales localizados en sistemas de film metálico de oro sobre arreglos ordenados de nanoesferas
    </div>

    <div class="student-abstract">
      <strong>Abstract.</strong>
      Numerical and experimental characterization of Au-film systems on ordered arrays of nanospheres (AuFON), focusing on localized surface plasmon modes and the spatial distribution of the electric field. The study analyzes the dependence of the plasmonic response on nanostructure dimensions, light polarization, angle of incidence, and sample orientation, including a comparison between numerical simulations and experimental results.
    </div>

    <div class="student-keywords">
      <strong>Keywords:</strong>
      plasmonics, localized surface plasmons, AuFON, nanospheres, numerical simulation
    </div>

  </div>

</div>

</div>
