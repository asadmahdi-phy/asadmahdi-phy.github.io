---
layout: page
title: CV
permalink: /cv/
description: Academic curriculum vitae of Asad Mahdi
nav: true
nav_order: 5
---

<style>

  .cv-container {
    max-width: 980px;
    margin: 0 auto;
  }

  .cv-header {
    text-align: center;
    margin-bottom: 2.5rem;
  }

  .cv-header h1 {
    margin-bottom: 0.4rem;
    font-size: 2.4rem;
  }

  .cv-subtitle {
    font-size: 1.08rem;
    color: var(--global-text-color-light);
    margin-bottom: 1rem;
  }

  .cv-contact {
    line-height: 1.8;
  }

  .cv-section {
    margin-top: 2.8rem;
  }

  .cv-section-title {
    border-bottom: 2px solid var(--global-theme-color);
    padding-bottom: 0.4rem;
    margin-bottom: 1.5rem;
  }


  /* =========================================================
     MAIN CV ENTRY
     ========================================================= */

  .cv-entry {
    display: grid;
    grid-template-columns: 135px 1fr;
    gap: 1.4rem;
    margin-bottom: 2rem;
    align-items: start;
  }


  /* =========================================================
     SINGLE INSTITUTION LOGO
     ========================================================= */

  .cv-thumbnail {
    width: 125px;
    height: 95px;
    object-fit: contain;
    background: white;
    border: 1px solid var(--global-divider-color);
    border-radius: 7px;
    padding: 7px;
    box-sizing: border-box;
  }


  /* =========================================================
     MULTIPLE INSTITUTION LOGOS
     ========================================================= */

  .cv-logo-stack {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.65rem;
    width: 125px;
  }

  .cv-logo-stack .cv-institution-logo {
    width: 125px;
    height: 62px;
    object-fit: contain;
    background: white;
    border: 1px solid var(--global-divider-color);
    border-radius: 7px;
    padding: 7px;
    box-sizing: border-box;
  }


  /* AMU + CPT */

  .cv-logo-stack-two .cv-institution-logo {
    height: 72px;
  }


  /* NPAC: Paris Cité + Paris-Saclay + Sorbonne */

  .cv-logo-stack-three .cv-institution-logo {
    height: 58px;
  }


  /* =========================================================
     ENTRY CONTENT
     ========================================================= */

  .cv-entry-content h3 {
    margin-top: 0;
    margin-bottom: 0.25rem;
    font-size: 1.25rem;
  }

  .cv-institution {
    font-weight: 600;
    margin-bottom: 0.25rem;
  }

  .cv-date {
    color: var(--global-text-color-light);
    margin-bottom: 0.7rem;
  }

  .cv-entry-content ul {
    margin-top: 0.5rem;
    padding-left: 1.25rem;
  }

  .cv-entry-content li {
    margin-bottom: 0.35rem;
  }

  .cv-details-item {
    list-style: none;
    margin-left: -1.25rem;
  }


  /* =========================================================
     SIMPLE ENTRIES
     ========================================================= */

  .cv-simple-entry {
    margin-bottom: 1.5rem;
  }

  .cv-simple-entry h3 {
    margin-bottom: 0.25rem;
  }


  /* =========================================================
     TWO COLUMN BOXES
     ========================================================= */

  .cv-two-column {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1.5rem;
  }

  .cv-info-box {
    border: 1px solid var(--global-divider-color);
    border-radius: 7px;
    padding: 1.1rem;
  }

  .cv-info-box h3 {
    margin-top: 0;
  }


  /* =========================================================
     DROPDOWN SECTIONS
     ========================================================= */

  details {
    margin-top: 0.8rem;
    padding: 0.7rem 0.9rem;
    border-left: 3px solid var(--global-theme-color);
    background: var(--global-card-bg-color);
  }

  summary {
    cursor: pointer;
    font-weight: 600;
  }


  /* =========================================================
     MOBILE
     ========================================================= */

  @media (max-width: 700px) {

    .cv-entry {
      grid-template-columns: 1fr;
      gap: 1rem;
    }

    .cv-thumbnail {
      width: 115px;
      height: 85px;
    }

    .cv-logo-stack {
      width: 100%;
      flex-direction: row;
      flex-wrap: wrap;
      justify-content: flex-start;
      gap: 0.6rem;
    }

    .cv-logo-stack .cv-institution-logo,
    .cv-logo-stack-two .cv-institution-logo,
    .cv-logo-stack-three .cv-institution-logo {
      width: 110px;
      height: 58px;
    }

    .cv-two-column {
      grid-template-columns: 1fr;
    }

  }

</style>


<div class="cv-container">


<!-- =========================================================
     HEADER
     ========================================================= -->

<header class="cv-header">

  <h1>Asad Mahdi</h1>

  <div class="cv-subtitle">
    Master’s student in high-energy physics, gravity, and cosmology
  </div>

  <div class="cv-contact">

    France<br>

    <a href="mailto:asadmahdi.6.162@gmail.com">
      asadmahdi.6.162@gmail.com
    </a>

    &nbsp;|&nbsp;

    <a href="mailto:asad.mahdi@etu.u-paris.fr">
      asad.mahdi@etu.u-paris.fr
    </a>

    <br>

    LinkedIn

  </div>

</header>



<!-- =========================================================
     PROFILE
     ========================================================= -->

<section class="cv-section">

  <h2 class="cv-section-title">Profile</h2>

  <p>
    Master’s 2 student in high-energy physics and gravity, aspiring to
    pursue doctoral research in theoretical, numerical, and computational
    physics. My current interests include gravitational-wave physics,
    tests of general relativity, cosmology, quantum gravity, statistical
    physics, and renormalization-group methods.
  </p>

</section>



<!-- =========================================================
     EDUCATION
     ========================================================= -->

<section class="cv-section">

  <h2 class="cv-section-title">Education</h2>


  <!-- =======================================================
       AIX-MARSEILLE UNIVERSITÉ
       ======================================================= -->

  <div class="cv-entry">


    <!-- AMU + CPT logos -->

    <div
      class="cv-logo-stack cv-logo-stack-two"
      aria-label="Aix-Marseille Université and Centre de Physique Théorique"
    >

      <img
        src="{{ '/assets/img/institutions/aix-marseille-universite.png' | relative_url }}"
        alt="Aix-Marseille Université"
        class="cv-institution-logo"
        loading="lazy"
      >

      <img
        src="{{ '/assets/img/institutions/cpt.jpg' | relative_url }}"
        alt="Centre de Physique Théorique"
        class="cv-institution-logo"
        loading="lazy"
      >

    </div>


    <!-- AMU degree content -->

    <div class="cv-entry-content">

      <h3>
        Master’s 2 in Fundamental Physics
      </h3>

      <div class="cv-institution">
        Aix-Marseille Université | Centre de Physique Théorique (CPT)
      </div>

      <div class="cv-date">
        September 2026 to Present | Marseille, France
      </div>

      <ul>

        <li>
          Master’s 2 programme in fundamental physics comprising 60 ECTS.
        </li>

        <li>
          Pursuing advanced theoretical training in relativistic and
          fundamental physics while preparing for PhD opportunities.
        </li>

        <li class="cv-details-item">

          <details>

            <summary>
              First Semester Courses
            </summary>

            <ul>
              <li>General Relativity (Formulation, Weak Field Limit, Gravitational Waves< Black Hole Thermodynamics)</li>
              <li>Relativistic Universe (Standard Model of Cosmology, Inflation, Relativistic Perturbation Theory, Modified Gravity Predictions)</li>
              <li>Advanced Quantum Field Theory (Renormalization Group and Effective Field Theory) </li>
              <li>Advanced Quantum Mechanics (Path Integral Formalism of QM and Quantum Information Theory)</li>
              <li>Galaxy and Cosmology (Early & Late Universe, Formation of Large Scale Structure, Numerical Cosmology, Gravitational Lensing)</li>
              <li>AI and Data Science</li>
            </ul>

          </details>

        </li>

      </ul>

    </div>

  </div>



  <!-- =======================================================
       NPAC MASTER'S
       ======================================================= -->

  <div class="cv-entry">


    <!-- Three NPAC component-university logos -->

    <div
      class="cv-logo-stack cv-logo-stack-three"
      aria-label="NPAC partner universities"
    >

      <img
        src="{{ '/assets/img/institutions/paris-cite.png' | relative_url }}"
        alt="Université Paris Cité"
        class="cv-institution-logo"
        loading="lazy"
      >

      <img
        src="{{ '/assets/img/institutions/paris-saclay.png' | relative_url }}"
        alt="Université Paris-Saclay"
        class="cv-institution-logo"
        loading="lazy"
      >

      <img
        src="{{ '/assets/img/institutions/sorbonne-universite.png' | relative_url }}"
        alt="Sorbonne Université"
        class="cv-institution-logo"
        loading="lazy"
      >

    </div>


    <!-- NPAC degree content -->

    <div class="cv-entry-content">

      <h3>
        Master’s 2 in Nuclear, Particle, Astroparticle Physics and Cosmology
      </h3>

      <div class="cv-institution">
        Université Paris Cité, Université Paris-Saclay and Sorbonne Université
      </div>

      <div class="cv-date">
        September 2025 to June 2026 | Paris, France
      </div>

      <ul>

        <li>
          One-year research Master’s programme comprising 60 ECTS.
        </li>

        <li>
          Particle Physics and Cosmology stream.
        </li>

        <li class="cv-details-item">

          <details>

            <summary>
              Relevant Coursework
            </summary>

            <ul>

              <li>
                Particle Physics
                (Quantum Field Theory up to QED and the Standard Model
                of Particle Physics)
              </li>

              <li>
                Astroparticles and Cosmology
                (including a component on General Relativity)
              </li>

              <li>
                Particle Physics - Additional Topics
                (Symmetry Breaking, Yang-Mills Theory, and
                Renormalization Group Analysis)
              </li>

              <li>
                Beyond the Standard Model Physics
              </li>

              <li>
                Data Science
              </li>

            </ul>

          </details>

        </li>

      </ul>

    </div>

  </div>



  <!-- =======================================================
       UNIVERSITY OF DHAKA
       MASTER OF SCIENCE
       ======================================================= -->

  <div class="cv-entry">

    <div>

      <img
        src="{{ '/assets/img/institutions/university-of-dhaka.jpg' | relative_url }}"
        alt="University of Dhaka"
        class="cv-thumbnail"
        loading="lazy"
      >

    </div>

    <div class="cv-entry-content">

      <h3>
        Master of Science in Theoretical Physics
      </h3>

      <div class="cv-institution">
        University of Dhaka
      </div>

      <div class="cv-date">
        March 2023 to August 2024 | Dhaka, Bangladesh
      </div>

      <ul>


        <li>
          One-year programme comprising 30 DU credits.
        </li>

        <li>
          Thesis:
          <em>Complexity of Scalar Curvature Perturbation</em>.
        </li>

        <li>
          Thesis supervisor: Professor Tibra Ali, BRAC University.
        </li>

        <li class="cv-details-item">

          <details>

            <summary>
              First Semester Courses
            </summary>

            <ul>
              <li>General Relativity</li>
              <li>Condensed Matter Physics</li>
              <li>Relativistic Quantum Mechanics and Quantum Electrodynamics</li>
              <li>Introduction to Standard Model I</li>
              <li>Non-equilibrium Statistical Mechanics</li>
              <li>Quantum Mechanics</li>
            </ul>

          </details>

        </li>

      </ul>

    </div>

  </div>



  <!-- =======================================================
       UNIVERSITY OF DHAKA
       BACHELOR OF SCIENCE
       ======================================================= -->

  <div class="cv-entry">

    <div>

      <img
        src="{{ '/assets/img/institutions/university-of-dhaka.jpg' | relative_url }}"
        alt="University of Dhaka"
        class="cv-thumbnail"
        loading="lazy"
      >

    </div>

    <div class="cv-entry-content">

      <h3>
        Bachelor of Science in Physics
      </h3>

      <div class="cv-institution">
        University of Dhaka
      </div>

      <div class="cv-date">
        January 2018 to February 2023 | Dhaka, Bangladesh
      </div>

      <ul>

        <li>
          CGPA: <strong>3.78/4.00</strong>.
        </li>

        <li>
          Ranked <strong>4th among 124 graduates</strong>.
        </li>

        <li>
          Minor subjects: Mathematics and Statistics.
        </li>

        <li>
          Four-year programme comprising 136 University of Dhaka credits.
        </li>

        <li>
          Included 32 credits of practical laboratory coursework distributed
          over four years.
        </li>

        <li class="cv-details-item">

          <details>

            <summary>
              Relevant Undergraduate Courses
            </summary>

            <ul>
              <li>Quantum Mechanics I and II</li>
              <li>Classical Mechanics and Special Relativity</li>
              <li>Statistical Mechanics</li>
              <li>Electrodynamics</li>
              <li>Mathematical Physics</li>
              <li>Nuclear and Particle Physics</li>
              <li>Thermal Physics</li>
              <li>Optics</li>
              <li>Laser and Photonics</li>
              <li>Astrophysics</li>
              <li>Linear Algebra</li>
              <li>Calculus I and II</li>
              <li>Ordinary Differential Equations</li>
              <li>Probability and Statistics</li>
              <li>Numerical Analysis</li>
              <li>Computational Physics Laboratory I and II</li>
              <li>Practical Physics Laboratories</li>
            </ul>

          </details>

        </li>

      </ul>

    </div>

  </div>



  <!-- =======================================================
       NOTRE DAME COLLEGE
       ======================================================= -->

  <div class="cv-entry">

    <div>

      <img
        src="{{ '/assets/img/institutions/notre-dame-college.jpg' | relative_url }}"
        alt="Notre Dame College"
        class="cv-thumbnail"
        loading="lazy"
      >

    </div>

    <div class="cv-entry-content">

      <h3>
        Higher Secondary Certificate
      </h3>

      <div class="cv-institution">
        Notre Dame College
      </div>

      <div class="cv-date">
        2017 | Dhaka, Bangladesh
      </div>

      <ul>

        <li>
          Science group.
        </li>

        <li>
          GPA: <strong>5.00/5.00</strong>.
        </li>

      </ul>

    </div>

  </div>



  <!-- =======================================================
       IDEAL SCHOOL AND COLLEGE
       ======================================================= -->

  <div class="cv-entry">

    <div>

      <img
        src="{{ '/assets/img/institutions/ideal-school-and-college.jpg' | relative_url }}"
        alt="Ideal School and College"
        class="cv-thumbnail"
        loading="lazy"
      >

    </div>

    <div class="cv-entry-content">

      <h3>
        Secondary School Certificate
      </h3>

      <div class="cv-institution">
        Ideal School and College, Banasree Branch
      </div>

      <div class="cv-date">
        2015 | Dhaka, Bangladesh
      </div>

      <ul>

        <li>
          Science group.
        </li>

        <li>
          GPA: <strong>5.00/5.00</strong>.
        </li>

      </ul>

    </div>

  </div>

</section>



<!-- =========================================================
     RESEARCH PROJECTS
     ========================================================= -->

<section class="cv-section">

  <h2 class="cv-section-title">
    Research Projects
  </h2>



  <!-- L2IT -->

  <div class="cv-entry">

    <div>

      <img
        src="{{ '/assets/img/institutions/L2IT.jpg' | relative_url }}"
        alt="L2IT Toulouse"
        class="cv-thumbnail"
        loading="lazy"
      >

    </div>

    <div class="cv-entry-content">

      <h3>
        Testing General Relativity with Gravitational Waves
      </h3>

      <div class="cv-institution">
        Laboratoire des 2 Infinis Toulouse, L2IT
      </div>

      <div class="cv-date">
        March 2026 to July 2026 | Toulouse, France
      </div>

      <p>
        Supervisor: Dr. Sylvain Marsat
      </p>

      <ul>

        <li>
          Studying gravitational waves from compact-binary coalescences
          across the inspiral, merger, and ringdown regimes.
        </li>

        <li>
          Modelling beyond-GR deviations using post-Newtonian phase
          corrections and quasinormal-mode parametrizations.
        </li>

        <li>
          Developing data-analysis tools to investigate how deviations in
          one signal regime influence parameter recovery in another regime.
        </li>

        <li>
          Investigating gravitational-wave signals for the Laser
          Interferometer Space Antenna.
        </li>

      </ul>

    </div>

  </div>



  <!-- NORDITA -->

  <div class="cv-entry">

    <div>

      <img
        src="{{ '/assets/img/institutions/NORDITA.jpg' | relative_url }}"
        alt="NORDITA"
        class="cv-thumbnail"
        loading="lazy"
      >

    </div>

    <div class="cv-entry-content">

      <h3>
        Anisotropic Quenched Noise in the \( \phi^4 \) Model
      </h3>

      <div class="cv-institution">
        Stockholm University
      </div>

      <div class="cv-date">
        May 2026 to August 2026
      </div>

      <p>
        Supervisor: Dr. Dhrubaditya Mitra
      </p>

      <ul>

        <li>
          Studying the renormalization group of the
          \( \phi^4 \) model and evaluating its critical exponents.
        </li>

        <li>
          Investigating the effect of anisotropic quenched noise on the
          paramagnetic-to-ferromagnetic phase transition.
        </li>

        <li>
          Applying mean-field and renormalization-group methods to study
          changes in critical behaviour.
        </li>

      </ul>

    </div>

  </div>



  <!-- BRAC UNIVERSITY -->

  <div class="cv-entry">

    <div>

      <img
        src="{{ '/assets/img/institutions/bracu.jpg' | relative_url }}"
        alt="BRAC University"
        class="cv-thumbnail"
        loading="lazy"
      >

    </div>

    <div class="cv-entry-content">

      <h3>
        Quantum Complexity in Cosmology
      </h3>

      <div class="cv-institution">
        BRAC University
      </div>

      <div class="cv-date">
        June 2024 to Present
      </div>

      <p>
        Supervisor: Professor Tibra Ali
      </p>

      <ul>

        <li>
          Studying quantum complexity for scalar curvature perturbations
          using the squeezed-state formalism.
        </li>

        <li>
          Considering perturbations around a
          Friedmann-Lemaître-Robertson-Walker cosmological background.
        </li>

        <li>
          Investigating possible connections between quantum complexity,
          cosmological perturbations, and gravitational entropy.
        </li>

      </ul>

    </div>

  </div>

</section>



<!-- =========================================================
     SCHOLARSHIPS AND FELLOWSHIPS
     ========================================================= -->

<section class="cv-section">

  <h2 class="cv-section-title">
    Scholarships and Fellowships
  </h2>


  <div class="cv-simple-entry">

    <h3>
      SMARTS-UP International Mobility Fellowship
    </h3>

    <div class="cv-date">
      2025 to 2026
    </div>

    <p>
      Université Paris Cité and the French National Research Agency.
      A one-year international mobility grant supporting master’s studies
      and residence in France.
    </p>

  </div>


  <div class="cv-simple-entry">

    <h3>
      National Science and Technology Fellowship
    </h3>

    <div class="cv-date">
      2023
    </div>

    <p>
      Ministry of Science and Technology, Government of Bangladesh.
      Awarded with a research grant for the master’s thesis on the basis
      of academic performance in the bachelor’s programme.
    </p>

  </div>


  <div class="cv-simple-entry">

    <h3>
      General Scholarship
    </h3>

    <div class="cv-date">
      2023
    </div>

    <p>
      Ministry of Education, Government of Bangladesh. Merit-based
      scholarship awarded for undergraduate academic performance.
    </p>

  </div>

</section>



<!-- =========================================================
     STANDARDIZED TEST SCORES
     ========================================================= -->

<section class="cv-section">

  <h2 class="cv-section-title">
    Standardized Test Scores
  </h2>

  <div class="cv-two-column">


    <!-- TOEFL -->

    <div class="cv-info-box">

      <h3>
        TOEFL iBT
      </h3>

      <p>
        <strong>110/120</strong>
      </p>

      <ul>
        <li>Reading: 30</li>
        <li>Listening: 30</li>
        <li>Speaking: 27</li>
        <li>Writing: 23</li>
      </ul>

      Score report

    </div>


    <!-- GRE PHYSICS -->

    <div class="cv-info-box">

      <h3>
        GRE Physics
      </h3>

      <p>
        <strong>920/990</strong>
      </p>

      <p>
        85th percentile
      </p>

      Score report

    </div>


    <!-- GRE GENERAL -->

    <div class="cv-info-box">

      <h3>
        GRE General
      </h3>

      <p>
        <strong>311</strong>
      </p>

      <ul>
        <li>Quantitative Reasoning: 163</li>
        <li>Analytical Writing: 4.0</li>
      </ul>

      Score report

    </div>

  </div>

</section>



<!-- =========================================================
     COMPUTER AND RESEARCH SKILLS
     ========================================================= -->

<section class="cv-section">

  <h2 class="cv-section-title">
    Computer and Research Skills
  </h2>

  <div class="cv-two-column">


    <div class="cv-info-box">

      <h3>
        Programming
      </h3>

      <p>
        Python, C, C++
      </p>

    </div>


    <div class="cv-info-box">

      <h3>
        Scientific Computing
      </h3>

      <p>
        Wolfram Mathematica, NumPy, SciPy, Matplotlib, MS Excel
      </p>

    </div>


    <div class="cv-info-box">

      <h3>
        Scientific Software
      </h3>

      <p>
        LALSuite, lisabeta, Qiskit, COMSOL Multiphysics, Gnuplot, Origin
      </p>

    </div>


    <div class="cv-info-box">

      <h3>
        Research Tools
      </h3>

      <p>
        LaTeX, Git, GitHub, Jupyter Notebook, Linux, SLURM
      </p>

    </div>

  </div>

</section>



<!-- =========================================================
     REFERENCES
     ========================================================= -->

<section class="cv-section">

  <h2 class="cv-section-title">
    References
  </h2>


  <!-- SYLVAIN MARSAT -->

  <div class="cv-simple-entry">

    <h3>
      Dr. Sylvain Marsat
    </h3>

    <p>
      CNRS Researcher<br>
      Laboratoire des 2 Infinis Toulouse, L2IT<br>
      M2 internship supervisor
    </p>

    <a href="mailto:sylvain.marsat@l2it.in2p3.fr">
      sylvain.marsat@l2it.in2p3.fr
    </a>

  </div>


  <!-- DHRUBADITYA MITRA -->

  <div class="cv-simple-entry">

    <h3>
      Dr. Dhrubaditya Mitra
    </h3>

    <p>
      Assistant Professor<br>
      Stockholm University and Nordic Institute of Theoretical Physics<br>
      NORDITA summer internship supervisor
    </p>

    <a href="mailto:dhrubaditya.mitra@su.se">
      dhrubaditya.mitra@su.se
    </a>

  </div>


  <!-- IRENA NIKOLIC -->

  <div class="cv-simple-entry">

    <h3>
      Dr. Irena Nikolic
    </h3>

    <p>
      Université Paris Cité<br>
      NPAC Master’s programme coordinator
    </p>

    <a href="mailto:nikolic@lpnhe.in2p3.fr">
      nikolic@lpnhe.in2p3.fr
    </a>

  </div>


  <!-- CÉCILE ROUCELLE -->

  <div class="cv-simple-entry">

    <h3>
      Dr. Cécile Roucelle
    </h3>

    <p>
      Université Paris Cité<br>
      NPAC Master’s programme coordinator
    </p>

    <a href="mailto:roucelle@apc.in2p3.fr">
      roucelle@apc.in2p3.fr
    </a>

  </div>

</section>



<!-- =========================================================
     INTERESTS AND ACTIVITIES
     ========================================================= -->

<section class="cv-section">

  <h2 class="cv-section-title">
    Interests and Activities
  </h2>

  <ul>

    <li>
      Writing literature
    </li>

    <li>
      Travelling
    </li>

    <li>
      Popularizing science
    </li>

    <li>
      Debater at Ideal Debating Club from January 2011 to May 2015.
    </li>

    <li>
      Participant and award winner in national debate competitions.
    </li>

    <li>
      Volunteer in activities promoting debating among school students.
    </li>

    <li>
      Academic volunteer and examiner at the Bangladesh Physics Olympiad
      in 2023.
    </li>

  </ul>

</section>


</div>
