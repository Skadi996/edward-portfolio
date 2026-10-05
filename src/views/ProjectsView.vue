<template>
  <main class="projects-page">
    <section class="projects-hero">
      <div class="container">
        <span class="badge rounded-pill text-bg-primary px-3 py-2 mb-3">
          Projects
        </span>

        <h1 class="display-4 fw-bold mb-3">
          Enterprise systems and business modules
        </h1>

        <p class="lead text-secondary">
          Case studies from ERP and OMS-style applications built with Vue 3,
          ASP.NET Core Web API, SQL Server, stored procedures, and role-based access control.
        </p>

        <p class="portfolio-note text-secondary mt-3 mb-0">
          Selected websites and application features I contributed to during previous roles.
          These projects were developed as part of larger, company-owned systems and are
          presented here to showcase my professional experience and contributions.
        </p>
      </div>
    </section>

    <section class="projects-section">
      <div class="container">
        <div
          v-for="project in projects"
          :key="project.title"
          class="project-card mb-5"
        >
          <div class="row g-4 align-items-center">
            <div class="col-lg-5">
              <div class="screenshot-box">
                <div
                  v-for="image in project.images"
                  :key="image.src"
                  class="screenshot-thumbnail"
                  @click="openImage(image)"
                >
                  <img
                    :src="image.src"
                    :alt="image.alt"
                    class="project-image"
                  />

                  <div class="view-image">
                    <i class="bi bi-zoom-in"></i>
                    View Screenshot
                  </div>
                </div>
              </div>
            </div>

            <div class="col-lg-7">
              <p class="project-type">{{ project.type }}</p>

              <h2 class="fw-bold mb-3">
                {{ project.title }}
              </h2>

              <p class="text-secondary mb-4">
                {{ project.description }}
              </p>

              <div class="mb-4">
                <span
                  v-for="tech in project.tech"
                  :key="tech"
                  class="tech-badge"
                >
                  {{ tech }}
                </span>
              </div>

              <div class="row g-3">
                <div
                  v-for="feature in project.features"
                  :key="feature"
                  class="col-md-6"
                >
                  <div class="feature-item">
                    <i class="bi bi-check-circle-fill"></i>
                    <span>{{ feature }}</span>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="impact-box mt-4">
            <strong>Impact:</strong>
            {{ project.impact }}
          </div>
        </div>
      </div>
    </section>
    <div
      v-if="selectedImage"
      class="image-modal"
      @click.self="closeImage"
    >
      <button
        class="close-button"
        type="button"
        @click="closeImage"
      >
        &times;
      </button>

      <img
        :src="selectedImage.src"
        :alt="selectedImage.alt"
        class="large-image"
      />
    </div>
  </main>
</template>

<script setup>
import { ref } from 'vue'
import storeMaster from '../assets/StoreMaster.png'
import userAccessRight from '../assets/UserAccessRight.png'
import warehouse from '../assets/Warehouse.png'


const selectedImage = ref(null)

const openImage = (image) => {
  selectedImage.value = image
}

const closeImage = () => {
  selectedImage.value = null
}

const projects = [
  {
    icon: '📦',
    type: 'TMK OMS',
    title: 'Warehouse & Inventory Management System',
    screenshotText: 'Add screenshots: Warehouse Master, Store Transaction, Container Storage',

    images: [
    {
      src: warehouse,
      alt: 'TMK OMS Warehouse'
    }
  ],

    description:
      'Worked on warehouse and inventory modules supporting storage allocation, warehouse capacity, stock transactions, and container tracking for operational users.',
    tech: ['Vue 3', 'Bootstrap 5', 'ASP.NET Core Web API', 'C#', 'SQL Server', 'Stored Procedures'],
    features: [
      'Warehouse master maintenance',
      'Storage capacity management',
      'Stock transaction processing',
      'Container storage tracking',
      'Data-heavy operational screens',
      'SQL stored procedure integration',
    ],
    impact:
      'Improved visibility of warehouse space, inventory movement, and container-related operational data.',
  },
  {
    icon: '🚚',
    type: 'TMK OMS',
    title: 'Shipment & Logistics Management',
    screenshotText: 'Add screenshots: Sales Order Shipment Update, Weighbridge Schedule',
    description:
      'Built and maintained shipment-related modules involving sales order shipment updates, container scheduling, cargo readiness, ETA handling, and weighbridge operations.',
    tech: ['Vue 3', 'Vue Router', 'ASP.NET Core Web API', 'Dapper', 'SQL Server'],
    features: [
      'Sales order shipment update',
      'Cargo ready date validation',
      'Vessel closing date validation',
      'Weighbridge schedule tracking',
      'Container status handling',
      'ETA synchronization logic',
    ],
    impact:
      'Supported logistics users with clearer shipment status, container movement, and scheduling information.',
  },
  {
    icon: '🧪',
    type: 'TMK OMS',
    title: 'Batch Quality Approval Workflow',
    screenshotText: 'Add screenshots: Batch Approval, QC Result, COA Print',
    description:
      'Worked on quality control workflow modules involving batch registration, QC approval, rejection handling, COA printing, and approval status updates.',
    tech: ['Vue 3', 'Bootstrap 5', 'ASP.NET Core Web API', 'SQL Server', 'T-SQL'],
    features: [
      'Batch registration and update',
      'QC approval workflow',
      'Approval and rejection handling',
      'COA print support',
      'Business rule validation',
      'Approval status tracking',
    ],
    impact:
      'Helped support a structured quality approval process with traceable status updates and document output.',
  },
  {
    icon: '🔐',
    type: 'TMK OMS',
    title: 'Role-Based Access Control',
    screenshotText: 'Add screenshots: User Access Rights, Permission-Controlled Screens',
    images: [
    {
      src: userAccessRight,
      alt: 'TMK OMS User Access Rights'
    }
  ],

    description:
      'Implemented and debugged permission-based UI behavior using access rights to control viewing, editing, adding, deleting, and approval actions.',
    tech: ['Vue 3', 'Pinia', 'Vue Router', 'ASP.NET Core Web API', 'SQL Server'],
    features: [
      'User access rights management',
      'Role-based CRUD permissions',
      'Dynamic button disabling',
      'Permission-controlled workflow actions',
      'Authentication state handling',
      'Access control area validation',
    ],
    impact:
      'Improved system security by ensuring users only access actions allowed by their assigned permission group.',
  },
  {
    icon: '🏭',
    type: 'INDKOM ERP',
    title: 'ERP Operational Support & Debugging',
    screenshotText: 'Add screenshots: GRN Incoming, Purchase Order, Material Lot Search',
    description:
      'Supported ERP desktop modules involving receiving, purchase order forms, material lot searching, SQL Server permission issues, and application debugging.',
    tech: ['VB.NET', 'C#', '.NET Framework', 'WinForms', 'SQL Server'],
    features: [
      'GRN incoming process support',
      'Purchase order form debugging',
      'Material lot search implementation',
      'SQL Server permission troubleshooting',
      'Desktop application issue fixing',
      'Enterprise ERP support',
    ],
    impact:
      'Helped maintain and troubleshoot operational ERP workflows used in receiving, purchasing, and inventory-related processes.',
  },
]
</script>

<style scoped>
.projects-page {
  background: #f8fafc;
}

.projects-hero {
  padding: 90px 0 55px;
  background:
    radial-gradient(circle at top right, rgba(13, 110, 253, 0.15), transparent 35%),
    linear-gradient(135deg, #ffffff 0%, #f1f5f9 100%);
}

.projects-hero p {
  max-width: 850px;
}

.projects-section {
  padding: 70px 0;
}

.project-card {
  background: #ffffff;
  border: 1px solid #e5e7eb;
  border-radius: 30px;
  padding: 34px;
  box-shadow: 0 22px 60px rgba(15, 23, 42, 0.08);
}

.screenshot-box {
  background: #f1f5f9;
  padding: 12px;
  border-radius: 26px;
}

.screenshot-thumbnail {
  position: relative;
  cursor: pointer;
  overflow: hidden;
  border-radius: 18px;
}

.project-image {
  display: block;
  width: 100%;
  height: 220px;
  object-fit: cover;
  object-position: top;
  border-radius: 18px;
  transition: transform 0.3s ease;
}

.screenshot-thumbnail:hover .project-image {
  transform: scale(1.03);
}

.view-image {
  position: absolute;
  inset: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: rgba(0, 0, 0, 0.55);
  color: white;
  font-weight: 600;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.screenshot-thumbnail:hover .view-image {
  opacity: 1;
}

/* Full-screen image viewer */

.image-modal {
  position: fixed;
  inset: 0;
  z-index: 9999;
  background: rgba(0, 0, 0, 0.88);
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 40px;
}

.large-image {
  max-width: 95vw;
  max-height: 90vh;
  object-fit: contain;
  border-radius: 12px;
  box-shadow: 0 20px 60px rgba(0, 0, 0, 0.4);
}

.close-button {
  position: fixed;
  top: 20px;
  right: 30px;
  z-index: 10000;

  width: 45px;
  height: 45px;

  border: none;
  border-radius: 50%;

  background: rgba(255, 255, 255, 0.15);
  color: white;

  font-size: 32px;
  line-height: 1;

  cursor: pointer;
}

.close-button:hover {
  background: rgba(255, 255, 255, 0.3);
}

.placeholder-icon {
  font-size: 54px;
  margin-bottom: 16px;
}

.project-type {
  color: #0d6efd;
  font-weight: 800;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  font-size: 13px;
  margin-bottom: 8px;
}

.tech-badge {
  display: inline-block;
  background: #eef2ff;
  color: #1e3a8a;
  padding: 7px 12px;
  border-radius: 999px;
  font-size: 13px;
  font-weight: 600;
  margin: 0 8px 8px 0;
}

.feature-item {
  display: flex;
  gap: 10px;
  align-items: flex-start;
  background: #f8fafc;
  border-radius: 14px;
  padding: 12px 14px;
  height: 100%;
  color: #334155;
}

.feature-item i {
  color: #0d6efd;
  margin-top: 2px;
}

.impact-box {
  background: #f8fafc;
  border-left: 4px solid #0d6efd;
  border-radius: 14px;
  padding: 16px 20px;
  color: #475569;
}

.portfolio-note {
  max-width: 850px;
  font-size: 0.95rem;
}

@media (max-width: 768px) {
  .projects-hero {
    padding: 60px 0 40px;
  }

  .project-card {
    padding: 24px;
  }
}
</style>