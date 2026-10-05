<template>
  <main>
    <section class="hero-section d-flex align-items-center">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-7">
            <p class="text-primary fw-semibold mb-2">Full Stack Developer</p>

            <h1 class="display-4 fw-bold mb-4">
              Building Enterprise Business Systems with Vue 3, .NET & SQL Server
            </h1>

            <p class="lead text-secondary mb-4">
              I develop practical business applications for warehouse management,
              shipment logistics, quality workflows, inventory control, and role-based
              access systems.
            </p>

            <div class="d-flex gap-3 flex-wrap">
              <RouterLink to="/projects" class="btn btn-primary btn-lg">
                View Projects
              </RouterLink>

              <RouterLink to="/contact" class="btn btn-outline-dark btn-lg">
                Contact Me
              </RouterLink>
            </div>
          </div>

          <div class="col-lg-5 mt-5 mt-lg-0">
            <div class="card shadow-lg border-0 rounded-4">
              <div class="card-body p-4">
                <h4 class="fw-bold mb-4">Core Expertise</h4>

                <div class="expertise-item">📦 Warehouse & Inventory Management</div>
                <div class="expertise-item">🚚 Shipment & Logistics Systems</div>
                <div class="expertise-item">🧪 Batch Quality Approval Workflows</div>
                <div class="expertise-item">🔐 Role-Based Access Control</div>
                <div class="expertise-item">🗄 SQL Server Stored Procedures</div>
                <div class="expertise-item">⚡ Vue 3 + ASP.NET Core Web API</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="py-5 bg-light">
      <div class="container">
        <div class="text-center mb-5">
          <h2 class="fw-bold">Technology Stack</h2>
          <p class="text-secondary">Technologies I use to build business applications</p>
        </div>

        <div class="row g-4">
          <div class="col-md-3">
            <div class="stack-card">
              <h5>Frontend</h5>
              <p>Vue 3, Pinia, Vue Router, Bootstrap 5, Axios</p>
            </div>
          </div>

          <div class="col-md-3">
            <div class="stack-card">
              <h5>Backend</h5>
              <p>ASP.NET Core Web API, C#, Dapper</p>
            </div>
          </div>

          <div class="col-md-3">
            <div class="stack-card">
              <h5>Database</h5>
              <p>SQL Server, T-SQL, Stored Procedures</p>
            </div>
          </div>

          <div class="col-md-3">
            <div class="stack-card">
              <h5>Tools</h5>
              <p>Git, Swagger, Postman, Visual Studio</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="py-5">
      <div class="container">
        <div class="row text-center g-4">
          <div class="col-md-4">
            <h2 class="fw-bold text-primary">2+</h2>
            <p class="text-secondary">Years Experience</p>
          </div>

          <div class="col-md-4">
            <h2 class="fw-bold text-primary">20+</h2>
            <p class="text-secondary">Business Modules Worked On</p>
          </div>

          <div class="col-md-4">
            <h2 class="fw-bold text-primary">100+</h2>
            <p class="text-secondary">SQL Procedures Maintained</p>
          </div>
        </div>
      </div>
    </section>

    <section class="py-5 bg-dark text-white text-center">
      <div class="container">
        <h2 class="fw-bold mb-3">Want to see what I’ve built?</h2>
        <p class="mb-4 text-white-50">
          View my project case studies covering warehouse, logistics, QC workflow,
          and access control systems.
        </p>

        <RouterLink to="/projects" class="btn btn-light btn-lg">
          Explore Projects
        </RouterLink>
      </div>
    </section>
  </main>
</template>

<style scoped>
.hero-section {
  min-height: 85vh;
  padding: 80px 0;
}

.expertise-item {
  padding: 12px 0;
  border-bottom: 1px solid #eee;
  font-weight: 500;
}

.expertise-item:last-child {
  border-bottom: none;
}

.stack-card {
  height: 100%;
  background: white;
  border-radius: 16px;
  padding: 24px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.06);
}

.stack-card h5 {
  font-weight: 700;
  margin-bottom: 12px;
}

.stack-card p {
  color: #6c757d;
  margin-bottom: 0;
}
</style>