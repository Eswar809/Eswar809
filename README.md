<!-- Banner: commit hero-dark.svg and hero-light.svg to assets/ in this repo -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/hero-dark.svg">
  <img src="https://raw.githubusercontent.com/Eswar809/Eswar809/main/assets/hero-light.svg" alt="Deevi Eswar — Backend & AI engineer. I build systems that survive production." width="100%">
</picture>

<p align="center">
  <a href="https://devs-portiofolio.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-2D333B?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio"></a>&nbsp;
  <a href="https://www.linkedin.com/in/eswar-dev-55a54536a/"><img src="https://img.shields.io/badge/LinkedIn-2D333B?style=flat-square&logoColor=white" alt="LinkedIn"></a>&nbsp;
  <a href="https://leetcode.com/u/Eswardeevi/"><img src="https://img.shields.io/badge/LeetCode-2D333B?style=flat-square&logo=leetcode&logoColor=white" alt="LeetCode"></a>&nbsp;
  <a href="mailto:deevieswar44@gmail.com"><img src="https://img.shields.io/badge/Email-2D333B?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
</p>

B.Tech CSE (AI & Data Science), Class of 2026. Looking for my first full-time **Software Engineer role** — backend, full-stack, or AI. Based in India, open to relocation.

I like the unglamorous parts of software: idempotent webhooks, retries with jitter, race conditions, token budgets. The work nobody notices until it's missing.

<br>

## The short version

1. **My software is in production.** [PaperCheck AI](https://paper-checking.netlify.app/) grades handwritten CA/CS answer sheets and is used daily by coaching faculty — ₹15–21 per paper against the ₹100–190 human evaluators charge, in minutes instead of 2–3 days.
2. **Google merged my code.** [PR #26884](https://github.com/google-gemini/gemini-cli/pull/26884) in `google-gemini/gemini-cli`, approved by a Google maintainer — picked up from a *help-wanted* issue.
3. **TCS CodeVita Season 13:** global rank 2028 out of 100,000+ participants — top ~2%.

<br>

## Projects

### PaperCheck AI — [live](https://paper-checking.netlify.app/)

Grades batches of handwritten CA/CS answer sheets in parallel — one streaming AI worker per student — and returns annotated, examiner-style PDFs. In active daily use.

- Layered reliability: 10-step jittered exponential backoff, zero-output-gated stream restarts (no paper graded twice), bounded auto-resume for paused long runs
- Browser-direct streaming, so multi-minute model runs never hit serverless timeouts
- SHA-256-keyed prompt cache (6 h TTL), 50 MB signed-token PDF uploads, strict token budgeting on Gemini Flash

### CA GURU — [live](https://ca-study.netlify.app/)

An all-in-one learning platform for CA students: AI tutoring over chat, voice, and TTS, a notes library, a social feed with DMs and stories, study rooms, leaderboards.

- ~85K lines of TypeScript — Next.js + React 19, 29+ API routes, 26+ dashboard pages
- Security enforced at the database: 34 tables, 85 row-level-security policies, 18 `SECURITY DEFINER` RPCs on Supabase Postgres
- Three-model Gemini fallback cascade (a degraded answer beats downtime), SSE streaming chat, per-IP sliding-window rate limits with `Retry-After`

### WhatsApp messaging platform — [source](https://github.com/Eswar809/whatsapp-messaging-platform)

Event-driven admissions automation on the official WhatsApp Cloud API: FAQs, demo booking, payments, doubt triage to faculty, and a daily MCQ engine.

- HMAC-SHA256-verified webhooks with constant-time compare; fast ACK, async processing
- Message-id idempotency absorbs Meta's webhook redeliveries; full-jitter retries with transient-vs-permanent error classification
- WhatsApp's 24-hour messaging rule enforced at a single outbound choke point; 16-entity Prisma/PostgreSQL schema; runs credential-free in stub mode

### Spring Boot backends

A role-based academic portal, and a 15-endpoint complaint system built in a three-person team through PRs and code review. Database-level race-condition fix proven by a concurrency test, Hibernate N+1 fix with a regression guard, Spring Security, Docker with MySQL health checks, CI via GitHub Actions and Jenkins.

<p>
  <a href="https://github.com/Eswar809/student-management"><img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=Eswar809&repo=student-management&hide_border=true&bg_color=00000000&title_color=58A6FF&icon_color=3FB950&text_color=8B949E" alt="student-management"></a>
  <a href="https://github.com/Eswar809/Complaint-Management-System"><img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=Eswar809&repo=Complaint-Management-System&hide_border=true&bg_color=00000000&title_color=58A6FF&icon_color=3FB950&text_color=8B949E" alt="Complaint-Management-System"></a>
</p>

<br>

## Open source

Contributing to [google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli) — Google's official Gemini CLI.

- [PR #26884, merged](https://github.com/google-gemini/gemini-cli/pull/26884) — `fix(core): ignore .pak & .rpa game archives by default`, approved by a Google maintainer
- [12 PRs submitted, 3 currently open](https://github.com/google-gemini/gemini-cli/pulls?q=is%3Apr+author%3AEswar809)

<br>

## Achievements

|  |  |
|:--|:--|
| **TCS CodeVita Season 13** | Global rank 2028 of 100,000+ — top ~2% |
| **LeetCode** | [150+ problems solved](https://leetcode.com/u/Eswardeevi/) |
| **Google Cloud Skills Boost** | Gold League · 21,010 pts · 25+ badges |
| **Certifications** | NPTEL Java (IIT) · AICTE-EduSkills AI/ML |

<br>

## Stack

<table>
  <tr><td align="right"><b>Backend</b></td><td><img src="https://skillicons.dev/icons?i=java,spring,nodejs,express,py" height="36" alt="Java, Spring Boot, Node.js, Express, Python"></td></tr>
  <tr><td align="right"><b>Web</b></td><td><img src="https://skillicons.dev/icons?i=ts,js,react,nextjs" height="36" alt="TypeScript, JavaScript, React, Next.js"></td></tr>
  <tr><td align="right"><b>Data</b></td><td><img src="https://skillicons.dev/icons?i=postgres,mysql,prisma,supabase" height="36" alt="PostgreSQL, MySQL, Prisma, Supabase"></td></tr>
  <tr><td align="right"><b>Cloud</b></td><td><img src="https://skillicons.dev/icons?i=gcp,docker,githubactions,git" height="36" alt="Google Cloud, Docker, GitHub Actions, Git"></td></tr>
</table>

<br>

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Eswar809&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&bg_color=00000000&title_color=58A6FF&icon_color=3FB950&text_color=8B949E&ring_color=3FB950" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Eswar809&layout=compact&langs_count=6&hide_border=true&bg_color=00000000&title_color=58A6FF&text_color=8B949E" alt="Top languages">
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=Eswar809&theme=transparent&hide_border=true&ring=3FB950&fire=3FB950&currStreakNum=58A6FF&sideNums=58A6FF&currStreakLabel=8B949E&sideLabels=8B949E&dates=8B949E" alt="GitHub streak">
</p>

<br>

---

<p align="center">
  If this sounds like your team's kind of work — <a href="mailto:deevieswar44@gmail.com"><b>deevieswar44@gmail.com</b></a> gets the fastest reply.
</p>
