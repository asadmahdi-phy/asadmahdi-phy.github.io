---
layout: page
title: additional coursework
permalink: /coursework/
description: Schools, workshops, and supplementary courses in theoretical physics, gravitational waves, quantum information, and scientific computing.
nav: true
nav_order: 5
---

<style>
  .coursework-intro {
    margin-bottom: 2rem;
  }

  .coursework-list {
    margin-top: 1.5rem;
  }

  .coursework-item {
    display: grid;
    grid-template-columns: 8.5rem minmax(0, 1fr);
    column-gap: 1.5rem;
    padding: 1.4rem 0;
    border-bottom: 1px solid var(--global-divider-color);
  }

  .coursework-item:first-child {
    border-top: 1px solid var(--global-divider-color);
  }

  .coursework-date {
    color: var(--global-theme-color);
    font-weight: 600;
    line-height: 1.5;
  }

  .coursework-content h3 {
    margin: 0 0 0.3rem;
    font-size: 1.08rem;
    font-weight: 700;
  }

  .coursework-institution {
    margin-bottom: 0.5rem;
    color: var(--global-text-color-light);
    font-size: 0.95rem;
    font-weight: 500;
  }

  .coursework-description {
    margin: 0;
    line-height: 1.65;
  }

  .coursework-highlight {
    margin-top: 0.45rem;
    font-weight: 600;
  }

  .coursework-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem;
    margin-top: 0.75rem;
  }

  .coursework-link {
    display: inline-block;
    padding: 0.28rem 0.7rem;
    border: 1px solid var(--global-theme-color);
    border-radius: 0.3rem;
    color: var(--global-theme-color);
    font-size: 0.85rem;
    font-weight: 500;
    text-decoration: none;
    transition:
      color 0.2s ease,
      background-color 0.2s ease;
  }

  .coursework-link:hover {
    color: var(--global-bg-color);
    background-color: var(--global-theme-color);
    text-decoration: none;
  }

  @media (max-width: 576px) {
    .coursework-item {
      grid-template-columns: 1fr;
      row-gap: 0.35rem;
    }

    .coursework-date {
      font-size: 0.9rem;
    }
  }
</style>

<div class="coursework-intro">
  <p>
    In addition to my formal university education, I have participated in
    specialized schools, workshops, and supplementary courses covering
    theoretical physics, gravitational-wave data analysis, general relativity,
    quantum information, quantum computing, and machine learning.
  </p>
</div>

<div class="coursework-list">

  <!-- GW Open Data Workshop -->
  <div class="coursework-item">
    <div class="coursework-date">April 2026</div>

    <div class="coursework-content">
      <h3>GW Open Data Workshop 2026</h3>

      <div class="coursework-institution">
        L2IT, Toulouse, France
      </div>

      <p class="coursework-description">
        Lectures, tutorials, quizzes, and challenges on LIGO-Virgo-KAGRA
        gravitational-wave data analysis, including signal processing,
        compact-binary-coalescence searches, and parameter inference.
      </p>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1PbmPZZ4fAnfnkH7GRS8YuNbncwIqsgxB/view?usp=sharing"
          target="_blank"
          rel="noopener noreferrer"
        >
          Certificate
        </a>
      </div>
    </div>
  </div>

  <!-- JNI Memorial Winter School -->
  <div class="coursework-item">
    <div class="coursework-date">February 2025</div>

    <div class="coursework-content">
      <h3>JNI Memorial Winter School in Mathematical and Theoretical Physics</h3>

      <div class="coursework-institution">
        ICTP Physics Without Frontiers
      </div>

      <p class="coursework-description">
        Lectures on string theory, black holes, and the black-hole information
        paradox.
      </p>
    </div>
  </div>

  <!-- QFT School -->
  <div class="coursework-item">
    <div class="coursework-date">August 2024</div>

    <div class="coursework-content">
      <h3>School on Quantum Field Theory</h3>

      <div class="coursework-institution">
        ICTP Physics Without Frontiers: Physics for Bangladesh
      </div>

      <p class="coursework-description">
        Quantum field theory from canonical quantization to the path-integral
        formulation.
      </p>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1ItzpFx0SBUfBEOPVdSnI419z618Wgtte/view?usp=drivesdk"
          target="_blank"
          rel="noopener noreferrer"
        >
          Certificate
        </a>
      </div>
    </div>
  </div>

  <!-- Relativistic Geometrodynamics -->
  <div class="coursework-item">
    <div class="coursework-date">
      July 2023<br>
      to December 2023
    </div>

    <div class="coursework-content">
      <h3>Modern Relativistic Geometrodynamics</h3>

      <div class="coursework-institution">
        Community of Physics
      </div>

      <p class="coursework-description">
        Audited course on exterior calculus and its application to the
        Einstein-Cartan formulation of general relativity.
      </p>
    </div>
  </div>

  <!-- Qiskit Global Summer School -->
  <div class="coursework-item">
    <div class="coursework-date">September 2023</div>

    <div class="coursework-content">
      <h3>Qiskit Global Summer School 2023</h3>

      <div class="coursework-institution">
        IBM
      </div>

      <p class="coursework-description">
        Qiskit fundamentals, quantum query algorithms, phase estimation,
        factoring, quantum noise, iterative quantum phase estimation,
        variational quantum eigensolvers, and noise-mitigation techniques.
      </p>

      <p class="coursework-highlight">
        Earned the Quantum Excellence badge after completing all laboratory
        exercises.
      </p>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1Z8umHJOVNzrAY0ud266fKYhdLr6lw1yy/view?usp=sharing"
          target="_blank"
          rel="noopener noreferrer"
        >
          Certificate
        </a>

        <a
          class="coursework-link"
          href="https://www.credly.com/badges/b215d398-533c-4c02-9907-b634c2118558/linked_in_profile"
          target="_blank"
          rel="noopener noreferrer"
        >
          Quantum Excellence Badge
        </a>
      </div>
    </div>
  </div>

  <!-- AWS Machine Learning -->
  <div class="coursework-item">
    <div class="coursework-date">September 2023</div>

    <div class="coursework-content">
      <h3>Introduction to Machine Learning and Reinforcement Learning</h3>

      <div class="coursework-institution">
        Amazon Web Services
      </div>

      <p class="coursework-description">
        Completed introductory coursework in machine learning and reinforcement
        learning, with pre-qualification for the AWS AI &amp; ML Scholarship.
      </p>
    </div>
  </div>

  <!-- Womanium -->
  <div class="coursework-item">
    <div class="coursework-date">August 2023</div>

    <div class="coursework-content">
      <h3>Womanium Global Quantum Program 2023</h3>

      <div class="coursework-institution">
        Womanium
      </div>

      <p class="coursework-description">
        Modules on quantum key distribution, quantum error correction, quantum
        hardware, and quantum software.
      </p>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1ohcy6n4WnjcU8Upit20faios2O2FAFHR/view?usp=drivesdk"
          target="_blank"
          rel="noopener noreferrer"
        >
          Certificate
        </a>
      </div>
    </div>
  </div>

  <!-- QNickel -->
  <div class="coursework-item">
    <div class="coursework-date">August 2023</div>

    <div class="coursework-content">
      <h3>QNickel-7: Quantum Computing and Programming</h3>

      <div class="coursework-institution">
        QWorld
      </div>

      <p class="coursework-description">
        Deutsch-Jozsa, Bernstein-Vazirani, and Simon's algorithms, together
        with solving the Max-Cut problem using Grover's search algorithm.
      </p>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1rK3UN3z73ByCAtuApbP6LUkN7WNtavtl/view?usp=drive_link"
          target="_blank"
          rel="noopener noreferrer"
        >
          Certificate
        </a>
      </div>
    </div>
  </div>

  <!-- GR Workshop -->
  <div class="coursework-item">
    <div class="coursework-date">May 2023</div>

    <div class="coursework-content">
      <h3>1st Workshop on General Relativity: Geometry Matters</h3>

      <div class="coursework-institution">
        Community of Physics
      </div>

      <p class="coursework-description">
        Five-day introductory workshop comprising approximately 50 hours of
        lectures on general relativity.
      </p>

      <p class="coursework-highlight">
        Secured first position in the post-workshop assessment.
      </p>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1yU8pisfuep7piuQ83I6YE2NpmcagDrJH/view?usp=share_link"
          target="_blank"
          rel="noopener noreferrer"
        >
          Certificate
        </a>
      </div>
    </div>
  </div>

  <!-- Quantum Information -->
  <div class="coursework-item">
    <div class="coursework-date">
      November 2022<br>
      to May 2023
    </div>

    <div class="coursework-content">
      <h3>Quantum Information</h3>

      <div class="coursework-institution">
        Tensor College, Bangladesh
      </div>

      <p class="coursework-description">
        A series of three semester-long courses on quantum mechanics, quantum
        information, and related computational methods, instructed by
        Dr. Tibra Ali.
      </p>
    </div>
  </div>

  <!-- QBronze -->
  <div class="coursework-item">
    <div class="coursework-date">April 2023</div>

    <div class="coursework-content">
      <h3>QBronze-106: Quantum Computing and Programming</h3>

      <div class="coursework-institution">
        QWorld
      </div>

      <p class="coursework-description">
        Four online classes of four hours each, with graded assignments based
        on the standard QBronze repository.
      </p>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1D3kV9KnGwDzLwJRjH6K0avktsFWvdnoO/view?usp=sharing"
          target="_blank"
          rel="noopener noreferrer"
        >
          Certificate
        </a>
      </div>
    </div>
  </div>

  <!-- Quantum Mechanics and Computation -->
  <div class="coursework-item">
    <div class="coursework-date">2022</div>

    <div class="coursework-content">
      <h3>Quantum Mechanics and Computation, Parts I and II</h3>

      <p class="coursework-description">
        Fundamental concepts of quantum mechanics using wave-mechanical and
        matrix-mechanical approaches, together with numerical simulations
        using COMSOL.
      </p>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1TcJpnGgyBT2aRqA_hBcLIz_n4zduaxJp/view?usp=share_link"
          target="_blank"
          rel="noopener noreferrer"
        >
          Part I Certificate
        </a>

        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1gtM30EVi3dj5BdD2smRK5PwDJ54QpdSY/view?usp=share_link"
          target="_blank"
          rel="noopener noreferrer"
        >
          Part II Certificate
        </a>
      </div>
    </div>
  </div>

</div>
