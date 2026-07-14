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

  .cv-buttons {
    margin-top: 1.2rem;
  }

  .cv-button {
    display: inline-block;
    margin: 0.25rem;
    padding: 0.45rem 0.85rem;
    border: 1px solid var(--global-theme-color);
    border-radius: 5px;
    text-decoration: none;
  }

  .cv-button:hover {
    background-color: var(--global-theme-color);
    color: white;
    text-decoration: none;
  }

  .cv-section {
    margin-top: 2.8rem;
  }

  .cv-section-title {
    border-bottom: 2px solid var(--global-theme-color);
    padding-bottom: 0.4rem;
    margin-bottom: 1.5rem;
  }

  .cv-entry {
    display: grid;
    grid-template-columns: 130px 1fr;
    gap: 1.4rem;
    margin-bottom: 2rem;
    align-items: start;
  }

  .cv-thumbnail {
    width: 125px;
    height: 95px;
    object-fit: contain;
    background: white;
    border: 1px solid var(--global-divider-color);
    border-radius: 7px;
    padding: 7px;
  }

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

  .cv-links {
    margin-top: 0.6rem;
  }

  .cv-links a {
    margin-right: 0.8rem;
  }

  .cv-simple-entry {
    margin-bottom: 1.5rem;
  }

  .cv-simple-entry h3 {
    margin-bottom: 0.25rem;
  }

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

  @media (max-width: 700px) {
    .cv-entry {
      grid-template-columns: 1fr;
    }

    .cv-thumbnail {
      width: 115px;
      height: 85px;
    }

    .cv-two-column {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="cv-container">

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

      <a
        href="https://www.linkedin.com/in/asad-mahdi-1100b6196"
        target="_blank"
        rel="noopener noreferrer"
      >
        LinkedIn
      </a>
    </div>

    <div class="cv-buttons">
      <a
        class="cv-button"
        href="{{ '/assets/pdf/Asad_Mahdi_CV.pdf' | relative_url }}"
        target="_blank"
      >
        Download PDF CV
      </a>

      <a
        class="cv-button"
        href="mailto:asadmahdi.6.162@gmail.com"
      >
        Contact
      </a>
    </div>
  </header>


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


  <section class="cv-section">
    <h2 class="cv-section-title">Education</h2>


    <div class="cv-entry">
      <div>
        <img
          class="cv-thumbnail"
          src="{{ '/assets/img/institutions/npac.jpg' | relative_url }}"
          alt="NPAC Master's programme"
          loading="lazy"
        >
      </div>

      <div class="cv-entry-content">
        <h3>
          Master’s 2 in Nuclear, Particle, Astroparticle Physics and Cosmology
        </h3>

        <div class="cv-institution">
          Université Paris Cité, Université Paris-Saclay and Sorbonne Université
        </div>

        <div class="cv-date">
          September 2025 to Present | Paris, France
        </div>

        <ul>
          <li>
            One-year research master’s programme comprising 60 ECTS.
          </li>

          <li>
            Programme focused on high-energy physics, particle physics,
            astroparticle physics, gravity, and cosmology.
          </li>

          <li>
            Master’s internship conducted at the Laboratoire des 2 Infinis
            Toulouse, L2IT.
          </li>

          <li>
            Internship title:
            <em>
              How Do Beyond-GR Merger-Ringdown Deviations Affect the
              Inspiral Phase of Gravitational Waves?
            </em>
          </li>

          <li>
            Supervisors: Dr. Sylvain Marsat and Dr. Manuel Piarulli.
          </li>
        </ul>

        <div class="cv-links">
          <a
            href="https://drive.google.com/file/d/1Nodv42oHZDR8U--pb-If-AUu_BbXqVLB/view"
            target="_blank"
            rel="noopener noreferrer"
          >
            Transcript
          </a>

          <a
            href="https://drive.google.com/file/d/172c9MCY-9rhmV-jLKMdpx4_oxIIVNkNo/view"
            target="_blank"
            rel="noopener noreferrer"
          >
            Internship synopsis
          </a>
        </div>
      </div>
    </div>


    <div class="cv-entry">
      <div>
        <img
          class="cv-thumbnail"
          src="{{ '/assets/img/institutions/university-of-dhaka.jpg' | relative_url }}"
          alt="University of Dhaka"
          loading="lazy"
        >
      </div>

      <div class="cv-entry-content">
        <h3>Master of Science in Theoretical Physics</h3>

        <div class="cv-institution">
          University of Dhaka
        </div>

        <div class="cv-date">
          March 2023 to August 2024 | Dhaka, Bangladesh
        </div>

        <ul>
          <li>
            GPA: <strong>3.82/4.00</strong>.
          </li>

          <li>
            Ranked <strong>3rd among 18</strong> theoretical-physics students.
          </li>

          <li>
            One-year programme comprising 30 University of Dhaka credits.
          </li>

          <li>
            Thesis:
            <em>Complexity of Scalar Curvature Perturbation</em>.
          </li>

          <li>
            Thesis supervisor: Professor Tibra Ali, BRAC University.
          </li>
        </ul>

        <div class="cv-links">
          <a
            href="https://drive.google.com/file/d/10d0ccspIJDQDXKulkQYRUGRL1HdvuTjZ/view"
            target="_blank"
            rel="noopener noreferrer"
          >
            Transcript
          </a>

          <a
            href="https://drive.google.com/file/d/1wTRjZl6pP_HHo3DbtFHdXkrikcq6qNtL/view"
            target="_blank"
            rel="noopener noreferrer"
          >
            Master’s thesis
          </a>
        </div>
      </div>
    </div>


    <div class="cv-entry">
      <div>
        <img
          class="cv-thumbnail"
          src="{{ '/assets/img/institutions/university-of-dhaka.jpg' | relative_url }}"
          alt="University of Dhaka"
          loading="lazy"
        >
      </div>

      <div class="cv-entry-content">
        <h3>Bachelor of Science in Physics</h3>

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
        </ul>

        <details>
          <summary>Relevant undergraduate courses</summary>

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

        <div class="cv-links">
          <a
            href="https://drive.google.com/file/d/1lbBYl5eUg4Z1qaja3dsl0yC-QiNkyPaN/view"
            target="_blank"
            rel="noopener noreferrer"
          >
            Transcript
          </a>
        </div>
      </div>
    </div>


    <div class="cv-entry">
      <div>
        <img
          class="cv-thumbnail"
          src="{{ '/assets/img/institutions/notre-dame-college.jpg' | relative_url }}"
          alt="Notre Dame College"
          loading="lazy"
        >
      </div>

      <div class="cv-entry-content">
        <h3>Higher Secondary Certificate</h3>

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

        <div class="cv-links">
          <a
            href="https://drive.google.com/file/d/1tlpX3mFHsMxkj0pqQ7C4dd9zG0sFVlpO/view"
            target="_blank"
            rel="noopener noreferrer"
          >
            Transcript
          </a>
        </div>
      </div>
    </div>


    <div class="cv-entry">
      <div>
        <img
          class="cv-thumbnail"
          src="{{ '/assets/img/institutions/ideal-school-and-college.jpg' | relative_url }}"
          alt="Ideal School and College"
          loading="lazy"
        >
      </div>

      <div class="cv-entry-content">
        <h3>Secondary School Certificate</h3>

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

        <div class="cv-links">
          <a
            href="https://drive.google.com/file/d/1tle4A-cL4TRGEva4SLwmw2VQAicwp75e/view"
            target="_blank"
            rel="noopener noreferrer"
          >
            Transcript
          </a>
        </div>
      </div>
    </div>
  </section>


  <section class="cv-section">
    <h2 class="cv-section-title">Research Projects</h2>


    <div class="cv-entry">
      <div>
        <img
          class="cv-thumbnail"
          src="{{ '/assets/img/institutions/l2it.jpg' | relative_url }}"
          alt="L2IT Toulouse"
          loading="lazy"
        >
      </div>

      <div class="cv-entry-content">
        <h3>Testing General Relativity with Gravitational Waves</h3>

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


    <div class="cv-entry">
      <div>
        <img
          class="cv-thumbnail"
          src="{{ '/assets/img/institutions/stockholm-university.jpg' | relative_url }}"
          alt="Stockholm University"
          loading="lazy"
        >
      </div>

      <div class="cv-entry-content">
        <h3>
          Anisotropic Quenched Noise in the
          \( \phi^4 \) Model
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


    <div class="cv-entry">
      <div>
        <img
          class="cv-thumbnail"
          src="{{ '/assets/img/institutions/brac-university.jpg' | relative_url }}"
          alt="BRAC University"
          loading="lazy"
        >
      </div>

      <div class="cv-entry-content">
        <h3>Quantum Complexity in Cosmology</h3>

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


  <section class="cv-section">
    <h2 class="cv-section-title">Scholarships and Fellowships</h2>

    <div class="cv-simple-entry">
      <h3>SMARTS-UP International Mobility Fellowship</h3>

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
      <h3>National Science and Technology Fellowship</h3>

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
      <h3>General Scholarship</h3>

      <div class="cv-date">
        2023
      </div>

      <p>
        Ministry of Education, Government of Bangladesh. Merit-based
        scholarship awarded for undergraduate academic performance.
      </p>
    </div>
  </section>


  <section class="cv-section">
    <h2 class="cv-section-title">Standardized Test Scores</h2>

    <div class="cv-two-column">

      <div class="cv-info-box">
        <h3>TOEFL iBT</h3>

        <p>
          <strong>110/120</strong>
        </p>

        <ul>
          <li>Reading: 30</li>
          <li>Listening: 30</li>
          <li>Speaking: 27</li>
          <li>Writing: 23</li>
        </ul>

        <a
          href="https://drive.google.com/file/d/1S960eyKAnr5FQGjhPmM9QHzUB8hwvRcE/view"
          target="_blank"
          rel="noopener noreferrer"
        >
          Score report
        </a>
      </div>


      <div class="cv-info-box">
        <h3>GRE Physics</h3>

        <p>
          <strong>920/990</strong>
        </p>

        <p>
          85th percentile
        </p>

        <a
          href="https://drive.google.com/file/d/1jga6qc5ynaRrcDhFkubsLhUydjEJSP1g/view"
          target="_blank"
          rel="noopener noreferrer"
        >
          Score report
        </a>
      </div>


      <div class="cv-info-box">
        <h3>GRE General</h3>

        <p>
          <strong>311</strong>
        </p>

        <ul>
          <li>Quantitative Reasoning: 163</li>
          <li>Analytical Writing: 4.0</li>
        </ul>

        <a
          href="https://drive.google.com/file/d/1r_2h1lE17prYDVrvBkGee8CCc8-N0Ren/view"
          target="_blank"
          rel="noopener noreferrer"
        >
          Score report
        </a>
      </div>

    </div>
  </section>


  <section class="cv-section">
    <h2 class="cv-section-title">Computer and Research Skills</h2>

    <div class="cv-two-column">

      <div class="cv-info-box">
        <h3>Programming</h3>
        <p>Python, C, C++</p>
      </div>

      <div class="cv-info-box">
        <h3>Scientific Computing</h3>
        <p>Wolfram Mathematica, NumPy, SciPy, Matplotlib, MS Excel</p>
      </div>

      <div class="cv-info-box">
        <h3>Scientific Software</h3>
        <p>
          LALSuite, lisabeta, Qiskit, COMSOL Multiphysics, Gnuplot, Origin
        </p>
      </div>

      <div class="cv-info-box">
        <h3>Research Tools</h3>
        <p>
          LaTeX, Git, GitHub, Jupyter Notebook, Linux, SLURM
        </p>
      </div>

    </div>
  </section>


  <section class="cv-section">
    <h2 class="cv-section-title">References</h2>

    <div class="cv-simple-entry">
      <h3>Dr. Sylvain Marsat</h3>

      <p>
        CNRS Researcher<br>
        Laboratoire des 2 Infinis Toulouse, L2IT<br>
        M2 internship supervisor
      </p>

      <a href="mailto:sylvain.marsat@l2it.in2p3.fr">
        sylvain.marsat@l2it.in2p3.fr
      </a>
    </div>


    <div class="cv-simple-entry">
      <h3>Dr. Irena Nikolic</h3>

      <p>
        Université Paris Cité<br>
        NPAC Master’s programme coordinator
      </p>

      <a href="mailto:nikolic@lpnhe.in2p3.fr">
        nikolic@lpnhe.in2p3.fr
      </a>
    </div>


    <div class="cv-simple-entry">
      <h3>Dr. Cécile Roucelle</h3>

      <p>
        Université Paris Cité<br>
        NPAC Master’s programme coordinator
      </p>

      <a href="mailto:roucelle@apc.in2p3.fr">
        roucelle@apc.in2p3.fr
      </a>
    </div>
  </section>


  <section class="cv-section">
    <h2 class="cv-section-title">Interests and Activities</h2>

    <ul>
      <li>Writing literature</li>
      <li>Travelling</li>
      <li>Popularizing science</li>

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
