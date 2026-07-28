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
- **Quality Assurance:** 92.66% statement test coverage (Vitest), automated CI/CD API sync checks
- **Documentation:** [https://mobitrendz.github.io/react-frontend-template/](https://mobitrendz.github.io/react-frontend-template/) (Docusaurus)

### [Expo Mobile App Template](https://github.com/mobitrendz/expo-mobile-template)

Part of the MobiTrendz starter kit — a React Native app (Expo SDK 54) connected to the FastAPI backend.

- **Tech Stack:** Expo SDK 54, React Native 0.81, React 19, TypeScript
- **Features:** JWT authentication, task manager with platform-aware date pickers, profile management
- **API Integration:** Auto-generated type-safe client from OpenAPI specification
- **Documentation:** [https://mobitrendz.github.io/expo-mobile-template/](https://mobitrendz.github.io/expo-mobile-template/) (Docusaurus)

---

## Knowledge Hub

### [AI Continuum](https://aicontinuum.mobitrendz.com/)

A comprehensive AI reference hub (not an open-source template) that organizes core AI knowledge across historical eras, model families, tools, developer libraries, key figures, research labs, and future concepts.

- **Website:** [https://aicontinuum.mobitrendz.com/](https://aicontinuum.mobitrendz.com/)

---

## Applications

### [Digital Dietitian](https://digidiet.mobitrendz.com/)

An evidence-based nutrition planning application that generates structured dietary guidance using biometric inputs, activity levels, and clinical condition toggles.

- **Core Engine:** Mifflin-St Jeor calorie computation with activity multipliers and baseline fallbacks
- **Clinical Protocols:** Hypertension, celiac disease, diabetes, pregnancy, and lactation adjustments
- **Output Modes:** Dashboard view plus exportable structured JSON nutrient report
- **Architecture:** Gemini 3.5 Flash integration with deterministic local fallback support
- **Website:** [https://digidiet.mobitrendz.com/](https://digidiet.mobitrendz.com/)

### [108 Drigganita Music](https://astromusic.mobitrendz.com/)

A Vedic astronomy and spiritual music application that combines Drik-ganita sidereal calculations with Sahasranama, Keerthana, and Bhajana playback.

- **Astronomy Engine:** Live Nirayana Gochara transit chart and Drik-ganita Jathakam birth-chart calculation
- **Muhurta Timing:** Daily day/night Muhurta explorer with deity mappings and location-aware sidereal timekeeping
- **Music Player:** Archival playlist recommendations aligned to active Gochara and Muhurta influences
- **Languages:** English, Malayalam, and Telugu
- **Website:** [https://astromusic.mobitrendz.com/](https://astromusic.mobitrendz.com/)
- **Repository:** [https://github.com/mobitrendz/astromusic](https://github.com/mobitrendz/astromusic)

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

## Documentation

| Template | Docs URL | Generator |
|----------|----------|-----------|
| FastAPI Backend | [mobitrendz.github.io/fastapi-backend-template](https://mobitrendz.github.io/fastapi-backend-template/) | Zensical |
| React Frontend | [mobitrendz.github.io/react-frontend-template](https://mobitrendz.github.io/react-frontend-template/) | Docusaurus |
| Expo Mobile | [mobitrendz.github.io/expo-mobile-template](https://mobitrendz.github.io/expo-mobile-template/) | Docusaurus |

## Links

- **Website:** [https://mobitrendz.github.io](https://mobitrendz.github.io)
- **GitHub Organization:** [https://github.com/mobitrendz](https://github.com/mobitrendz)
