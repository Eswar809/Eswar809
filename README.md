<!-- ═══════════════════════════ HEADER ═══════════════════════════ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=210&section=header&text=Deevi%20Eswar&fontSize=58&fontColor=FFFFFF&animation=fadeIn&fontAlignY=32&desc=Backend%20%26%20AI%20Engineer%20%C2%B7%20I%20ship%20systems%20that%20survive%20production&descSize=17&descAlignY=54" width="100%" alt="Deevi Eswar — Backend & AI Engineer"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2800&pause=900&color=7AA2F7&center=true&vCenter=true&width=640&height=45&lines=Event-driven+messaging+systems+%E2%9A%A1;AI+products+running+live+in+production+%F0%9F%9A%80;Merged+contributor+%40+google-gemini%2Fgemini-cli+%E2%9C%85;Open+to+SWE+roles+%C2%B7+Class+of+2026+%F0%9F%8E%93" alt="Event-driven messaging systems · AI products in production · Merged contributor @ google-gemini/gemini-cli"/>

<br/>

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

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%" alt=""/>

## 👨‍💻 About Me

- 🎓 **B.Tech — Artificial Intelligence & Data Science**, Class of **2026**
- 💼 Looking for **Software Engineer (Backend / AI)** roles · 📍 India, **open to relocation**
- ⚡ I obsess over the unglamorous things that keep systems alive — **idempotency, retries with jitter, race conditions, webhook security, prompt-cost engineering**
- 📫 Fastest way to reach me → **[deevieswar44@gmail.com](mailto:deevieswar44@gmail.com)**

<br/>

## 🚀 Featured Builds

### 📄 [PaperCheck AI](https://paper-checking.netlify.app/) · ![Live in Production](https://img.shields.io/badge/Live_in_Production-16a34a?style=flat-square)

> **AI exam-grading platform** — grades batches of handwritten CA/CS answer sheets **in parallel** (one streaming AI worker per student) and returns **annotated, examiner-style PDFs**. In active daily use by coaching faculty.

- 💸 **~85% cheaper than human evaluation** — ₹15–21/paper vs the ₹100–190 evaluators charge, in **minutes instead of 2–3 days**
- 🧠 **Two prompt-caching layers** — SHA-256-keyed explicit cache (6 h TTL) + `cache_control` prefix reuse to hold cost down
- 🛡️ **Layered reliability** — 10-step jittered exponential backoff · zero-output-gated stream restarts (**no paper graded twice**) · bounded auto-resume for paused long runs
- ⚡ **Browser-direct streaming** — multi-minute model runs never hit serverless timeouts

<br/>

### 💬 [Event-Driven WhatsApp Messaging Platform](https://github.com/Eswar809/whatsapp-messaging-platform) · ![Official WhatsApp Cloud API](https://img.shields.io/badge/Official_WhatsApp_Cloud_API-25D366?style=flat-square&logo=whatsapp&logoColor=white)

> **24/7 admissions automation** — FAQs, demo booking, payments, doubt triage to faculty, and a daily MCQ engine.

- 🔐 **HMAC-SHA256-verified webhooks** (constant-time compare) · fast ACK + async processing
- ♻️ **Message-id idempotency** absorbs Meta's webhook redeliveries · **exponential backoff + full-jitter retries** with transient-vs-permanent error classification
- 🚦 WhatsApp's **24-hour policy enforced at a single outbound choke point** with graceful degradation — policy limits never crash the service
- 🗄️ **16-entity Prisma/PostgreSQL schema** · timezone-aware cron jobs · runs fully **credential-free in stub mode**

<br/>

### ☕ Java / Spring Boot Backends

| Repository | What's inside |
|:--|:--|
| 🎓 [**student-management**](https://github.com/Eswar809/student-management) | Role-based academic portal — **database-level race-condition fix** proven by a concurrency test · Hibernate **N+1 fix** with a regression guard · Spring Security · Docker with MySQL health check |
| 📋 [**Complaint-Management-System**](https://github.com/Eswar809/Complaint-Management-System) | **15-endpoint** Spring Boot REST API + React · centralized CORS policy bean · **GitHub Actions + Jenkins CI** · built in a 3-person team via PRs & code reviews |

<br/>

## 🌱 Open Source

**[google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli/pulls?q=is%3Apr+author%3AEswar809)** — contributing to **Google's official Gemini CLI**

- ✅ [**PR #26884 — merged**](https://github.com/google-gemini/gemini-cli/pull/26884) · `fix(core)`, **approved by a Google maintainer**, picked up from a *help-wanted* issue
- 📬 **12 PRs submitted** · **3 currently open**

<br/>

## 🏆 Achievements

|  |  |
|:--|:--|
| 🥇 **TCS CodeVita Season 13 (2025)** | **Global Rank 2028** of **100,000+** participants — **Top 2%** |
| 🧮 **LeetCode** | **150+ problems** solved |
| ☁️ **Google Cloud Skills Boost** | **Gold League** · **21,010 pts** · **25+ badges** |
| 🧪 **LLM evaluation engineering** | [**rag-eval-pipeline**](https://github.com/Eswar809/rag-eval-pipeline) — merge-blocking CI quality gates · chunking retune lifted Faithfulness **0.45 → 0.82** |

<br/>

## 🛠️ Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=java,spring,py,ts,nodejs,nextjs,react,postgres,mysql,prisma,docker,githubactions,gcp,git&perline=7" alt="Java · Spring Boot · Python · TypeScript · Node.js · Next.js · React · PostgreSQL · MySQL · Prisma · Docker · GitHub Actions · Google Cloud · Git"/>

</div>

<br/>

## 📊 Analytics

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Eswar809&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" alt="GitHub stats"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Eswar809&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages"/>

<br/><br/>

<img src="https://streak-stats.demolab.com?user=Eswar809&theme=tokyonight&hide_border=true" alt="GitHub streak"/>

<br/><br/>

<img src="https://leetcard.jacoblin.cool/Eswardeevi?theme=dark&font=JetBrains+Mono&ext=heatmap" alt="LeetCode stats"/>

<br/><br/>

<img src="https://github-profile-trophy.vercel.app/?username=Eswar809&theme=tokyonight&no-frame=true&no-bg=true&row=1&column=7&margin-w=8" alt="GitHub trophies"/>

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%" alt=""/>

<!-- ═══════════════════════════ FOOTER CTA ═══════════════════════════ -->
<div align="center">

## 💼 Open to Software Engineer roles

**Backend · AI/LLM Systems · Distributed Messaging** &nbsp;·&nbsp; Class of 2026 &nbsp;·&nbsp; 📍 India, open to relocation

<br/>

<a href="mailto:deevieswar44@gmail.com"><img src="https://img.shields.io/badge/deevieswar44@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email me"/></a>&nbsp;
<a href="https://www.linkedin.com/in/eswar-dev-55a54536a/"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn"/></a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=Eswar809&style=flat-square&color=7AA2F7&label=profile+views" alt="Profile views"/>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=110&section=footer" width="100%" alt=""/>
