# Mobitrendz Enterprise Full-Stack Templates

Welcome to the Mobitrendz open-source hub. This page highlights our evolving, enterprise-grade templates optimized for 2026 industry standards [1, 2].

## [FastAPI AI-Optimized Enterprise Backend Template](https://github.com/mobitrendz/fastapi-backend-template)
This backend provides a layered modular architecture designed for high performance and AI-driven development [1, 3, 4].
* **Tech Stack**: It leverages Python 3.12+, FastAPI, SQLModel, and PostgreSQL 18 [4, 5].
* **Security & Observability**: It implements a robust Role-Based Access Control (RBAC) system, structured JSON logging with Structlog, real-time metrics with Prometheus, and automated security scanning [4-6].
* **Developer Workflows**: The template is fully integrated with `uv` for fast dependency management, Docker health checks, and Alembic for robust schema migrations [4, 5, 7].
* **Live Documentation**: Deep-dive architecture and deployment guides are generated via Zensical and hosted at `https://mobitrendz.github.io/fastapi-backend-template/` [8].

## [React 19 + FastAPI Frontend Template](https://github.com/mobitrendz/react-frontend-template)
This template is a modern companion frontend pre-configured to consume the FastAPI backend [2, 4].
* **Tech Stack**: It is built with React 19 (TypeScript), Vite 8, Tailwind CSS 4, and the shadcn/ui framework [2, 9].
* **Data & Orchestration**: It features a contract-first, type-safe SDK generated from the backend's OpenAPI schema using `@hey-api/openapi-ts`, orchestrated by TanStack Query for automatic caching and background revalidation [9, 10].
* **Features**: The frontend includes secure JWT authentication, multi-page architecture with React Router 7, adaptive dark mode, and a powerful admin dashboard for user lifecycle management [11, 12].
* **Quality Assurance**: System reliability is enforced with over 92% statement test coverage via Vitest, alongside automated CI/CD API sync checks that prevent broken contracts from reaching production [13-15].
