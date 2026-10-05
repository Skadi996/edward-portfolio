<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-white sticky-top shadow-sm">
    <div class="container">

      <RouterLink class="navbar-brand fw-bold fs-3" to="/">
        Edward Auyong
      </RouterLink>

      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarNav">

        <ul class="navbar-nav mx-auto">

          <li class="nav-item">
            <RouterLink class="nav-link" to="/">
              Home
            </RouterLink>
          </li>

          <li class="nav-item">
            <RouterLink class="nav-link" to="/projects">
              Projects
            </RouterLink>
          </li>

        </ul>

        <div class="d-flex gap-2">
          <RouterLink
            to="/resume"
            class="btn btn-outline-dark"
          >
            Resume
          </RouterLink>
        </div>

      </div>

    </div>
  </nav>

  <RouterView />
</template>

<style>
body {
  background: #f8fafc;
}

.navbar {
  height: 80px;
}

.navbar-brand {
  letter-spacing: -0.5px;
}

.nav-link {
  font-weight: 500;
  margin: 0 10px;
  color: #334155 !important;
}

.nav-link:hover {
  color: #0d6efd !important;
}

.router-link-active {
  color: #0d6efd !important;
  font-weight: 700;
}
</style>