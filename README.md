<!-- ═══════════════ HEADER (animated wave) ═══════════════ -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=venom&color=0:0f2027,50:203a43,100:2c5364&height=250&section=header&text=SIDDAROODH&fontSize=68&fontColor=ffffff&animation=fadeIn&fontAlignY=40&desc=Backend%20Engineer%20%7C%20Java%20%C2%B7%20Spring%20Boot%20%C2%B7%20PostgreSQL&descSize=19&descAlignY=64&descColor=00D4FF" alt="header" />
</p>

<!-- ═══════════════ TYPING ANIMATION ═══════════════ -->
<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=900&color=00D4FF&center=true&vCenter=true&width=900&lines=Concurrency-safe+backend+systems%2C+end+to+end;Java+%7C+Spring+Boot+%7C+PostgreSQL+%7C+Redis;I+prove+it+with+load+tests%2C+not+%22it+runs+on+my+machine%22;2026+B.Tech+CSE+%40+Alliance+University;Open+to+Backend+Engineer+%2F+SDE+Intern+roles" alt="Typing animation" />
  </a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=siddaroodh05&style=for-the-badge&color=0E75B6&label=PROFILE+VIEWS" alt="Profile views" />
  <img src="https://img.shields.io/badge/OPEN%20TO-Backend%20%2F%20SDE%20Intern-28A745?style=for-the-badge" alt="Open to work" />
  <img src="https://img.shields.io/badge/OCI%202025-GenAI%20Professional-FF1744?style=for-the-badge&logo=oracle&logoColor=white" alt="OCI" />
</p>

<p align="center">
  <a href="mailto:siddaroodh2004@gmail.com"><img src="https://img.shields.io/badge/Gmail-siddaroodh2004%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/siddaroodh-venkatapur-821551262/"><img src="https://img.shields.io/badge/LinkedIn-Siddaroodh-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://siddaroodh-portfolio.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-Visit-FF6B6B?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://leetcode.com/u/siddaroodh__2004/"><img src="https://img.shields.io/badge/LeetCode-siddaroodh__2004-FFA116?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f2027,50:00D4FF,100:0f2027&height=3&section=header" width="80%" alt="divider" />
</p>

<!-- ═══════════════ TERMINAL CARD ═══════════════ -->
## 👨‍💻 `whoami`

```bash
$ whoami
siddaroodh — backend engineer

$ cat about.txt
 role      : Backend Engineer / SDE Intern (open to opportunities)
 education : B.Tech CSE, Alliance University, Bengaluru (2026)
 focus     : architecture · authN/authZ · transaction consistency · concurrency
 mindset   : "If I can't load-test it, I don't trust it."

$ ls ./now
 core-banking-system/       # microservices, JWT, RBAC, optimistic locking
 game-recommendation-rag/   # RAG-based game recommender (in progress)

$ cat achievements.txt
 ✔ 300+ DSA problems solved on LeetCode (Java)
 ✔ Gold-rated on HackerRank (Python)
 ✔ OCI 2025 Certified Generative AI Professional
```

<!-- ═══════════════ IMPACT METRICS ═══════════════ -->
## 📈 Proven, Not Promised

<table align="center">
  <tr>
    <td align="center" width="25%">
      <h1>0</h1>
      <b>data leaks</b><br/>
      <sub>10 simultaneous requests,<br/>2 users sharing an idempotency key</sub>
    </td>
    <td align="center" width="25%">
      <h1>100%</h1>
      <b>balance accuracy</b><br/>
      <sub>35 concurrent requests<br/>with optimistic locking</sub>
    </td>
    <td align="center" width="25%">
      <h1>0</h1>
      <b>duplicate transactions</b><br/>
      <sub>10 concurrent duplicates,<br/>DB-enforced idempotency</sub>
    </td>
    <td align="center" width="25%">
      <h1>30+</h1>
      <b>REST endpoints</b><br/>
      <sub>Auth · Account · Transaction<br/>services</sub>
    </td>
  </tr>
</table>

<!-- ═══════════════ FEATURED PROJECT ═══════════════ -->
## 🏦 Core Banking System

> A microservices banking backend built around **correctness under concurrency**, not just CRUD.

```mermaid
flowchart LR
    C([Client]) --> G{{API Gateway<br/>JWT check · routing}}
    G -. "Redis rate limit<br/>25 req / 2 min per user" .-> R[(Redis)]
    G --> A[Auth Service<br/>JWT + refresh rotation]
    G --> B[Account Service<br/>optimistic locking]
    G --> T[Transaction Service<br/>idempotent requests]
    A --> DA[(Auth DB)]
    B --> DB[(Account DB)]
    T --> DT[(Transaction DB)]
```

<sub>Database-per-service: each microservice owns its own PostgreSQL database.</sub>

<details open>
<summary><b>🔐 Security & Correctness Highlights</b></summary>
<br/>

| Area | What I built |
| :-- | :-- |
| **Authorization** | Fixed a cross-user gap in idempotent request handling and verified it with a concurrent 2-user test |
| **Consistency** | Optimistic locking for transaction consistency under 35 concurrent requests |
| **Idempotency** | Database-enforced key handling that removes duplicate processing |
| **Auth** | JWT with refresh-token rotation and RBAC |
| **Gateway** | Centralized routing and Redis rate limiting with structured `429` responses |

</details>

<p>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <a href="https://github.com/digital-banking-platform/Core-Banking-System"><img src="https://img.shields.io/badge/View%20Repo-181717?style=flat-square&logo=github&logoColor=white" /></a>
</p>

---

## 🤖 ATS Launchpad

> AI-powered ATS: resume analysis, job matching, skill-gap detection and resume-based skill tests.

- 🧠 **GPT-OSS-20B** via Spring AI for resume/job-fit analysis and skill-gap detection
- ⚡ **Real-time SSE streaming** with JWT-based auth for progressive result delivery
- 📄 **Apache Tika** for resume parsing across document formats

<p>
  <img src="https://img.shields.io/badge/Java%2017-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring%20AI-6DB33F?style=flat-square&logo=spring&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <a href="https://github.com/siddaroodh05/ATS-Launchpad"><img src="https://img.shields.io/badge/View%20Repo-181717?style=flat-square&logo=github&logoColor=white" /></a>
</p>

---

## 🎮 Currently Building: RAG Game Recommendation System

Retrieval-augmented game recommendations, with LLM-generated queries and vector search.

<a href="https://github.com/siddaroodh05/rag-game-recommendation-system"><img src="https://img.shields.io/badge/Status-In%20Progress-FFD700?style=for-the-badge" alt="In progress" /></a>

---

## 🧰 Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,postgres,redis,docker,git,github,react,python,postman&perline=10" alt="Tech stack" />
</p>

<table align="center">
  <tr><td><b>Languages</b></td><td>Java · SQL · Python</td></tr>
  <tr><td><b>Backend</b></td><td>Spring Boot · Spring Security · Spring Data JPA · Hibernate · REST · Microservices · API Gateway</td></tr>
  <tr><td><b>Data</b></td><td>PostgreSQL · Redis</td></tr>
  <tr><td><b>Tools</b></td><td>Git · GitHub · Docker · Postman</td></tr>
  <tr><td><b>Frontend</b></td><td>React.js</td></tr>
  <tr><td><b>Core CS</b></td><td>DSA · OOP · DBMS · Operating Systems · Computer Networks</td></tr>
</table>

---

## 📂 More Projects

| Project | Description |
| :-- | :-- |
| [**rag-game-recommendation-system**](https://github.com/siddaroodh05/rag-game-recommendation-system) | Retrieval-augmented generation for game recommendations |
| [**Stock-Portfolio-Optimization**](https://github.com/siddaroodh05/Stock-Portfolio-Optimization) | Portfolio optimization in Python / Jupyter |
| [**DMart-Clone-React**](https://github.com/siddaroodh05/DMart-Clone-React-E-Commerce-Web-Application) | Responsive React storefront: cart, search, categories, PDP |
| [**siddaroodh-portfolio**](https://github.com/siddaroodh05/siddaroodh-portfolio) | Personal portfolio site |

---

## 📊 GitHub Activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=siddaroodh05&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="165" alt="GitHub stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=siddaroodh05&layout=compact&theme=tokyonight&hide_border=true" height="165" alt="Top languages" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=siddaroodh05&theme=tokyonight&hide_border=true" alt="Streak" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=siddaroodh05&theme=tokyo-night&hide_border=true" alt="Activity graph" width="95%" />
</p>

<p align="center">
  <img src="https://leetcard.jacoblin.cool/siddaroodh__2004?theme=dark&font=JetBrains%20Mono&ext=heatmap" alt="LeetCode stats" />
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=siddaroodh05&theme=tokyonight&no-frame=true&row=1&column=7" alt="Trophies" />
</p>

<!-- Contribution snake: needs the workflow in .github/workflows/snake.yml -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/siddaroodh05/siddaroodh05/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/siddaroodh05/siddaroodh05/output/github-contribution-grid-snake.svg" />
    <img alt="Contribution snake" src="https://raw.githubusercontent.com/siddaroodh05/siddaroodh05/output/github-contribution-grid-snake-dark.svg" />
  </picture>
</p>

---

## 🤝 Let's Connect

<p align="center"><i>Open to Backend Engineer / SDE Intern opportunities. Feel free to reach out.</i></p>

<p align="center">
  <a href="mailto:siddaroodh2004@gmail.com"><img src="https://img.shields.io/badge/Say%20Hello-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/siddaroodh-venkatapur-821551262/"><img src="https://img.shields.io/badge/Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,100:0f2027&height=130&section=footer" width="100%" alt="footer" />
