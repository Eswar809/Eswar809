<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/hero-dark.svg">
  <img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/hero.svg" alt="Deevi Eswar — Software Engineer. I build systems that survive production." width="100%">
</picture>

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/taglines-dark.svg">
  <img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/taglines.svg" alt="Event-driven systems that don't drop messages · AI grading in production — 150+ answer sheets a day · Merged PR at google-gemini/gemini-cli · B.Tech CSE (AI & DS), Class of 2026" width="100%">
</picture>

<img src="https://img.shields.io/badge/%F0%9F%9F%A2_OPEN_TO_WORK-Software_Engineer_%C2%B7_Class_of_2026-00F5A0?style=for-the-badge&labelColor=0B1221" alt="Open to work — Software Engineer, Class of 2026"/>

<br/><br/>

<a href="https://devs-portiofolio.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-8B5CF6?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>&nbsp;
<a href="https://www.linkedin.com/in/eswar-dev-55a54536a/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>&nbsp;
<a href="https://leetcode.com/u/Eswardeevi/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode"/></a>&nbsp;
<a href="mailto:deevieswar44@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>

<br/><br/>

<!-- ── the 7-second proof strip — the numbers a recruiter must see ── -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/impact-dark.svg">
  <img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/impact.svg" alt="150+ answer sheets graded daily in production · ₹15–21 per paper vs ₹100–190 human · PR 26884 merged at gemini-cli · Global rank 2028 of 100,000+ TCS CodeVita S13 · 196 LeetCode problems solved" width="100%">
</picture>

</div>

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/divider.svg" width="100%" alt=""/>

## 👋 About Me

- 🎓 **B.Tech CSE (AI & Data Science)**, Vasireddy Venkatadri Institute of Technology, Guntur — Class of **2026** · CGPA 7.0/10
- 💼 Looking for my first full-time **Software Engineer role** — backend, full-stack, or AI · 📍 Guntur, India · **open to relocation** · **immediately available**
- ⚡ I work on the parts of software nobody notices until they're missing: **idempotent webhooks, retries with jitter, race conditions, token budgets**

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/divider.svg" width="100%" alt=""/>

## ⚡ The short version

1. **My software runs in production every day.** Sole engineer for a CA/CS coaching institute — I design, ship, and operate two systems end to end: [PaperCheck AI](https://paper-checking.netlify.app/) grades **150+ handwritten answer sheets a day**, and my WhatsApp automation platform serves **300+ daily queries**.
2. **The business case is measured.** PaperCheck grades a paper for **₹15–21** against the ₹100–190 human evaluators charge, in minutes instead of 2–3 days.
3. **Google merged my code.** [PR #26884](https://github.com/google-gemini/gemini-cli/pull/26884) in `google-gemini/gemini-cli`, approved by a Google maintainer — picked up from a *help-wanted* issue.
4. **TCS CodeVita Season 13:** global rank **2028** of 100,000+ participants — top ~2%.

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/divider.svg" width="100%" alt=""/>

## 💼 Experience

### Freelance Software Engineer — Client: CA/CS coaching institute · Jan 2026 – Present

**Sole engineer** reporting to the institute's directors. I own two production systems end to end — UI, APIs, data model, deployment, security, operations, and post-release verification.

<br/>

### 📄 PaperCheck AI

<a href="https://paper-checking.netlify.app/"><img src="https://img.shields.io/badge/%E2%96%B6_Open_Live_App-paper--checking.netlify.app-00D9F5?style=flat-square&labelColor=0B1221" alt="Open live app"/></a> <img src="https://img.shields.io/badge/LIVE_IN_PRODUCTION-00F5A0?style=flat-square&labelColor=0B1221" alt="Live in production"/>

> Grades batches of handwritten CA/CS answer sheets in parallel — one streaming AI worker per student — and returns **annotated, examiner-style PDFs**.

- 💸 **150+ answer sheets a day** in production; turnaround **2–3 days → minutes**, cost **₹100–190 → ₹15–21 per paper**
- 🛡️ The LLM only extracts inside **schema-constrained JSON**; decision logic, a faculty **human-review loop**, and typed fallbacks keep wrong outputs from reaching users
- ⚙️ Root-caused silent streaming hangs: **zero-chunks restart gate + 10-step jittered backoff** with transient-vs-permanent error classification — retry when safe, fail fast and loudly when not; **zero silent failures since**
- 🧠 Browser-direct streaming keeps multi-minute model runs clear of serverless timeouts; **SHA-256-keyed prompt cache** (6 h TTL); **50 MB signed-token** PDF uploads

<br/>

### 💬 WhatsApp messaging platform

<a href="https://github.com/Eswar809/whatsapp-messaging-platform"><img src="https://img.shields.io/badge/%E2%96%B6_View_Source-GitHub-00D9F5?style=flat-square&labelColor=0B1221&logo=github" alt="View source on GitHub"/></a> <img src="https://img.shields.io/badge/Official_WhatsApp_Cloud_API-25D366?style=flat-square&labelColor=0B1221&logo=whatsapp&logoColor=white" alt="Official WhatsApp Cloud API"/>

> Event-driven admissions automation: FAQs, demo booking, payments, doubt triage to faculty, and a daily MCQ engine. **300+ daily queries.**

- 🔐 **HMAC-SHA256** webhook verification with constant-time compare; fast ACK, async processing; message-id **idempotency** absorbs Meta's webhook redeliveries
- ♻️ Full-jitter retries with transient-vs-permanent error classification; WhatsApp's **24-hour messaging rule enforced at a single outbound choke point**
- 🚦 **Deterministic-first routing keeps decisions off the model**, cutting AI cost **~90%**; 16-entity Prisma/PostgreSQL schema; runs credential-free in stub mode

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/divider.svg" width="100%" alt=""/>

## 🚀 Featured builds

### 🎓 CA GURU — full-stack learning platform

<a href="https://ca-study.netlify.app/"><img src="https://img.shields.io/badge/%E2%96%B6_Open_Live_App-ca--study.netlify.app-00D9F5?style=flat-square&labelColor=0B1221" alt="Open live app"/></a> <img src="https://img.shields.io/badge/LIVE-00F5A0?style=flat-square&labelColor=0B1221" alt="Live"/>

> All-in-one platform for CA students: AI tutoring over chat and real-time voice, a notes library, a social feed with DMs and stories, study rooms, leaderboards.

- 🧱 **70.7K lines of TypeScript** — Next.js 16 + React 19, **36 REST API routes**, **138 reusable React components**
- 🔐 Security enforced at the database: **34 tables, 85 row-level-security policies, 18 `SECURITY DEFINER` functions** on Supabase Postgres; server-side price derivation eliminates client-side tampering
- 🎙️ Real-time **voice mentor** on an inline AudioWorklet with ephemeral WebSocket tokens and barge-in; cross-browser sample-rate mismatch solved with dynamic resampling
- 🤖 **Three-model Gemini fallback cascade** (a degraded answer beats downtime), SSE streaming chat, per-IP sliding-window rate limits with `Retry-After`

<br/>

### ☕ Spring Boot backends

<details>
<summary><b>⚙️ Two Java backends — open the engineering highlights</b></summary>
<br/>

- 📋 **Complaint Management System** — [source](https://github.com/Eswar809/Complaint-Management-System): a **15-endpoint REST API** in Java 17 / Spring Boot 3.1 with a decoupled React client, built in a **three-person team** through PRs and code review. Database-level **race-condition fix proven by a concurrency test**; Hibernate **N+1 fix with a regression guard**; CI via GitHub Actions and Jenkins (root-caused and pinned a JDK 11 vs 17 runner mismatch).
- 🎓 **Student management portal** — [source](https://github.com/Eswar809/student-management): role-based academic portal with Spring Security and Docker MySQL health checks.

</details>

<p>
  <a href="https://github.com/Eswar809/student-management"><img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=Eswar809&repo=student-management&hide_border=true&bg_color=00000000&title_color=00D9F5&icon_color=00F5A0&text_color=8B949E" alt="student-management"></a>
  <a href="https://github.com/Eswar809/Complaint-Management-System"><img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=Eswar809&repo=Complaint-Management-System&hide_border=true&bg_color=00000000&title_color=00D9F5&icon_color=00F5A0&text_color=8B949E" alt="Complaint-Management-System"></a>
</p>

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/divider.svg" width="100%" alt=""/>

## 🌱 Open source

**Merged code into [google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli)** — Google's official Gemini CLI.

<img src="https://img.shields.io/badge/PRs_submitted-12-00D9F5?style=flat-square&labelColor=0B1221" alt="12 PRs submitted"/> <img src="https://img.shields.io/badge/merged-fix%28core%29_%2326884-00F5A0?style=flat-square&labelColor=0B1221" alt="PR 26884 merged"/> <img src="https://img.shields.io/badge/currently_open-3-8B5CF6?style=flat-square&labelColor=0B1221" alt="3 PRs open"/>

- ✅ [**PR #26884 — merged**](https://github.com/google-gemini/gemini-cli/pull/26884) — `fix(core): ignore .pak & .rpa game archives by default`, **approved by a Google maintainer**; stops silent context bloat from game-archive files. Picked up from a *help-wanted* issue.
- 📬 [**12 PRs submitted, 3 currently open**](https://github.com/google-gemini/gemini-cli/pulls?q=is%3Apr+author%3AEswar809)

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/divider.svg" width="100%" alt=""/>

## 🏆 Achievements

|  |  |
|:--|:--|
| 🥇 **TCS CodeVita Season 13** | Global rank **2028** of 100,000+ — top ~2% · [cert](https://drive.google.com/file/d/1JOcloo3anttUxjaUHiX0Z6wL3hVLxrh_/view?usp=sharing) |
| 🧮 **LeetCode** | [**196 problems solved**](https://leetcode.com/u/Eswardeevi/) — 91 Medium, 14 Hard |
| ☁️ **Google Cloud Skills Boost** | [**Gold League**](https://www.skills.google/public_profiles/7cf59d17-1529-4a12-9a4f-55c9c6568efd) · 30 badges |
| 📜 **Certifications** | NPTEL Java (IIT) · AICTE–EduSkills AI/ML internship (2024) |

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/divider.svg" width="100%" alt=""/>

## 🧰 Stack

<div align="center">

<table>
  <tr><td align="right"><b>Backend</b></td><td><img src="https://skillicons.dev/icons?i=java,spring,nodejs,express,py" height="36" alt="Java, Spring Boot, Node.js, Express, Python"></td></tr>
  <tr><td align="right"><b>Web</b></td><td><img src="https://skillicons.dev/icons?i=ts,js,react,nextjs" height="36" alt="TypeScript, JavaScript, React, Next.js"></td></tr>
  <tr><td align="right"><b>Data</b></td><td><img src="https://skillicons.dev/icons?i=postgres,mysql,prisma,supabase" height="36" alt="PostgreSQL, MySQL, Prisma, Supabase"></td></tr>
  <tr><td align="right"><b>AI</b></td><td><img src="https://img.shields.io/badge/Gemini_API-2D333B?style=flat-square" alt="Gemini API">&nbsp;<img src="https://img.shields.io/badge/Claude_Code-2D333B?style=flat-square" alt="Claude Code">&nbsp;<img src="https://img.shields.io/badge/MCP-2D333B?style=flat-square" alt="MCP">&nbsp;<img src="https://img.shields.io/badge/Prompt_caching-2D333B?style=flat-square" alt="Prompt caching"></td></tr>
  <tr><td align="right"><b>Cloud</b></td><td><img src="https://skillicons.dev/icons?i=gcp,vercel,docker,githubactions,git" height="36" alt="Google Cloud, Vercel, Docker, GitHub Actions, Git"></td></tr>
</table>

</div>

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/divider.svg" width="100%" alt=""/>

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Eswar809&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&bg_color=00000000&title_color=00D9F5&icon_color=00F5A0&text_color=8B949E&ring_color=00F5A0" alt="GitHub stats">
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Eswar809&layout=compact&langs_count=6&hide_border=true&bg_color=00000000&title_color=00D9F5&text_color=8B949E" alt="Top languages">

<br/>

<img src="https://streak-stats.demolab.com?user=Eswar809&theme=transparent&hide_border=true&ring=00F5A0&fire=00F5A0&currStreakNum=00D9F5&sideNums=00D9F5&currStreakLabel=8B949E&sideLabels=8B949E&dates=8B949E" alt="GitHub streak">

</div>

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

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/divider.svg" width="100%" alt=""/>

<p align="center">
  If this sounds like your team's kind of work — <a href="mailto:deevieswar44@gmail.com"><b>deevieswar44@gmail.com</b></a> gets the fastest reply.
</p>
