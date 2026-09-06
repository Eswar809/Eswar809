<!-- Banner: assets/hero-dark.svg (dark mode) and assets/hero.svg (light mode) live in this repo -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/hero-dark.svg">
  <img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/hero.svg" alt="Deevi Eswar — Software Engineer. I build systems that survive production." width="100%">
</picture>

<p align="center">
  <a href="https://devs-portiofolio.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-2D333B?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio"></a>&nbsp;
  <a href="https://www.linkedin.com/in/eswar-dev-55a54536a/"><img src="https://img.shields.io/badge/LinkedIn-2D333B?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>&nbsp;
  <a href="https://leetcode.com/u/Eswardeevi/"><img src="https://img.shields.io/badge/LeetCode-2D333B?style=flat-square&logo=leetcode&logoColor=white" alt="LeetCode"></a>&nbsp;
  <a href="mailto:deevieswar44@gmail.com"><img src="https://img.shields.io/badge/Email-2D333B?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
</p>

**B.Tech CSE (AI & Data Science)**, Vasireddy Venkatadri Institute of Technology, Guntur — Class of 2026 · CGPA 7.0/10.

Looking for my first full-time **Software Engineer role** — backend, full-stack, or AI. Guntur, India · **open to relocation** · **immediately available**.

I work on the parts of software nobody notices until they're missing: idempotent webhooks, retries with jitter, race conditions, token budgets.

<br>

## The short version

1. **My software runs in production every day.** Sole engineer for a CA/CS coaching institute — I design, ship, and operate two systems end to end: [PaperCheck AI](https://paper-checking.netlify.app/) grades **150+ handwritten answer sheets a day**, and my WhatsApp automation platform serves **300+ daily queries**.
2. **The business case is measured.** PaperCheck grades a paper for **₹15–21** against the ₹100–190 human evaluators charge, in minutes instead of 2–3 days.
3. **Google merged my code.** [PR #26884](https://github.com/google-gemini/gemini-cli/pull/26884) in `google-gemini/gemini-cli`, approved by a Google maintainer — picked up from a *help-wanted* issue.
4. **TCS CodeVita Season 13:** global rank **2028** of 100,000+ participants — top ~2%.

<br>

## Experience

### Freelance Software Engineer — Client: CA/CS coaching institute · Jan 2026 – Present

**Sole engineer** reporting to the institute's directors. I own two production systems end to end — UI, APIs, data model, deployment, security, operations, and post-release verification.

**PaperCheck AI** — [live](https://paper-checking.netlify.app/)

Grades batches of handwritten CA/CS answer sheets in parallel — one streaming AI worker per student — and returns annotated, examiner-style PDFs.

- **150+ answer sheets a day** in production; turnaround **2–3 days → minutes**, cost **₹100–190 → ₹15–21 per paper**
- The LLM only extracts inside **schema-constrained JSON**; decision logic, a faculty **human-review loop**, and typed fallbacks keep wrong outputs from reaching users
- Root-caused silent streaming hangs: **zero-chunks restart gate + 10-step jittered backoff** with transient-vs-permanent error classification — retry when safe, fail fast and loudly when not; **zero silent failures since**
- Browser-direct streaming keeps multi-minute model runs clear of serverless timeouts; SHA-256-keyed prompt cache (6 h TTL); 50 MB signed-token PDF uploads

**WhatsApp messaging platform** — [source](https://github.com/Eswar809/whatsapp-messaging-platform)

Event-driven admissions automation on the official WhatsApp Cloud API: FAQs, demo booking, payments, doubt triage to faculty, daily MCQ engine. **300+ daily queries.**

- **HMAC-SHA256** webhook verification with constant-time compare; fast ACK, async processing; message-id **idempotency** absorbs Meta's webhook redeliveries
- Full-jitter retries with transient-vs-permanent error classification; WhatsApp's 24-hour messaging rule enforced at a single outbound choke point
- **Deterministic-first routing keeps decisions off the model**, cutting AI cost **~90%**; 16-entity Prisma/PostgreSQL schema; runs credential-free in stub mode

<br>

## Projects

### CA GURU — full-stack learning platform · [live](https://ca-study.netlify.app/)

All-in-one platform for CA students: AI tutoring over chat and real-time voice, a notes library, a social feed with DMs and stories, study rooms, leaderboards.

- **70.7K lines of TypeScript** — Next.js 16 + React 19, **36 REST API routes**, **138 reusable React components**
- Security enforced at the database: **34 tables, 85 row-level-security policies, 18 `SECURITY DEFINER` functions** on Supabase Postgres; server-side price derivation eliminates client-side tampering
- Real-time **voice mentor** on an inline AudioWorklet with ephemeral WebSocket tokens and barge-in; cross-browser sample-rate mismatch solved with dynamic resampling
- Three-model Gemini fallback cascade (a degraded answer beats downtime), SSE streaming chat, per-IP sliding-window rate limits with `Retry-After`

### Spring Boot backends

- **Complaint Management System** — [source](https://github.com/Eswar809/Complaint-Management-System): a **15-endpoint REST API** in Java 17 / Spring Boot 3.1 with a decoupled React client, built in a **three-person team** through PRs and code review. Database-level **race-condition fix proven by a concurrency test**; Hibernate **N+1 fix with a regression guard**; CI via GitHub Actions and Jenkins (root-caused and pinned a JDK 11 vs 17 runner mismatch).
- **Student management portal** — [source](https://github.com/Eswar809/student-management): role-based academic portal with Spring Security and Docker MySQL health checks.

<p>
  <a href="https://github.com/Eswar809/student-management"><img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=Eswar809&repo=student-management&hide_border=true&bg_color=00000000&title_color=58A6FF&icon_color=3FB950&text_color=8B949E" alt="student-management"></a>
  <a href="https://github.com/Eswar809/Complaint-Management-System"><img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=Eswar809&repo=Complaint-Management-System&hide_border=true&bg_color=00000000&title_color=58A6FF&icon_color=3FB950&text_color=8B949E" alt="Complaint-Management-System"></a>
</p>

<br>

## Open source

**Merged code into [google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli)** — Google's official Gemini CLI.

- [PR #26884, merged](https://github.com/google-gemini/gemini-cli/pull/26884) — `fix(core): ignore .pak & .rpa game archives by default`, approved by a Google maintainer; stops silent context bloat from game-archive files
- [12 PRs submitted, 3 currently open](https://github.com/google-gemini/gemini-cli/pulls?q=is%3Apr+author%3AEswar809)

<br>

## Achievements

|  |  |
|:--|:--|
| **TCS CodeVita Season 13** | Global rank **2028** of 100,000+ — top ~2% · [cert](https://drive.google.com/file/d/1JOcloo3anttUxjaUHiX0Z6wL3hVLxrh_/view?usp=sharing) |
| **LeetCode** | [196 problems solved](https://leetcode.com/u/Eswardeevi/) — 91 Medium, 14 Hard |
| **Google Cloud Skills Boost** | [Gold League](https://www.skills.google/public_profiles/7cf59d17-1529-4a12-9a4f-55c9c6568efd) · 30 badges |
| **Certifications** | NPTEL Java (IIT) · AICTE–EduSkills AI/ML internship (2024) |

<br>

## Stack

<table>
  <tr><td align="right"><b>Backend</b></td><td><img src="https://skillicons.dev/icons?i=java,spring,nodejs,express,py" height="36" alt="Java, Spring Boot, Node.js, Express, Python"></td></tr>
  <tr><td align="right"><b>Web</b></td><td><img src="https://skillicons.dev/icons?i=ts,js,react,nextjs" height="36" alt="TypeScript, JavaScript, React, Next.js"></td></tr>
  <tr><td align="right"><b>Data</b></td><td><img src="https://skillicons.dev/icons?i=postgres,mysql,prisma,supabase" height="36" alt="PostgreSQL, MySQL, Prisma, Supabase"></td></tr>
  <tr><td align="right"><b>AI</b></td><td><img src="https://img.shields.io/badge/Gemini_API-2D333B?style=flat-square" alt="Gemini API">&nbsp;<img src="https://img.shields.io/badge/Claude_Code-2D333B?style=flat-square" alt="Claude Code">&nbsp;<img src="https://img.shields.io/badge/MCP-2D333B?style=flat-square" alt="MCP">&nbsp;<img src="https://img.shields.io/badge/Prompt_caching-2D333B?style=flat-square" alt="Prompt caching"></td></tr>
  <tr><td align="right"><b>Cloud</b></td><td><img src="https://skillicons.dev/icons?i=gcp,vercel,docker,githubactions,git" height="36" alt="Google Cloud, Vercel, Docker, GitHub Actions, Git"></td></tr>
</table>

<br>

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Eswar809&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&bg_color=00000000&title_color=58A6FF&icon_color=3FB950&text_color=8B949E&ring_color=3FB950" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Eswar809&layout=compact&langs_count=6&hide_border=true&bg_color=00000000&title_color=58A6FF&text_color=8B949E" alt="Top languages">
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=Eswar809&theme=transparent&hide_border=true&ring=3FB950&fire=3FB950&currStreakNum=58A6FF&sideNums=58A6FF&currStreakLabel=8B949E&sideLabels=8B949E&dates=8B949E" alt="GitHub streak">
</p>

<!-- Snake animation — the workflow (.github/workflows/snake.yml) is valid; it fails only because the
     GitHub account is billing-locked. After the billing issue is fixed at github.com/settings/billing,
     run the workflow once from the Actions tab (it publishes SVGs to the `output` branch), then
     uncomment this block.
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Eswar809/Eswar809/output/github-contribution-grid-snake-dark.svg">
    <img src="https://raw.githubusercontent.com/Eswar809/Eswar809/output/github-contribution-grid-snake.svg" alt="Contribution snake animation">
  </picture>
</p>
-->

<br>

---

<p align="center">
  If this sounds like your team's kind of work — <a href="mailto:deevieswar44@gmail.com"><b>deevieswar44@gmail.com</b></a> gets the fastest reply.
</p>
