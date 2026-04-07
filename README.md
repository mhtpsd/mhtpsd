# Hi there, I'm Mohit Prasad 👋

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=6C63FF&width=700&lines=Software+Engineer+%7C+Building+Scalable+Distributed+Systems;Java+%C2%B7+Spring+Boot+%C2%B7+React+%C2%B7+Kafka+%C2%B7+Kubernetes;Oracle+Certified+Java+SE+11+Developer)](https://git.io/typing-svg)

I'm a **Software Engineer** based in **Ranchi, India** with ~3 years of experience building enterprise-grade applications. I've delivered mission-critical backend and frontend features for **Citi Bank** at LTIMindtree, working on the BRCC (Business Risk Control Committee) platform using Spring Boot, Angular, Redis, and Oracle SQL. I'm passionate about clean architecture, scalable system design, and cloud-native development.

---

## 🏗️ Featured Projects

### [AssetBox](https://github.com/mhtpsd/AssetBox-prod) — Cloud SaaS Digital Asset Marketplace

> Full-stack marketplace for buying & selling digital assets with event-driven architecture

![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js_15-000000?style=flat-square&logo=next.js&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-008CDD?style=flat-square&logo=stripe&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

- **Turborepo** monorepo: `apps/api` (NestJS), `apps/web` (Next.js 15), `apps/workers` (Kafka consumers)
- **Kafka event-driven architecture** — domain events (`asset.uploaded`, `asset.purchased`, `user.registered`) with DLQ handling
- **BullMQ** for background jobs (media processing), **Meilisearch** for full-text search, **MinIO** for S3 storage
- **Stripe** payments with webhook-driven purchase flow, **Resend** transactional emails
- Production Docker Compose + CI/CD with GitHub Actions

---

### [URL Shortener](https://github.com/mhtpsd/url-shortener) — High-Throughput URL Shortening Service

> Production-grade URL shortener with Redis cache-aside & Kafka analytics pipeline

![Spring Boot](https://img.shields.io/badge/Spring_Boot_3.2-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![Java](https://img.shields.io/badge/Java_17-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Redis](https://img.shields.io/badge/Redis_7-DC382D?style=flat-square&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL_16-316192?style=flat-square&logo=postgresql&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

- **Cache-aside pattern** — Redis caches URL resolutions (TTL-based), DB fallback on miss
- **Async Kafka analytics pipeline** — click events published to Kafka, consumed by analytics worker (keeps redirects sub-10ms P99)
- **Base62 encoding** of auto-incremented DB IDs for short codes, custom alias support, QR code generation
- **Rate limiting**, Flyway migrations, SpringDoc OpenAPI, Testcontainers integration tests
- Full **Kubernetes** deployment with Kustomize overlays (dev/prod), HPA autoscaling, GitHub Actions CI/CD → GHCR

---

### [CodeCollab](https://github.com/mhtpsd/collaborative-code-editor) — Real-Time Collaborative Code Editor

> Multi-user code editor with WebSocket sync, sandboxed Docker execution & Kafka queues

![Spring Boot](https://img.shields.io/badge/Spring_Boot_3.2-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![React](https://img.shields.io/badge/React_18-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![WebSocket](https://img.shields.io/badge/WebSocket_(STOMP)-010101?style=flat-square&logo=websocket&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis_Pub%2FSub-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)

- **STOMP over SockJS** WebSocket for real-time code sync, cursor tracking & in-room chat
- **Redis Pub/Sub** enables horizontal scaling — messages forwarded across multiple backend instances
- **Monaco Editor** (VS Code engine) with remote cursor decorations and 6 language support
- **Sandboxed Docker execution** — code runs in network-disabled, memory-limited containers (128MB, 10s timeout)
- **Kafka execution queue** — decouples code submission from execution, with result broadcast via WebSocket
- Kubernetes manifests with **sticky sessions** for WebSocket affinity, HPA, Kustomize overlays

---

## 🧠 Architecture Patterns I Work With

```
✅ Event-Driven Architecture (Kafka)     ✅ Cache-Aside (Redis)
✅ WebSocket Real-Time Sync (STOMP)       ✅ Async Message Queues
✅ Microservices + Monorepo               ✅ Container Orchestration (K8s)
✅ CI/CD Pipelines (GitHub Actions)       ✅ Sandboxed Code Execution (Docker)
✅ Domain Events + DLQ Handling           ✅ Webhook-Driven Integrations
```

---

## 💻 Tech Stack

**Languages**

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

**Backend**

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)

**Frontend**

![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**Databases & Messaging**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)

**DevOps & Cloud**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

**Tools & Frameworks**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)
![Jira](https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white)
![IntelliJ](https://img.shields.io/badge/IntelliJ-000000?style=for-the-badge&logo=intellij-idea&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=mhtpsd&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" height="170" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mhtpsd&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top Languages" height="170" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=mhtpsd&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</p>

---

## 🎓 Certifications

- **Oracle Certified Professional: Java SE 11 Developer** (1Z0-819)

---

## 📫 Let's Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mhtpsd/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mhtpsd)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mohitmanoj1704@gmail.com)

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=mhtpsd&color=6C63FF&style=flat-square&label=Profile+Views" alt="Profile Views" />
</p>
