```html
---
layout: page
title: coursework
permalink: /coursework/
description: Schools, workshops, and supplementary coursework in theoretical physics, gravitational waves, quantum information, quantum computing, machine learning, and scientific programming.
nav: true
nav_order: 6
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
    grid-template-columns: 9rem minmax(0, 1fr);
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
    margin-bottom: 0.55rem;
    color: var(--global-text-color-light);
    font-size: 0.95rem;
    font-weight: 500;
  }

  .coursework-description {
    margin: 0;
    line-height: 1.65;
  }

  .coursework-topics {
    margin: 0.65rem 0 0;
    padding-left: 1.25rem;
  }

  .coursework-topics li {
    margin-bottom: 0.35rem;
    line-height: 1.55;
  }

  .coursework-highlight {
    margin-top: 0.55rem;
    font-weight: 600;
  }

  .coursework-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem;
    margin-top: 0.8rem;
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
    specialized schools, workshops, and supplementary courses in theoretical
    physics, gravitational-wave data analysis, general relativity, quantum
    information, quantum computing, machine learning, and scientific
    programming.
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
        Lectures, tutorials, quizzes, and practical challenges on
        LIGO-Virgo-KAGRA gravitational-wave data analysis, including signal
        processing, searches for compact binary coalescences, and source
        parameter inference.
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
        Specialized lectures on string theory, black-hole physics, and the
        black-hole information paradox.
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
        An intensive introduction to quantum field theory, progressing from
        canonical quantization to the path-integral formulation.
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

  <!-- Qiskit Global Summer School -->
  <div class="coursework-item">
    <div class="coursework-date">September 2023</div>

    <div class="coursework-content">
      <h3>Qiskit Global Summer School 2023</h3>

      <div class="coursework-institution">
        IBM
      </div>

      <p class="coursework-description">
        Coursework and laboratory exercises covering:
      </p>

      <ul class="coursework-topics">
        <li>Qiskit fundamentals and quantum circuit programming</li>
        <li>Quantum query algorithms</li>
        <li>Quantum phase estimation and integer factorization</li>
        <li>Iterative quantum phase estimation</li>
        <li>Variational quantum eigensolvers</li>
        <li>Quantum noise and error-mitigation techniques</li>
      </ul>

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
        Introductory coursework in machine learning and reinforcement learning.
        Completion of the programme resulted in pre-qualification for the AWS
        AI &amp; ML Scholarship.
      </p>
    </div>
  </div>

  <!-- Womanium and QWorld Programme -->
  <div class="coursework-item">
    <div class="coursework-date">
      August–September 2023
    </div>

    <div class="coursework-content">
      <h3>Womanium Global Quantum Program 2023</h3>

      <div class="coursework-institution">
        Womanium and QWorld
      </div>

      <p class="coursework-description">
        A global quantum-training programme comprising specialized coursework
        in quantum communication, quantum error correction, quantum software,
        and quantum hardware.
      </p>

      <ul class="coursework-topics">
        <li>
          <strong>QMercury-1: Quantum Key Distribution</strong><br>
          Classical cryptography and its limitations, quantum cryptography,
          the BB84 protocol, quantum key distribution in the presence of
          noise, and entanglement-based quantum key distribution.
        </li>

        <li>
          <strong>QZinc-1: Quantum Error Correction</strong><br>
          Classical and quantum error correction, quantum error-correcting
          codes, and the stabilizer formalism.
        </li>

        <li>
          <strong>Quantum Computing Software</strong><br>
          Quantum optimization, quantum annealing, quadratic unconstrained
          binary optimization, and quantum machine learning.
        </li>

        <li>
          <strong>Quantum Hardware</strong><br>
          Superconducting, trapped-ion, neutral-atom, photonic, and
          silicon-based quantum-computing platforms.
        </li>
      </ul>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1ohcy6n4WnjcU8Upit20faios2O2FAFHR/view?usp=drivesdk"
          target="_blank"
          rel="noopener noreferrer"
        >
          Programme Certificate
        </a>

        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1VqOcjjbpJDMEzt2ry34MXdfO4JMHvPwc/view?usp=drive_link"
          target="_blank"
          rel="noopener noreferrer"
        >
          QMercury Certificate
        </a>

        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1MG2RkQJbiX_5hJWjgvmwsSn2VlGkWDhK/view?usp=drive_link"
          target="_blank"
          rel="noopener noreferrer"
        >
          QZinc Certificate
        </a>

        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1Fcn_O9-oqj7Sx43MckbKqLaX4SZY5U7C/view?usp=drive_link"
          target="_blank"
          rel="noopener noreferrer"
        >
          Quantum Software Certificate
        </a>

        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1Nw_hhSwuH00qpgK58ktluOb3ZZBTm1pm/view?usp=drive_link"
          target="_blank"
          rel="noopener noreferrer"
        >
          Quantum Hardware Certificate
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
        Quantum algorithm coursework covering the Deutsch-Jozsa,
        Bernstein-Vazirani, and Simon algorithms, together with an application
        of Grover's search algorithm to the Max-Cut problem.
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

  <!-- Relativistic Geometrodynamics -->
  <div class="coursework-item">
    <div class="coursework-date">
      July–December 2023
    </div>

    <div class="coursework-content">
      <h3>Modern Relativistic Geometrodynamics</h3>

      <div class="coursework-institution">
        Community of Physics
      </div>

      <p class="coursework-description">
        Audited course on exterior calculus and differential-geometric methods
        leading to the Einstein-Cartan formulation of general relativity.
      </p>
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
        A five-day introductory workshop consisting of approximately 50 hours
        of lectures on the mathematical and physical foundations of general
        relativity.
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
      November 2022–May 2023
    </div>

    <div class="coursework-content">
      <h3>Quantum Information</h3>

      <div class="coursework-institution">
        Tensor College, Bangladesh
      </div>

      <p class="coursework-description">
        A three-course sequence designed as an introduction to quantum
        information and artificial intelligence, instructed by Dr. Tibra Ali.
      </p>

      <ul class="coursework-topics">
        <li>
          <strong>QI 101:</strong>
          Quantum Mechanics for Quantum Information
        </li>

        <li>
          <strong>QI 102:</strong>
          Introduction to Quantum Information
        </li>

        <li>
          <strong>AI 101:</strong>
          Artificial Intelligence and Machine Learning
        </li>
      </ul>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://drive.google.com/file/d/1qvWFZlJZtaeWtSH3YGDhBsUAbuUIPd1V/view?usp=sharing"
          target="_blank"
          rel="noopener noreferrer"
        >
          Detailed Course Outline
        </a>
      </div>
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
        Four online classes of four hours each, accompanied by graded
        assignments based on the standard QBronze educational repository.
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
        Coursework on the fundamental concepts and mathematical formulation of
        quantum mechanics using both wave-mechanical and matrix-mechanical
        approaches. The programme also included numerical and physical-system
        simulations using COMSOL.
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

  <!-- Python -->
  <div class="coursework-item">
    <div class="coursework-date">2020</div>

    <div class="coursework-content">
      <h3>Crash Course on Python</h3>

      <div class="coursework-institution">
        Google, offered through Coursera
      </div>

      <p class="coursework-description">
        Introductory programming course covering Python syntax, data
        structures, functions, loops, conditional logic, and basic programming
        practices.
      </p>

      <p class="coursework-highlight">
        Final grade: 95.50%
      </p>

      <div class="coursework-links">
        <a
          class="coursework-link"
          href="https://coursera.org/share/ac78dfb3c9f38cac40ee09c9a3188296"
          target="_blank"
          rel="noopener noreferrer"
        >
          Certificate
        </a>
      </div>
    </div>
  </div>

</div>
```
