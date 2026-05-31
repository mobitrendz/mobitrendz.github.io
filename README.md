# MobiTrendz

**Live site:** [https://mobitrendz.github.io](https://mobitrendz.github.io)

MobiTrendz is an information services initiative dedicated to creating and sharing enterprise-grade, open-source templates, applications, and digital resources. Our mission is to empower developers, organizations, and communities by providing accessible, high-quality tools that foster innovation, collaboration, and digital inclusion.

Through open-source solutions and knowledge-sharing, MobiTrendz aims to make technology more accessible to the public while supporting sustainable and community-driven development.

This repository hosts the static landing page for the MobiTrendz GitHub Pages site.

---

## Open-Source Templates

Our evolving, enterprise-grade templates are optimized for 2026 industry standards.

### [FastAPI AI-Optimized Enterprise Backend Template](https://github.com/mobitrendz/fastapi-backend-template)

A layered modular architecture designed for high performance and AI-driven development.

- **Tech Stack:** Python 3.12+, FastAPI, SQLModel, PostgreSQL 18
- **Security & Observability:** RBAC, Structlog JSON logging, Prometheus metrics, automated security scanning
- **Developer Workflows:** `uv` dependency management, Docker health checks, Alembic migrations
- **Documentation:** [https://mobitrendz.github.io/fastapi-backend-template/](https://mobitrendz.github.io/fastapi-backend-template/)

### [React 19 + FastAPI Frontend Template](https://github.com/mobitrendz/react-frontend-template)

A modern companion frontend pre-configured to consume the FastAPI backend.

- **Tech Stack:** React 19 (TypeScript), Vite 8, Tailwind CSS 4, shadcn/ui
- **Data & Orchestration:** Contract-first SDK via `@hey-api/openapi-ts`, TanStack Query caching
- **Features:** JWT authentication, React Router 7, adaptive dark mode, admin dashboard
- **Quality Assurance:** 92%+ statement test coverage (Vitest), automated CI/CD API sync checks

### [Expo Mobile App Template](https://github.com/mobitrendz/expo-mobile-template)

A React Native mobile app built with Expo SDK 54 that connects to the FastAPI backend.

- **Tech Stack:** Expo SDK 54, React Native, React 19, TypeScript
- **Features:** JWT authentication, full-featured task manager, profile management
- **API Integration:** Auto-generated type-safe client from OpenAPI specification

---

## Repository Structure

```
mobitrendz.github.io/
├── index.html          # Landing page
├── css/styles.css      # Site styles
├── assets/             # Logo and banner images
├── ref/                # Reference READMEs and brand assets
└── .nojekyll           # Bypass Jekyll processing on GitHub Pages
```

---

## Local Development

No build step is required. Serve the site locally with any static file server:

```bash
# Python
python3 -m http.server 8080

# Node.js (npx)
npx serve .
```

Then open [http://localhost:8080](http://localhost:8080).

---

## GitHub Pages Deployment

This repo is configured as a user/organization GitHub Pages site. To deploy:

1. Push changes to the `main` branch.
2. In **Settings → Pages**, set the source to **Deploy from branch** → `main` → `/ (root)`.
3. The site will be published at [https://mobitrendz.github.io](https://mobitrendz.github.io).

---

## Links

- **Website:** [https://mobitrendz.github.io](https://mobitrendz.github.io)
- **GitHub Organization:** [https://github.com/mobitrendz](https://github.com/mobitrendz)
