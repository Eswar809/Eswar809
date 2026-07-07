<!-- ═══════════════════════════ HEADER ═══════════════════════════ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&height=230&color=0:0f0c29,30:24243e,60:5b21b6,100:7aa2f7&text=Deevi%20Eswar&fontSize=62&fontColor=FFFFFF&animation=fadeIn&fontAlignY=42&desc=Backend%20%26%20AI%20Engineer%20%C2%B7%20systems%20that%20survive%20production&descSize=18&descAlignY=64" width="100%" alt="Deevi Eswar — Backend & AI Engineer"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=22&duration=2600&pause=850&color=7AA2F7&center=true&vCenter=true&width=700&height=48&lines=%E2%9A%A1+Event-driven+systems+that+don%27t+drop+messages;%F0%9F%9A%80+AI+products+running+live+in+production;%E2%9C%85+Merged+PR+%40+google-gemini%2Fgemini-cli;%F0%9F%8E%AF+SWE+%C2%B7+Class+of+2026+%C2%B7+Backend+%2F+AI" alt="Event-driven systems · AI in production · Merged PR @ google-gemini/gemini-cli"/>

<br/>

<img src="https://img.shields.io/badge/%F0%9F%9F%A2_OPEN_TO_WORK-Software_Engineer_%C2%B7_2026-16a34a?style=for-the-badge&labelColor=0d1117" alt="Open to work — Software Engineer, 2026"/>

<br/><br/>

<a href="https://devs-portiofolio.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-302b63?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>&nbsp;
<a href="https://www.linkedin.com/in/eswar-dev-55a54536a/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>&nbsp;
<a href="https://leetcode.com/u/Eswardeevi/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode"/></a>&nbsp;
<a href="mailto:deevieswar44@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>

<br/><br/>

<!-- ── 7-second proof strip — the three things a recruiter must see ── -->

| 🚀 **Shipping to production** | 🌱 **Open source @ Google** | 🏆 **Top 2% of 100K+** |
|:---:|:---:|:---:|
| AI grader **used daily by faculty**<br/>**~85% cheaper** than human evaluation | **Merged PR** in `google-gemini/gemini-cli`<br/>approved by a Google maintainer | **TCS CodeVita S13** · Global Rank **2028**<br/>among **100,000+** participants |

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f0c29,50:7aa2f7,100:bb9af7&height=3" width="100%" alt=""/>

## 👨‍💻 About Me

- 🎓 **B.Tech — Artificial Intelligence & Data Science**, Class of **2026**
- 💼 Looking for **Software Engineer (Backend / AI)** roles · 📍 India, **open to relocation**
- ⚡ I obsess over the unglamorous things that keep systems alive — **idempotency, retries with jitter, race conditions, webhook security, prompt-cost engineering**
- 📫 Fastest way to reach me → **[deevieswar44@gmail.com](mailto:deevieswar44@gmail.com)**

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f0c29,50:7aa2f7,100:bb9af7&height=3" width="100%" alt=""/>

## 🚀 Featured Builds

<div align="center"><samp>— things that run without me babysitting them —</samp></div>

<br/>

### 📄 PaperCheck AI

<a href="https://paper-checking.netlify.app/"><img src="https://img.shields.io/badge/%E2%96%B6_Open_Live_App-paper--checking.netlify.app-7aa2f7?style=flat-square&labelColor=0d1117" alt="Open live app"/></a> <img src="https://img.shields.io/badge/Live_in_Production-16a34a?style=flat-square" alt="Live in production"/>

> **AI exam-grading platform** — grades batches of handwritten CA/CS answer sheets **in parallel** (one streaming AI worker per student) and returns **annotated, examiner-style PDFs**. In active daily use by coaching faculty.

- 💸 **~85% cheaper than human evaluation** — ₹15–21/paper vs the ₹100–190 evaluators charge, in **minutes instead of 2–3 days**
- 🧠 **Two prompt-caching layers** — SHA-256-keyed explicit cache (6 h TTL) + `cache_control` prefix reuse to hold cost down
- 🛡️ **Layered reliability** — 10-step jittered exponential backoff · zero-output-gated stream restarts (**no paper graded twice**) · bounded auto-resume for paused long runs
- ⚡ **Browser-direct streaming** — multi-minute model runs never hit serverless timeouts

<br/>

### 💬 Event-Driven WhatsApp Messaging Platform

<a href="https://github.com/Eswar809/whatsapp-messaging-platform"><img src="https://img.shields.io/badge/%E2%96%B6_View_Source-GitHub-7aa2f7?style=flat-square&labelColor=0d1117&logo=github" alt="View source on GitHub"/></a> <img src="https://img.shields.io/badge/Official_WhatsApp_Cloud_API-25D366?style=flat-square&logo=whatsapp&logoColor=white" alt="Official WhatsApp Cloud API"/>

> **24/7 admissions automation** — FAQs, demo booking, payments, doubt triage to faculty, and a daily MCQ engine.

- 🔐 **HMAC-SHA256-verified webhooks** (constant-time compare) · fast ACK + async processing
- ♻️ **Message-id idempotency** absorbs Meta's webhook redeliveries · **exponential backoff + full-jitter retries** with transient-vs-permanent error classification
- 🚦 WhatsApp's **24-hour policy enforced at a single outbound choke point** with graceful degradation — policy limits never crash the service
- 🗄️ **16-entity Prisma/PostgreSQL schema** · timezone-aware cron jobs · runs fully **credential-free in stub mode**

<br/>

### ☕ Java / Spring Boot Backends

<div align="center">

<a href="https://github.com/Eswar809/student-management"><img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=Eswar809&repo=student-management&theme=tokyonight&hide_border=true" alt="student-management"/></a>
&nbsp;
<a href="https://github.com/Eswar809/Complaint-Management-System"><img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=Eswar809&repo=Complaint-Management-System&theme=tokyonight&hide_border=true" alt="Complaint-Management-System"/></a>

</div>

<details>
<summary><b>⚙️ Engineering highlights inside these repos</b></summary>
<br/>

- 🎓 **student-management** — role-based academic portal · **database-level race-condition fix** proven by a concurrency test · Hibernate **N+1 fix** with a regression guard · Spring Security · Docker with MySQL health check
- 📋 **Complaint-Management-System** — **15-endpoint** Spring Boot REST API + React · centralized CORS policy bean · **GitHub Actions + Jenkins CI** · built in a 3-person team via PRs & code reviews

</details>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f0c29,50:7aa2f7,100:bb9af7&height=3" width="100%" alt=""/>

## 🌱 Open Source

**[google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli/pulls?q=is%3Apr+author%3AEswar809)** — contributing to **Google's official Gemini CLI**

<img src="https://img.shields.io/badge/PRs_submitted-12-7aa2f7?style=flat-square&labelColor=0d1117" alt="12 PRs submitted"/> <img src="https://img.shields.io/badge/merged-fix%28core%29_%2326884-16a34a?style=flat-square&labelColor=0d1117" alt="PR 26884 merged"/> <img src="https://img.shields.io/badge/currently_open-3-eab308?style=flat-square&labelColor=0d1117" alt="3 PRs open"/>

- ✅ [**PR #26884 — merged**](https://github.com/google-gemini/gemini-cli/pull/26884) · `fix(core)`, **approved by a Google maintainer**, picked up from a *help-wanted* issue
- 📬 **12 PRs submitted** · **3 currently open**

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f0c29,50:7aa2f7,100:bb9af7&height=3" width="100%" alt=""/>

## 🏆 Achievements

|  |  |
|:--|:--|
| 🥇 **TCS CodeVita Season 13 (2025)** | **Global Rank 2028** of **100,000+** participants — **Top 2%** |
| 🧮 **LeetCode** | **150+ problems** solved |
| ☁️ **Google Cloud Skills Boost** | **Gold League** · **21,010 pts** · **25+ badges** |

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f0c29,50:7aa2f7,100:bb9af7&height=3" width="100%" alt=""/>

## 🛠️ Tech Stack

<div align="center">

<table>
<tr><td align="right"><b>⚙️ &nbsp;Backend</b></td><td><img src="https://skillicons.dev/icons?i=java,spring,nodejs,py" alt="Java, Spring Boot, Node.js, Python"/></td></tr>
<tr><td align="right"><b>🌐 &nbsp;Web</b></td><td><img src="https://skillicons.dev/icons?i=ts,react,nextjs" alt="TypeScript, React, Next.js"/></td></tr>
<tr><td align="right"><b>🗄️ &nbsp;Data</b></td><td><img src="https://skillicons.dev/icons?i=postgres,mysql,prisma" alt="PostgreSQL, MySQL, Prisma"/></td></tr>
<tr><td align="right"><b>☁️ &nbsp;Cloud &amp; DevOps</b></td><td><img src="https://skillicons.dev/icons?i=gcp,docker,githubactions,git" alt="Google Cloud, Docker, GitHub Actions, Git"/></td></tr>
</table>

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f0c29,50:7aa2f7,100:bb9af7&height=3" width="100%" alt=""/>

## 📈 Numbers Don't Lie

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Eswar809&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" alt="GitHub stats"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Eswar809&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages"/>

<br/><br/>

<img src="https://streak-stats.demolab.com?user=Eswar809&theme=tokyonight&hide_border=true" alt="GitHub streak"/>

<br/><br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Eswar809&theme=tokyo-night&hide_border=true&area=true&radius=8" width="100%" alt="Contribution activity graph"/>

<br/><br/>

<img src="https://leetcard.jacoblin.cool/Eswardeevi?theme=dark&font=JetBrains+Mono&ext=heatmap" alt="LeetCode stats"/>

<br/><br/>

<img src="https://github-profile-trophy.vercel.app/?username=Eswar809&theme=tokyonight&no-frame=true&no-bg=true&row=1&column=7&margin-w=8" alt="GitHub trophies"/>

<br/><br/>

<!-- 🐍 Generated by .github/workflows/snake.yml — appears after the action runs once -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Eswar809/Eswar809/output/github-contribution-grid-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Eswar809/Eswar809/output/github-contribution-grid-snake.svg"/>
  <img src="https://raw.githubusercontent.com/Eswar809/Eswar809/output/github-contribution-grid-snake.svg" alt="Contribution snake animation" width="100%"/>
</picture>

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f0c29,50:7aa2f7,100:bb9af7&height=3" width="100%" alt=""/>

<!-- ═══════════════════════════ FOOTER CTA ═══════════════════════════ -->
<div align="center">

## 💼 Open to Software Engineer roles

**Backend · AI/LLM Systems · Distributed Messaging** &nbsp;·&nbsp; Class of 2026 &nbsp;·&nbsp; 📍 India, open to relocation

<br/>

<a href="mailto:deevieswar44@gmail.com"><img src="https://img.shields.io/badge/deevieswar44@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email me"/></a>&nbsp;
<a href="https://www.linkedin.com/in/eswar-dev-55a54536a/"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn"/></a>

<br/>

<sub>⚡ Fastest response: email</sub>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=Eswar809&style=flat-square&color=7AA2F7&label=profile+views" alt="Profile views"/>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,30:24243e,60:5b21b6,100:7aa2f7&height=120&section=footer" width="100%" alt=""/>
