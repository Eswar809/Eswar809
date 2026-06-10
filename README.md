# Hi, I'm Deevi Eswar 👋

**Backend & AI engineer** — I build event-driven messaging systems and AI products that run in production.

🎓 B.Tech, Artificial Intelligence & Data Science — Class of 2026 · 📍 India, open to relocation · 💼 Looking for Software Engineer roles

[**Portfolio**](https://devs-portiofolio.netlify.app/) · [**LinkedIn**](https://www.linkedin.com/in/eswar-dev-55a54536a/) · [**LeetCode**](https://leetcode.com/u/Eswardeevi/) · [**deevieswar44@gmail.com**](mailto:deevieswar44@gmail.com)

---

## 🚀 Flagship work

### 📄 [PaperCheck AI](https://paper-checking.netlify.app/) — AI exam grading, **live in production**

Grades batches of handwritten CA/CS answer sheets **in parallel** (one streaming AI worker per student) and returns annotated, examiner-style PDFs — in active use by coaching faculty.

- **~85% cheaper than human evaluation** — Rs. 15–21/paper vs the Rs. 100–190 evaluators charge, in **minutes instead of 2–3 days**
- Two prompt-caching layers (SHA-256-keyed explicit cache w/ 6 h TTL + `cache_control` prefix reuse) to hold cost down
- Layered reliability: 10-step jittered exponential backoff, zero-output-gated stream restarts (no paper graded twice), bounded auto-resume for paused long runs
- Browser-direct streaming architecture so multi-minute model runs never hit serverless timeouts

### 💬 [Event-Driven WhatsApp Messaging Platform](https://github.com/Eswar809/whatsapp-messaging-platform)

24/7 admissions automation on the **official WhatsApp Cloud API** — FAQs, demo booking, payments, doubt triage to faculty, daily MCQ engine.

- **HMAC-SHA256-verified webhooks** (constant-time compare) · fast ACK + async processing
- **Message-id idempotency** absorbs Meta's webhook redeliveries · **exponential backoff + full-jitter retries** with transient-vs-permanent error classification
- WhatsApp's 24-hour policy enforced at a **single outbound choke point** with graceful degradation — policy limits never crash the service
- 16-entity Prisma/PostgreSQL schema · timezone-aware cron jobs · runs fully credential-free in stub mode

### ☕ Java / Spring Boot backends

- [**student-management**](https://github.com/Eswar809/student-management) — role-based academic portal: **database-level race-condition fix** proven by a concurrency test, Hibernate **N+1 fix** with a regression guard, Spring Security, Docker w/ MySQL health check
- [**Complaint-Management-System**](https://github.com/Eswar809/Complaint-Management-System) — 15-endpoint Spring Boot REST API + React, centralized CORS policy bean, GitHub Actions + Jenkins CI (built in a 3-person team via PRs and code reviews)

---

## 🔧 Open source

**[google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli/pulls?q=is%3Apr+author%3AEswar809)** — 12 PRs submitted to Google's official Gemini CLI: [**PR #26884 merged**](https://github.com/google-gemini/gemini-cli/pull/26884) (`fix(core)`, approved by a Google maintainer — picked up from a *help-wanted* issue), 3 currently open.

---

## 🏆 Highlights

- **TCS CodeVita Season 13 (2025): Global Rank 2028** among 100,000+ participants (Top 2%)
- **150+ LeetCode** problems solved · **Google Cloud Skills Boost Gold League** — 21,010 pts, 25+ badges
- LLM evaluation engineering: [**rag-eval-pipeline**](https://github.com/Eswar809/rag-eval-pipeline) — merge-blocking CI quality gates; chunking retune lifted Faithfulness **0.45 → 0.82**

---

## 🛠️ Stack

![Java](https://img.shields.io/badge/Java%2017-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js%2022-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)

---

<sub>📫 Fastest way to reach me: [deevieswar44@gmail.com](mailto:deevieswar44@gmail.com)</sub>
