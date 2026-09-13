## 👋 Hi, I'm Faiz Alam

Backend Engineer at **AgNext Technologies**, working across a multi-product B2B SaaS platform — REST APIs in **Node.js** and **Python**, PostgreSQL data modelling, event-driven workflows on **Azure Service Bus**, and multi-tenant access control.

I gravitate toward problems where correctness matters more than cleverness: audit trails that can't lose history, permission models that span organizations, and schema migrations that ship into a live product without downtime.

---

## 🏗 What I've Built

**Append-only ledger for physical-asset custody**
Every receipt, split, merge, transfer and dispatch is recorded as an immutable entry rather than overwriting state, so the full chain of custody stays auditable. Shipped with zero downtime alongside the existing APIs, letting clients cut over one at a time.

**Multi-tenant authorization model**
Fine-grained per-stage permissions — view, create, move, split, merge, approve — resolved from user and role assignments, plus cross-organization rules that let counterparties see the handoff between them without exposing either party's wider data.

**Observability layer**
Moved reporting onto a Logstash → OpenSearch pipeline backed by PostgreSQL materialized views, cutting dashboard load from **22s to 2–3s**. Added role-scoped multi-tenant log access so each team audits its own data.

**Identity & payments**
Unified authentication and authorization across platform services on **Keycloak SSO** (OAuth2, RBAC), replacing per-service auth with a single token model. Integrated **Razorpay** licensing with signature-verified webhooks and idempotent writes, so retried callbacks can't double-charge.

**Real-time notification delivery**
Socket.IO and Firebase Cloud Messaging layer persisting **~10K notifications daily** and pushing thousands to field agents across enterprise client organizations.

**Configurable workflow builder**
Let clients design their own inspection flows from ordered, reusable form templates with repeatable sections — replacing a hardcoded single-form process.

**RAG classification service**
Azure OpenAI service that auto-categorizes quality data the operations team previously sorted by hand. Adopted as their default workflow.

---

## 💻 Tech Stack

**Languages** &nbsp; JavaScript (Node.js) · Python · SQL · Java

**Backend & APIs** &nbsp; Express.js · FastAPI · Spring Boot · REST APIs · Microservices · Event-Driven Architecture · WebSockets (Socket.IO, SSE) · SQLAlchemy · Hibernate / JPA

**Frontend** &nbsp; React · Progressive Web Apps (PWA) · Vite · Vanilla JS

**Data & Messaging** &nbsp; PostgreSQL · MySQL (TiDB) · MongoDB · Redis · Apache Kafka · Azure Service Bus

**Cloud & DevOps** &nbsp; Azure · AWS · Docker · Kubernetes · Git · GitHub Actions · CI/CD

**Observability & Security** &nbsp; Grafana · OpenSearch · Logstash · Keycloak (OAuth2 / RBAC / SSO)

---

## 📌 Projects

### [Dynamic Surge Pricing Engine](https://github.com/FaizAlam4/Dynamic-Serge-Engine) — Event-driven geospatial price calculator
A production-grade ride-sharing simulator mirroring Uber's pricing backend. Maps high-throughput geospatial click events into an **Apache Kafka** cluster, calculates real-time zone multipliers via an in-memory aggregation layer, and pushes sub-millisecond updates to a Leaflet.js dashboard using **Server-Sent Events (SSE)**. Protected the MySQL database from event storms by implementing async `@Scheduled` batch upserts via Hibernate ORM. Includes self-healing multi-threaded auto-decay to organically resolve demand spikes.

`Java` `Spring Boot` `Apache Kafka` `MySQL (TiDB Serverless)` `Hibernate` `Leaflet.js`
→ [Live demo](https://dynamic-serge-engine.onrender.com/)

### [Job Pulse](https://github.com/FaizAlam4/job-pulse) — AI job aggregation & resume analysis
Cron-driven ingestion engine with SHA-256 content-hash deduplication, an AI resume analyzer (Groq, Azure OpenAI), and a composite ranking engine over a Redis cache-aside layer holding sub-5 ms reads. Containerized with Docker; every push gated by CI running **183 automated tests at 81% coverage**.

`Node.js` `MongoDB Atlas` `Upstash Redis` `Docker` `GitHub Actions` — deployed on Render + Vercel
→ [Live demo](https://job-pulse-ten.vercel.app/)

---

## 📫 Connect

📧 &nbsp; mfaizalam32@gmail.com
🔗 &nbsp; [LinkedIn](https://www.linkedin.com/in/faizalam4/)
🌐 &nbsp; [Portfolio](https://faizalam4.github.io/portfolio_faiz/)
🧩 &nbsp; [LeetCode](https://leetcode.com/u/FaizNexus/)
