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

### [The Ghost Letters](https://theghostletters.org/)

An interactive essay on how English silent letters — from Caxton’s Flemish typesetters to Renaissance etymological vanity — quietly inflate print volume into a compounding ecological cost.

- **Thesis:** Silent characters (roughly 5% of printed English) carry real timber, water, ink, and carbon overhead at global publishing scale
- **History:** Traces ghost letters through Caxton’s 1476 press, Flemish compositor conventions, and Latinate spelling reforms
- **Impact:** Estimates ~1.6 million trees pulped annually solely for letters that make no sound
- **Paths Forward:** Leaner orthography, eco-efficient typefaces, and recycled fiber in mass-market publishing
- **Website:** [https://theghostletters.org/](https://theghostletters.org/)

### [AI Continuum](https://aicontinuum.mobitrendz.com/)

A comprehensive AI reference hub (not an open-source template) that organizes core AI knowledge across historical eras, model families, tools, developer libraries, key figures, research labs, and future concepts.

- **Website:** [https://aicontinuum.mobitrendz.com/](https://aicontinuum.mobitrendz.com/)

---

## Applications

### [DraftAI](https://github.com/mobitrendz/DraftAI)

A smart content assistant for developers and tech writers. Turn a single topic or prompt into a full-length DEV.to technical article, LinkedIn post, and matching cover image — then review, schedule, and publish.

- **Monorepo Architecture:** FastAPI backend + ARQ background worker, PostgreSQL, Redis, React 19 + Vite dashboard (built on MobiTrendz enterprise templates)
- **Multi-Platform AI Generation:** Automated generation of technical DEV.to Markdown articles and LinkedIn posts from one prompt
- **AI Cover Images:** Synchronous AI-generated cover images with persistent object storage
- **Interactive Review Editor:** Split-view Markdown editor with live formatting, cover image management, and manual editing
- **Staggered Publishing & Scheduling:** Automated publishing queue that publishes DEV.to first, captures live URL, injects it into LinkedIn post text, and publishes (with copy-to-clipboard fallback)
- **Multi-Tenant Security:** Per-user Fernet-encrypted BYOK (Bring Your Own Keys) credentials for LLM providers (OpenAI, Anthropic) and publishing platforms
- **Repository:** [https://github.com/mobitrendz/DraftAI](https://github.com/mobitrendz/DraftAI)

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

- **Website:** [https://mobitrendz.com/](https://mobitrendz.com/)
- **GitHub Organization:** [https://github.com/mobitrendz](https://github.com/mobitrendz)
