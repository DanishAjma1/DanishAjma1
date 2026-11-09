# 👨‍💻 Danish Ajmal
### Full-Stack Systems Engineer · TypeScript | Next.js | Node.js | Distributed Systems

<p align="center">
  <a href="https://danishajma1.github.io/Portfolio/"><img src="https://img.shields.io/badge/Portfolio-Live_Site-000000?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/danish-ajmal-butt"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:danishajmalbutt@gmail.com"><img src="https://img.shields.io/badge/Email-Contact_Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Location-Punjab,_Pakistan-4682B4?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Location" />
</p>
<br/>

> **Software Engineer** specializing in full-stack architecture, high-concurrency Node.js/TypeScript distributed systems, Next.js SSR applications, and multi-tenant platforms. Experienced in architecting production solutions spanning Redis pub/sub WebSocket clusters, WebRTC media streaming, relational & document data modeling (PostgreSQL, MongoDB), and generative AI workflows.

---

## 🏛️ End-to-End Systems Engineering Blueprint

```mermaid
flowchart TD
    subgraph ClientPerimeter ["Client & Presentation Tier"]
        SSR["Next.js 15/16 App Router (SSR / Edge)"]
        PWA["React 18/19 Vite Progressive Web Apps"]
        Mobile["WebRTC Media Clients (Agora RTC)"]
    end

    subgraph SecurityGateway ["Perimeter Security & API Routing"]
        Gate["Reverse Proxy & Rate Limiters"]
        Auth["JWT, NextAuth & 2FA / TOTP Security Guards"]
        RBAC["Multi-Tenant Context & Granular RBAC"]
    end

    subgraph ServiceClusters ["Application & Microservices Tier"]
        NodeCluster["Express 5 / Node.js 20 Microservices"]
        SocketCluster["Socket.IO Horizontal Clusters (@socket.io/redis-adapter)"]
        AIWorkers["Gemini 2.5 Flash & OpenAI Generative Pipelines"]
        AdTech["Google Ads API Ingestion & Reporting Engine"]
    end

    subgraph PersistenceCluster ["Data & Distributed Infrastructure"]
        PG[("PostgreSQL (Prisma ORM / Supabase RLS)")]
        RedisState[("Redis Cluster (Pub/Sub & Cache)")]
        MongoDB[("MongoDB Replica Sets (Mongoose)")]
        DockerEnv["Alpine Linux Multi-Stage Docker Containers"]
    end

    ClientPerimeter --> Gate
    Gate --> Auth
    Auth --> RBAC
    RBAC --> SSR
    RBAC --> NodeCluster

    NodeCluster <--> SocketCluster
    SocketCluster <--> RedisState

    NodeCluster --> AIWorkers
    SSR --> AdTech

    NodeCluster --> MongoDB
    SSR --> PG
    AIWorkers --> PG
    AdTech --> MongoDB
    ServiceClusters -.-> DockerEnv
```

---

## 🚀 Flagship Production Systems

| System | Role & Architectural Pattern | Tech Stack | Repository |
|---|---|---|---|
| **Ember & Grain** | Multi-Role Restaurant Management Platform featuring real-time kitchen display systems, driver dispatch, and Gemini 2.5 Flash demand forecasting | Next.js 15, TypeScript, PostgreSQL, Prisma ORM, Gemini AI, Docker, pnpm | [View Repo ↗](https://github.com/DanishAjma1/AI-Driven-Resturant) |
| **TrustBridge Backend** | Distributed Real-Time Financial & Deal Engine with Redis pub/sub WebSocket clustering, WebRTC video calling, and Stripe escrow payments | Node.js, Express 5, Redis, Socket.IO, MongoDB, Agora RTC, Stripe, OpenAI | [View Repo ↗](https://github.com/DanishAjma1/TrustBridgeAI-Backend) |
| **TrustBridge UI** | Enterprise Investor Collaboration PWA with interactive term-sheet negotiation modals, real-time messaging, and Agora WebRTC video | React 18, Vite 5, TypeScript, WebRTC Agora, Socket.IO, Stripe, PWA, Vitest | [View Repo ↗](https://github.com/DanishAjma1/TrustBridge-AI) |
| **Harmony School Hub** | Multi-Tenant School ERP SaaS with dynamic institutional branding, automated fee billing, and PostgreSQL Row-Level Security | TanStack Start, React 19, Nitro Engine, Supabase, PostgreSQL RLS, Tailwind v4 | [View Repo ↗](https://github.com/DanishAjma1/harmony-school-hub) |
| **Ads CRM** | Full-Stack Advertising Intelligence CRM with Google Ads API v23 real-time ingestion, automated reporting, and NextAuth RBAC | Next.js 16, React 19, TypeScript, Google Ads API, MongoDB, NextAuth, Recharts | [View Repo ↗](https://github.com/DanishAjma1/CRM) |
| **Muhammadi Studio** | Media Pipeline & Booking Platform featuring Bun runtime, TanStack Table schedule matrix, and ExcelJS automated ledger export | Next.js 16, React 19, Bun Runtime, TanStack Table, ExcelJS, Nodemailer SMTP | [View Repo ↗](https://github.com/DanishAjma1/muhammadi-studio) |

---

## ⚡ Core Engineering & Performance Capabilities

- **Horizontal WebSocket Scaling**: Engineered multi-node WebSocket clusters using `@socket.io/redis-adapter` and Redis pub/sub channels to ensure sub-50ms message broadcast latency across distributed server instances.
- **Strict Multi-Tenant Data Isolation**: Implemented multi-tenant architectures enforcing data isolation at both the application level (tenant context middleware) and database level (PostgreSQL Row-Level Security policies).
- **Predictive AI Pipelines**: Built asynchronous inference pipelines integrating Google Gemini 2.5 Flash and OpenAI GPT models for inventory demand forecasting and automated deal viability scoring.
- **Containerized CI/CD & Production Hardening**: Author of multi-stage Alpine Linux Dockerfiles reducing container image footprints under 120MB with standalone Next.js compilation and GitHub Actions CI pipelines.

---

## 🛠️ Technical Arsenal

### Languages & Core Runtimes
<p align="left">
  <img src="https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/JavaScript-ES2024-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Node.js-20_LTS-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Bun-1.3-FBF0DF?style=for-the-badge&logo=bun&logoColor=black" alt="Bun" />
  <img src="https://img.shields.io/badge/Java-17_LTS-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
</p>

### Frontend & SSR Architectures
<p align="left">
  <img src="https://img.shields.io/badge/Next.js-15_%26_16_(App_Router)-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/React-18_%26_19-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React" />
  <img src="https://img.shields.io/badge/TanStack_Start-SSR-FF4154?style=for-the-badge&logo=tanstack&logoColor=white" alt="TanStack Start" />
  <img src="https://img.shields.io/badge/Vite-5.4-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-v3_%26_v4-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/Radix_UI-Primitives-161618?style=for-the-badge&logo=radixui&logoColor=white" alt="Radix UI" />
</p>

### Backend, Real-Time & Distributed Systems
<p align="left">
  <img src="https://img.shields.io/badge/Express-5.x-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express" />
  <img src="https://img.shields.io/badge/Socket.IO-4.8-010101?style=for-the-badge&logo=socketdotio&logoColor=white" alt="Socket.IO" />
  <img src="https://img.shields.io/badge/Redis-Pub%2FSub_%26_Caching-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />
  <img src="https://img.shields.io/badge/WebRTC-Agora_RTC-099DFD?style=for-the-badge&logo=agora&logoColor=white" alt="Agora RTC" />
  <img src="https://img.shields.io/badge/Google_Ads_API-v23-4285F4?style=for-the-badge&logo=googleads&logoColor=white" alt="Google Ads API" />
  <img src="https://img.shields.io/badge/Stripe-Escrow_&_Billing-635BFF?style=for-the-badge&logo=stripe&logoColor=white" alt="Stripe" />
</p>

### Databases & ORMs
<p align="left">
  <img src="https://img.shields.io/badge/PostgreSQL-16-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/MongoDB-Mongoose_8_%26_9-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
  <img src="https://img.shields.io/badge/Prisma-ORM-2D3748?style=for-the-badge&logo=prisma&logoColor=white" alt="Prisma" />
  <img src="https://img.shields.io/badge/Supabase-Backend_Suite-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase" />
</p>

### DevOps, Testing & Cloud
<p align="left">
  <img src="https://img.shields.io/badge/Docker-Multi--Stage_Builds-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/GitHub_Actions-CI%2FCD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" />
  <img src="https://img.shields.io/badge/Vitest-Unit_Testing-729B1B?style=for-the-badge&logo=vitest&logoColor=white" alt="Vitest" />
  <img src="https://img.shields.io/badge/Jest-Testing_Framework-C21325?style=for-the-badge&logo=jest&logoColor=white" alt="Jest" />
  <img src="https://img.shields.io/badge/pnpm-Workspaces-F69220?style=for-the-badge&logo=pnpm&logoColor=white" alt="pnpm" />
</p>

---

## 📈 Engineering Contributions
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=DanishAjma1&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="Danish's GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=DanishAjma1&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" />
</p>

---

## 💬 Let's Connect & Build
- 🌐 **Portfolio**: [https://danishajma1.github.io/Portfolio/](https://danishajma1.github.io/Portfolio/)
- 💼 **LinkedIn**: [linkedin.com/in/danish-ajmal](https://www.linkedin.com/in/danish-ajmal)
- 📧 **Direct Inquiries**: [danishajmalbutt@gmail.com](mailto:danishajmalbutt@gmail.com)
