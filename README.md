<!-- ═══════════════════════════ HERO ═══════════════════════════ -->
<div align="center">

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/hero.svg" width="100%" alt="Deevi Eswar — Backend & AI Engineer · shipping systems that survive production"/>

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/taglines.svg" width="100%" alt="Event-driven systems that don't drop messages · AI products running live in production · Merged PR @ google-gemini/gemini-cli · SWE Class of 2026"/>

<img src="https://img.shields.io/badge/%F0%9F%9F%A2_OPEN_TO_WORK-Software_Engineer_%C2%B7_Class_of_2026-00F5A0?style=for-the-badge&labelColor=0B1221" alt="Open to work — Software Engineer, Class of 2026"/>

<br/><br/>

<a href="https://devs-portiofolio.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-8B5CF6?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>&nbsp;
<a href="https://www.linkedin.com/in/eswar-dev-55a54536a/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>&nbsp;
<a href="https://leetcode.com/u/Eswardeevi/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode"/></a>&nbsp;
<a href="mailto:deevieswar44@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>

<br/><br/>

<!-- ── 7-second proof strip — the numbers a recruiter must see ── -->

<img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/impact.svg" width="100%" alt="~85% cheaper AI grading, live in production · 85K+ lines of TypeScript in one product · 12 PRs @ Google's gemini-cli, 1 merged · Top ~2% TCS CodeVita S13, Global Rank 2028 · 170+ LeetCode problems solved"/>

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00F5A0,25:00D9F5,50:8B5CF6,75:FF6EC7,100:FFB86C&height=4" width="100%" alt=""/>

## 👋 About Me

- 🎓 **B.Tech CSE (AI & Data Science)** · Class of **2026**
- 💼 Looking for **Software Engineer (Backend / Full-Stack / AI)** roles · 📍 India, **open to relocation**
- ⚡ I obsess over the unglamorous things that keep systems alive — **idempotency, retries with jitter, race conditions, webhook security, prompt-cost engineering**
- 📫 Fastest way to reach me → **[deevieswar44@gmail.com](mailto:deevieswar44@gmail.com)**

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00F5A0,25:00D9F5,50:8B5CF6,75:FF6EC7,100:FFB86C&height=4" width="100%" alt=""/>

## 🚀 Featured Builds

<div align="center"><samp>— things that run without me babysitting them —</samp></div>

<br/>

### 📄 PaperCheck AI

<a href="https://paper-checking.netlify.app/"><img src="https://img.shields.io/badge/%E2%96%B6_Open_Live_App-paper--checking.netlify.app-00D9F5?style=flat-square&labelColor=0B1221" alt="Open live app"/></a> <img src="https://img.shields.io/badge/LIVE_IN_PRODUCTION-00F5A0?style=flat-square&labelColor=0B1221" alt="Live in production"/>

> **AI exam-grading platform** — grades batches of handwritten CA/CS answer sheets **in parallel** (one streaming AI worker per student) and returns **annotated, examiner-style PDFs**. In active daily use by coaching faculty.

- 💸 **~85% cheaper than human evaluation** — **₹15–21/paper** vs the ₹100–190 evaluators charge, in **minutes instead of 2–3 days** — powered by Gemini Flash + strict token budgeting
- 🛡️ **Layered reliability** — 10-step jittered exponential backoff · zero-output-gated stream restarts (**no paper graded twice**) · bounded auto-resume for paused long runs
- ⚡ **Browser-direct streaming** — multi-minute model runs never hit serverless timeouts
- 🧠 **SHA-256-keyed explicit prompt cache** (6 h TTL) on the server route · **50 MB signed-token PDF uploads**

<br/>

### 🎓 CA GURU

<a href="https://ca-study.netlify.app/"><img src="https://img.shields.io/badge/%E2%96%B6_Open_Live_App-ca--study.netlify.app-00D9F5?style=flat-square&labelColor=0B1221" alt="Open live app"/></a> <img src="https://img.shields.io/badge/LIVE-00F5A0?style=flat-square&labelColor=0B1221" alt="Live"/>

> **All-in-one learning platform for CA students** — AI tutoring (chat · voice · TTS), notes library, social feed with DMs & stories, study rooms, leaderboards & rewards.

- 🧱 **~85K-LOC TypeScript codebase** — **Next.js + React 19** · **29+ API routes** · **26+ dashboard pages** · full social layer
- 🔐 **Security enforced at the database** — Supabase Postgres with **34 tables · 85 row-level-security policies · 18 `SECURITY DEFINER` RPCs**
- 🤖 **3-model Gemini fallback cascade** — a degraded answer beats downtime · SSE streaming chat · ephemeral-token live voice
- 🚦 **Per-IP sliding-window rate limiting** (with `Retry-After`) on every major route · constant-time webhook auth

<br/>

### 💬 Event-Driven WhatsApp Messaging Platform

<a href="https://github.com/Eswar809/whatsapp-messaging-platform"><img src="https://img.shields.io/badge/%E2%96%B6_View_Source-GitHub-00D9F5?style=flat-square&labelColor=0B1221&logo=github" alt="View source on GitHub"/></a> <img src="https://img.shields.io/badge/Official_WhatsApp_Cloud_API-25D366?style=flat-square&logo=whatsapp&logoColor=white" alt="Official WhatsApp Cloud API"/>

> **24/7 admissions automation** — FAQs, demo booking, payments, doubt triage to faculty, and a daily MCQ engine.

- 🔐 **HMAC-SHA256-verified webhooks** (constant-time compare) · fast ACK + async processing
- ♻️ **Message-id idempotency** absorbs Meta's webhook redeliveries · **exponential backoff + full-jitter retries** with transient-vs-permanent error classification
- 🚦 WhatsApp's **24-hour policy enforced at a single outbound choke point** with graceful degradation — policy limits never crash the service
- 🗄️ **16-entity Prisma/PostgreSQL schema** · timezone-aware cron jobs · runs fully **credential-free in stub mode**

<br/>

### ☕ Java / Spring Boot Backends

<div align="center">

<a href="https://github.com/Eswar809/student-management"><img src="https://img.shields.io/badge/%F0%9F%93%A6_student--management-Spring_Security_%C2%B7_Docker_%C2%B7_race--condition_tests-E76F00?style=for-the-badge&labelColor=0B1221" alt="student-management — Spring Security, Docker, race-condition tests"/></a>

<a href="https://github.com/Eswar809/Complaint-Management-System"><img src="https://img.shields.io/badge/%F0%9F%93%A6_Complaint--Management--System-15_REST_endpoints_%C2%B7_React_%C2%B7_3--dev_team-4285F4?style=for-the-badge&labelColor=0B1221" alt="Complaint-Management-System — 15 REST endpoints, React, 3-dev team"/></a>

</div>

<details>
<summary><b>⚙️ Engineering highlights inside these repos</b></summary>
<br/>

- 🎓 **student-management** — role-based academic portal · **database-level race-condition fix** proven by a concurrency test · Hibernate **N+1 fix** with a regression guard · Spring Security · Docker with MySQL health check
- 📋 **Complaint-Management-System** — **15-endpoint** Spring Boot REST API + React · centralized CORS policy bean · authored the CI configs (GitHub Actions workflow + Jenkinsfile) · built in a 3-person team via PRs & code reviews

</details>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00F5A0,25:00D9F5,50:8B5CF6,75:FF6EC7,100:FFB86C&height=4" width="100%" alt=""/>

## 🌱 Open Source

**[google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli/pulls?q=is%3Apr+author%3AEswar809)** — contributing to **Google's official Gemini CLI**

<img src="https://img.shields.io/badge/PRs_submitted-12-00D9F5?style=flat-square&labelColor=0B1221" alt="12 PRs submitted"/> <img src="https://img.shields.io/badge/merged-fix%28core%29_%2326884-00F5A0?style=flat-square&labelColor=0B1221" alt="PR 26884 merged"/> <img src="https://img.shields.io/badge/currently_open-3-8B5CF6?style=flat-square&labelColor=0B1221" alt="3 PRs open"/>

- ✅ [**PR #26884 — merged**](https://github.com/google-gemini/gemini-cli/pull/26884) · `fix(core): ignore .pak & .rpa game archives by default` — **approved by a Google maintainer**, picked up from a *help-wanted* issue
- 📬 **12 PRs submitted** · **3 currently open**

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00F5A0,25:00D9F5,50:8B5CF6,75:FF6EC7,100:FFB86C&height=4" width="100%" alt=""/>

## 🏆 Achievements

|  |  |
|:--|:--|
| 🥇 **TCS CodeVita Season 13 (2025)** | **Global Rank 2028** of **100,000+** participants — **Top ~2%** |
| 🧮 **LeetCode** | **[170+ problems solved](https://leetcode.com/u/Eswardeevi/)** · 90+ Medium & Hard |
| ☁️ **Google Cloud Skills Boost** | **Gold League** · **21,010 pts** · **25+ badges** |
| 📜 **Certifications** | **NPTEL Java (IIT)** · **AICTE-EduSkills AI/ML** |

<div align="center">

<img src="https://leetcard.jacoblin.cool/Eswardeevi?theme=dark&font=JetBrains+Mono&ext=heatmap" alt="LeetCode stats card"/>

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00F5A0,25:00D9F5,50:8B5CF6,75:FF6EC7,100:FFB86C&height=4" width="100%" alt=""/>

## 🛠️ Tech Stack

<div align="center">
<sub>⚡ hand-built animated icons — they draw themselves as the page loads</sub>
<br/><br/>

<table>
<tr>
<td align="right"><b>⚙️ Backend</b></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/java.svg" alt="Java"/><br/><sub><b>Java</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/spring.svg" alt="Spring Boot"/><br/><sub><b>Spring</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/nodejs.svg" alt="Node.js"/><br/><sub><b>Node.js</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/python.svg" alt="Python"/><br/><sub><b>Python</b></sub></td>
<td></td>
</tr>
<tr>
<td align="right"><b>🌐 Web</b></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/typescript.svg" alt="TypeScript"/><br/><sub><b>TypeScript</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/javascript.svg" alt="JavaScript"/><br/><sub><b>JavaScript</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/react.svg" alt="React"/><br/><sub><b>React</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/nextjs.svg" alt="Next.js"/><br/><sub><b>Next.js</b></sub></td>
<td></td>
</tr>
<tr>
<td align="right"><b>🗄️ Data</b></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/postgresql.svg" alt="PostgreSQL"/><br/><sub><b>PostgreSQL</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/mysql.svg" alt="MySQL"/><br/><sub><b>MySQL</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/prisma.svg" alt="Prisma"/><br/><sub><b>Prisma</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/supabase.svg" alt="Supabase"/><br/><sub><b>Supabase</b></sub></td>
<td></td>
</tr>
<tr>
<td align="right"><b>☁️ Cloud · AI · Tools</b></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/gcp.svg" alt="Google Cloud"/><br/><sub><b>G Cloud</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/gemini.svg" alt="Gemini AI"/><br/><sub><b>Gemini</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/docker.svg" alt="Docker"/><br/><sub><b>Docker</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/git.svg" alt="Git"/><br/><sub><b>Git</b></sub></td>
<td align="center" width="86"><img width="40" height="40" src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/icons/github.svg" alt="GitHub"/><br/><sub><b>GitHub</b></sub></td>
</tr>
</table>

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00F5A0,25:00D9F5,50:8B5CF6,75:FF6EC7,100:FFB86C&height=4" width="100%" alt=""/>

<!-- 🐍 Contribution snake — DISABLED: GitHub Actions is blocked by an account billing lock,
     so .github/workflows/snake.yml can't run and the output branch doesn't exist yet.
     After fixing billing (github.com/settings/billing), run the "Generate snake animation"
     workflow once from the Actions tab, then paste this block back (inside a centered div):

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Eswar809/Eswar809/output/github-contribution-grid-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Eswar809/Eswar809/output/github-contribution-grid-snake.svg"/>
  <img src="https://raw.githubusercontent.com/Eswar809/Eswar809/output/github-contribution-grid-snake.svg" alt="Contribution snake animation" width="100%"/>
</picture>
-->

<!-- ═══════════════════════════ FOOTER CTA ═══════════════════════════ -->
<div align="center">

## 💼 Open to Software Engineer roles

**Backend · AI/LLM Systems · Full-Stack** &nbsp;·&nbsp; Class of 2026 &nbsp;·&nbsp; 📍 India, open to relocation

<br/>

<a href="mailto:deevieswar44@gmail.com"><img src="https://img.shields.io/badge/deevieswar44@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email me"/></a>&nbsp;
<a href="https://www.linkedin.com/in/eswar-dev-55a54536a/"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn"/></a>

<br/>

<sub>⚡ Fastest response: email</sub>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=Eswar809&style=flat-square&color=00D9F5&label=profile+views" alt="Profile views"/>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00F5A0,25:00D9F5,50:8B5CF6,75:FF6EC7,100:FFB86C&height=130&section=footer" width="100%" alt=""/>
