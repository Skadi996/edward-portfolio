<template>
  <main class="resume-page">

    <!-- Hero -->
    <section class="resume-hero">
      <div class="container">

        <span class="badge rounded-pill text-bg-primary px-3 py-2 mb-3">
          Resume
        </span>

        <div class="d-flex flex-column flex-lg-row justify-content-between align-items-lg-end gap-4">

          <div>
            <h1 class="display-4 fw-bold mb-3">
              Edward Au Yong
            </h1>

            <p class="hero-role mb-3">
              Full Stack Developer
            </p>

            <div class="contact-list">
              <span>
                <i class="bi bi-envelope"></i>
                edward.aysk@gmail.com
              </span>

              <span>
                <i class="bi bi-telephone"></i>
                0433 739 589
              </span>

              <span>
                <i class="bi bi-geo-alt"></i>
                Craigieburn, VIC
              </span>
            </div>
          </div>

          <div class="resume-actions">
            <a
              href="https://www.linkedin.com/in/edward-au-yong-a7600a266/"
              target="_blank"
              rel="noopener noreferrer"
              class="btn btn-outline-dark"
            >
              <i class="bi bi-linkedin me-2"></i>
              LinkedIn
            </a>

            <a
            href="/Edward-Auyong-Resume.pdf"
            download
            class="btn btn-primary"
            >
            <i class="bi bi-download me-2"></i>
            Download PDF Resume
            </a>
          </div>

        </div>

      </div>
    </section>


    <!-- Resume Content -->
    <section class="resume-section">
      <div class="container">

        <div class="row g-5">

          <!-- Main Column -->
          <div class="col-lg-8">

            <!-- Professional Summary -->
            <section class="resume-block">
              <div class="section-heading">
                <span class="section-number">01</span>
                <h2>Professional Summary</h2>
              </div>

              <p class="summary-text">
                Experienced Full Stack Developer skilled in .NET, MS SQL,
                Vue.js, and API integration, with a track record of delivering
                end-to-end web applications for streamlined business operations.
                Adept at translating business needs into custom enterprise
                software including MRP, POS, and logistics systems, optimizing
                complex database performance by 40–60%, and developing responsive
                frontends integrated with robust backend architectures.
              </p>
            </section>


            <!-- Professional Experience -->
            <section class="resume-block">

              <div class="section-heading">
                <span class="section-number">02</span>
                <h2>Professional Experience</h2>
              </div>


              <!-- Freelance -->
              <article class="experience-item">

                <div class="experience-header">

                  <div>
                    <h3>Full Stack Developer</h3>

                    <p class="company">
                      Self-employed · Freelance
                    </p>
                  </div>

                  <span class="date">
                    March 2024 – Present
                  </span>

                </div>

                <ul class="experience-list">

                  <li>
                    <strong>Enterprise Solutions:</strong>
                    Support custom enterprise systems including MRP, POS,
                    QC Audit, Issue Tracker, and Shipping Logistics platforms
                    for small to medium enterprise clients to automate
                    business operations.
                  </li>

                  <li>
                    <strong>Full-Stack Engineering:</strong>
                    Build responsive frontend user interfaces using Vue.js,
                    Bootstrap, and jQuery, integrated with .NET Web APIs
                    for reliable data flow and workflow efficiency.
                  </li>

                  <li>
                    <strong>Database Management:</strong>
                    Structure and maintain MS SQL databases, designing
                    schemas and stored procedures to ensure backend stability
                    and query efficiency.
                  </li>

                  <li>
                    <strong>Quality &amp; Optimization:</strong>
                    Perform system UI/UX refinements, API integration testing,
                    and bug fixing to improve software performance and
                    end-user adoption.
                  </li>

                </ul>

                <div class="experience-tech">
                  <span>.NET</span>
                  <span>Vue.js</span>
                  <span>JavaScript</span>
                  <span>jQuery</span>
                  <span>Bootstrap</span>
                  <span>MS SQL</span>
                  <span>REST APIs</span>
                </div>

              </article>


              <!-- JME -->
              <article class="experience-item">

                <div class="experience-header">

                  <div>
                    <h3>SQL Developer</h3>

                    <p class="company">
                      JME Technology (WA) Pty Ltd
                    </p>
                  </div>

                  <span class="date">
                    Jan 2018 – Jul 2018
                  </span>

                </div>

                <ul class="experience-list">

                  <li>
                    <strong>Query Optimization:</strong>
                    Authored and tuned complex T-SQL scripts to diagnose
                    slow-running database operations, achieving a
                    40–60% reduction in key query execution times.
                  </li>

                  <li>
                    <strong>Data Governance:</strong>
                    Collaborated on developing data governance frameworks,
                    reducing reporting errors and enhancing business data
                    reliability for stakeholders.
                  </li>

                </ul>

                <div class="experience-tech">
                  <span>SQL Server</span>
                  <span>T-SQL</span>
                  <span>Query Optimization</span>
                  <span>Data Governance</span>
                </div>

              </article>

            </section>


            <!-- Education -->
            <section class="resume-block">

              <div class="section-heading">
                <span class="section-number">03</span>
                <h2>Education</h2>
              </div>

              <article class="education-item">

                <div class="education-icon">
                  <i class="bi bi-mortarboard-fill"></i>
                </div>

                <div>
                  <h3>Bachelor of Information Technology</h3>

                  <p class="company">
                    RMIT University
                  </p>

                  <span class="date">
                    Graduated 2023
                  </span>
                </div>

              </article>


              <article class="education-item">

                <div class="education-icon">
                  <i class="bi bi-mortarboard"></i>
                </div>

                <div>
                  <h3>Diploma of Information Technology</h3>

                  <p class="company">
                    RMIT University
                  </p>

                  <span class="date">
                    Graduated 2017
                  </span>
                </div>

              </article>

            </section>

          </div>


          <!-- Sidebar -->
          <div class="col-lg-4">

            <aside class="resume-sidebar">

              <!-- Technical Skills -->
              <section class="sidebar-card">

                <div class="sidebar-heading">
                  <i class="bi bi-code-slash"></i>
                  <h2>Technical Skills</h2>
                </div>


                <div class="skill-group">

                  <h3>Backend Development</h3>

                  <div class="skill-tags">
                    <span>.NET Web API</span>
                    <span>.NET Framework</span>
                    <span>VB</span>
                    <span>RESTful APIs</span>
                  </div>

                </div>


                <div class="skill-group">

                  <h3>Frontend Development</h3>

                  <div class="skill-tags">
                    <span>Vue.js</span>
                    <span>JavaScript</span>
                    <span>jQuery</span>
                    <span>Bootstrap</span>
                    <span>HTML</span>
                    <span>CSS</span>
                  </div>

                </div>


                <div class="skill-group">

                  <h3>Database &amp; Architecture</h3>

                  <div class="skill-tags">
                    <span>MS SQL</span>
                    <span>T-SQL</span>
                    <span>Database Design</span>
                    <span>Stored Procedures</span>
                    <span>Schema Optimization</span>
                  </div>

                </div>


                <div class="skill-group">

                  <h3>Tools &amp; Methodologies</h3>

                  <div class="skill-tags">
                    <span>Git</span>
                    <span>UI/UX Design</span>
                    <span>Testing</span>
                    <span>Debugging</span>
                    <span>Performance Optimization</span>
                    <span>Data Governance</span>
                  </div>

                </div>

              </section>


              <!-- Core Strengths -->
              <section class="sidebar-card">

                <div class="sidebar-heading">
                  <i class="bi bi-stars"></i>
                  <h2>Core Strengths</h2>
                </div>

                <ul class="strength-list">
                  <li>
                    <i class="bi bi-check-circle-fill"></i>
                    Full-stack web development
                  </li>

                  <li>
                    <i class="bi bi-check-circle-fill"></i>
                    Enterprise application development
                  </li>

                  <li>
                    <i class="bi bi-check-circle-fill"></i>
                    SQL performance optimization
                  </li>

                  <li>
                    <i class="bi bi-check-circle-fill"></i>
                    API integration
                  </li>

                  <li>
                    <i class="bi bi-check-circle-fill"></i>
                    UI/UX refinement
                  </li>

                  <li>
                    <i class="bi bi-check-circle-fill"></i>
                    Testing and debugging
                  </li>
                </ul>

              </section>

            </aside>

          </div>

        </div>

      </div>
    </section>

  </main>
</template>


<style scoped>

.resume-page {
  background: #f8fafc;
  min-height: 100vh;
}


/* Hero */

.resume-hero {
  padding: 80px 0 65px;

  background:
    radial-gradient(
      circle at top right,
      rgba(13, 110, 253, 0.15),
      transparent 35%
    ),
    linear-gradient(
      135deg,
      #ffffff 0%,
      #f1f5f9 100%
    );
}

.resume-hero h1 {
  letter-spacing: -1.5px;
}

.hero-role {
  font-size: 1.35rem;
  font-weight: 600;
  color: #475569;
}

.contact-list {
  display: flex;
  flex-wrap: wrap;
  gap: 18px;
  color: #64748b;
  font-size: 0.95rem;
}

.contact-list span {
  display: inline-flex;
  align-items: center;
  gap: 7px;
}

.contact-list i {
  color: #0d6efd;
}

.resume-actions {
  display: flex;
  gap: 10px;
}


/* Main Section */

.resume-section {
  padding: 70px 0;
}


/* Section headings */

.resume-block {
  margin-bottom: 70px;
}

.section-heading {
  display: flex;
  align-items: center;
  gap: 14px;
  margin-bottom: 30px;
}

.section-heading h2 {
  margin: 0;
  font-size: 1.65rem;
  font-weight: 800;
  letter-spacing: -0.5px;
}

.section-number {
  display: inline-flex;
  align-items: center;
  justify-content: center;

  width: 38px;
  height: 38px;

  border-radius: 12px;

  background: #e8f1ff;
  color: #0d6efd;

  font-size: 0.8rem;
  font-weight: 800;
}


/* Summary */

.summary-text {
  font-size: 1.08rem;
  line-height: 1.85;
  color: #475569;
}


/* Experience */

.experience-item {
  position: relative;

  padding: 0 0 40px;
  margin-bottom: 40px;

  border-bottom: 1px solid #e2e8f0;
}

.experience-item:last-child {
  border-bottom: none;
  margin-bottom: 0;
}

.experience-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 20px;

  margin-bottom: 22px;
}

.experience-header h3 {
  font-size: 1.25rem;
  font-weight: 750;
  margin-bottom: 6px;
}

.company {
  color: #0d6efd;
  font-weight: 600;
  margin-bottom: 0;
}

.date {
  flex-shrink: 0;

  padding: 6px 12px;

  border-radius: 999px;

  background: #f1f5f9;
  color: #64748b;

  font-size: 0.85rem;
  font-weight: 600;
}

.experience-list {
  padding-left: 20px;
  margin-bottom: 25px;
}

.experience-list li {
  color: #475569;
  line-height: 1.75;
  margin-bottom: 13px;
  padding-left: 5px;
}

.experience-list li::marker {
  color: #0d6efd;
}

.experience-tech {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.experience-tech span {
  padding: 6px 11px;

  background: #eef2ff;
  color: #1e3a8a;

  border-radius: 999px;

  font-size: 0.78rem;
  font-weight: 650;
}


/* Education */

.education-item {
  display: flex;
  gap: 18px;

  padding: 20px;

  background: #ffffff;

  border: 1px solid #e5e7eb;
  border-radius: 18px;

  margin-bottom: 15px;
}

.education-icon {
  display: flex;
  align-items: center;
  justify-content: center;

  flex-shrink: 0;

  width: 45px;
  height: 45px;

  border-radius: 13px;

  background: #e8f1ff;
  color: #0d6efd;

  font-size: 1.2rem;
}

.education-item h3 {
  font-size: 1.05rem;
  font-weight: 700;
  margin-bottom: 5px;
}


/* Sidebar */

.resume-sidebar {
  position: sticky;
  top: 105px;
}

.sidebar-card {
  background: #ffffff;

  border: 1px solid #e5e7eb;
  border-radius: 24px;

  padding: 28px;

  margin-bottom: 20px;

  box-shadow: 0 15px 40px rgba(15, 23, 42, 0.05);
}

.sidebar-heading {
  display: flex;
  align-items: center;
  gap: 10px;

  margin-bottom: 25px;
}

.sidebar-heading i {
  color: #0d6efd;
  font-size: 1.15rem;
}

.sidebar-heading h2 {
  margin: 0;

  font-size: 1.2rem;
  font-weight: 800;
}


/* Skills */

.skill-group {
  margin-bottom: 25px;
}

.skill-group:last-child {
  margin-bottom: 0;
}

.skill-group h3 {
  font-size: 0.85rem;
  font-weight: 750;
  color: #475569;

  margin-bottom: 10px;
}

.skill-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 7px;
}

.skill-tags span {
  padding: 6px 10px;

  background: #f8fafc;
  border: 1px solid #e2e8f0;

  border-radius: 8px;

  color: #334155;

  font-size: 0.78rem;
  font-weight: 600;
}


/* Strengths */

.strength-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.strength-list li {
  display: flex;
  align-items: flex-start;
  gap: 10px;

  color: #475569;

  font-size: 0.9rem;
  line-height: 1.5;

  margin-bottom: 13px;
}

.strength-list li:last-child {
  margin-bottom: 0;
}

.strength-list i {
  color: #0d6efd;
  margin-top: 3px;
}


/* CTA */

.sidebar-cta {
  padding: 30px;

  border-radius: 24px;

  background:
    linear-gradient(
      135deg,
      #0d6efd,
      #2563eb
    );

  color: #ffffff;

  box-shadow: 0 20px 45px rgba(13, 110, 253, 0.2);
}

.sidebar-cta > i {
  font-size: 2rem;
  opacity: 0.9;
}

.sidebar-cta h2 {
  font-size: 1.25rem;
  font-weight: 800;
  margin: 18px 0 10px;
}

.sidebar-cta p {
  color: rgba(255, 255, 255, 0.85);
  line-height: 1.65;
  font-size: 0.9rem;
  margin-bottom: 20px;
}


/* Responsive */

@media (max-width: 991px) {

  .resume-sidebar {
    position: static;
  }

}

@media (max-width: 768px) {

  .resume-hero {
    padding: 60px 0 45px;
  }

  .resume-section {
    padding: 50px 0;
  }

  .resume-actions {
    width: 100%;
  }

  .resume-actions .btn {
    flex: 1;
  }

  .experience-header {
    flex-direction: column;
    gap: 10px;
  }

  .contact-list {
    flex-direction: column;
    gap: 8px;
  }

  .resume-block {
    margin-bottom: 50px;
  }

}

</style>