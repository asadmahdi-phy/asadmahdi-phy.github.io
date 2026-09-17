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
     CV ENTRIES
     ========================================================= */

  .cv-entry {
    display: grid;
    grid-template-columns: 135px 1fr;
    gap: 1.5rem;
    margin-bottom: 2.2rem;
    align-items: start;
  }

  /* Single institution image */

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

  /* Multiple institution logos */

  .cv-logo-stack {
    width: 125px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.7rem;
  }

  .cv-logo-stack .cv-institution-logo {
    width: 125px;
    height: 64px;
    object-fit: contain;
    background: white;
    border: 1px solid var(--global-divider-color);
    border-radius: 7px;
    padding: 7px;
    box-sizing: border-box;
  }

  /*
    Slightly taller logos for entries containing only two institutions,
    such as Aix-Marseille Université + CPT.
  */

  .cv-logo-stack.cv-logo-stack-two .cv-institution-logo {
    height: 72px;
  }

  /*
    Slightly more compact logos for the three NPAC universities.
  */

  .cv-logo-stack.cv-logo-stack-three .cv-institution-logo {
    height: 58px;
  }

  /* =========================================================
     ENTRY TEXT
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
    .cv-logo-stack.cv-logo-stack-two .cv-institution-logo,
    .cv-logo-stack.cv-logo-stack-three .cv-institution-logo {
      width: 110px;
      height: 58px;
    }

    .cv-two-column {
      grid-template-columns: 1fr;
    }
  }
</style>


<!-- =========================================================
     EDUCATION
     ========================================================= -->

<section class="cv-section">

  <h2 class="cv-section-title">Education</h2>


  <!-- =======================================================
       AIX-MARSEILLE UNIVERSITÉ
       ======================================================= -->

  <div class="cv-entry">

    <div
      class="cv-logo-stack cv-logo-stack-two"
      aria-label="Aix-Marseille Université and Centre de Physique Théorique"
    >

      <img
        src="{{ '/assets/img/institutions/aix-marseille-universite.png' | relative_url }}"
        alt="Aix-Marseille Université"
        class="cv-institution-logo"
        loading="lazy"
      />

      <img
        src="{{ '/assets/img/institutions/cpt.png' | relative_url }}"
        alt="Centre de Physique Théorique"
        class="cv-institution-logo"
        loading="lazy"
      />

    </div>


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

            <summary>First Semester Courses</summary>

            <ul>
              <li>General Relativity</li>
              <li>Relativistic Universe</li>
              <li>Advanced Quantum Field Theory</li>
              <li>Advanced Quantum Mechanics</li>
              <li>Galaxy and Cosmology</li>
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

    <div
      class="cv-logo-stack cv-logo-stack-three"
      aria-label="NPAC partner universities"
    >

      <img
        src="{{ '/assets/img/institutions/paris-cite.png' | relative_url }}"
        alt="Université Paris Cité"
        class="cv-institution-logo"
        loading="lazy"
      />

      <img
        src="{{ '/assets/img/institutions/paris-saclay.png' | relative_url }}"
        alt="Université Paris-Saclay"
        class="cv-institution-logo"
        loading="lazy"
      />

      <img
        src="{{ '/assets/img/institutions/sorbonne-universite.png' | relative_url }}"
        alt="Sorbonne Université"
        class="cv-institution-logo"
        loading="lazy"
      />

    </div>


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

            <summary>Relevant Coursework</summary>

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
                Particle Physics – Additional Topics
                (Symmetry Breaking, Yang–Mills Theory, and
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
       UNIVERSITY OF DHAKA — MSc
       ======================================================= -->

  <div class="cv-entry">

    <div>

      <img
        src="{{ '/assets/img/institutions/university-of-dhaka.jpg' | relative_url }}"
        alt="University of Dhaka"
        class="cv-thumbnail"
        loading="lazy"
      />

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

    </div>

  </div>


  <!-- =======================================================
       UNIVERSITY OF DHAKA — BSc
       ======================================================= -->

  <div class="cv-entry">

    <div>

      <img
        src="{{ '/assets/img/institutions/university-of-dhaka.jpg' | relative_url }}"
        alt="University of Dhaka"
        class="cv-thumbnail"
        loading="lazy"
      />

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
          Included 32 credits of practical laboratory coursework
          distributed over four years.
        </li>

        <li class="cv-details-item">

          <details>

            <summary>Relevant Undergraduate Courses</summary>

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
      />

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
      />

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
