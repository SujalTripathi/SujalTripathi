<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1f2937,50:2563eb,100:0ea5e9&height=200&section=header&text=Sujal%20Tripathi&fontSize=56&fontColor=ffffff&fontAlignY=40&desc=Full%20Stack%20Developer%20%C2%B7%20GSoC%202026%20Contributor%20%40%20LibreHealth&descSize=16&descAlignY=62&animation=fadeIn" />

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&duration=3200&pause=1000&color=2563EB&center=true&vCenter=true&width=700&lines=Full+Stack+MERN+Developer;GSoC+2026+Contributor+%40+LibreHealth;Built+a+FHIR-based+Drag-and-Drop+Form+Designer;Open+Source+Advocate+%C2%B7+100%2B+PRs+Merged" alt="Typing SVG" />
</a>

<br>

<img src="https://img.shields.io/badge/GSoC%202026-Completed-2ea44f?style=for-the-badge&logo=google&logoColor=white" alt="GSoC Status"/>
<img src="https://img.shields.io/badge/Status-Open%20to%20Opportunities-2563eb?style=for-the-badge" alt="Status"/>

<br><br>

<img src="https://img.shields.io/github/followers/SujalTripathi?label=Followers&style=flat-square&color=1f2937" alt="followers"/>
<img src="https://komarev.com/ghpvc/?username=SujalTripathi&label=Profile%20Views&color=2563eb&style=flat-square" alt="Profile views"/>
<img src="https://img.shields.io/badge/PRs%20Merged-100%2B-2563eb?style=flat-square" alt="PRs Merged"/>
<img src="https://img.shields.io/badge/Issues%20Resolved-50%2B-2563eb?style=flat-square" alt="Issues Resolved"/>

<br><br>

<a href="https://www.linkedin.com/in/sujaltripathi" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="https://github.com/SujalTripathi" target="_blank"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"/></a>
<a href="mailto:sujaltripathi816@gmail.com" target="_blank"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Gmail"/></a>
<a href="https://sujalprotfolio.netlify.app/" target="_blank"><img src="https://img.shields.io/badge/Portfolio-2563EB?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio"/></a>
<a href="https://twitter.com/SujalTripathi" target="_blank"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=flat-square&logo=twitter&logoColor=white" alt="Twitter"/></a>
<a href="https://www.instagram.com/official_sujaltripathi" target="_blank"><img src="https://img.shields.io/badge/Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white" alt="Instagram"/></a>
<a href="https://www.youtube.com/@sujaldancechannel" target="_blank"><img src="https://img.shields.io/badge/YouTube-FF0000?style=flat-square&logo=youtube&logoColor=white" alt="YouTube"/></a>

</div>

<br>

## Table of Contents

- [Summary](#summary)
- [GSoC 2026 — LibreHealth](#gsoc-2026--librehealth)
- [Experience Highlights](#experience-highlights)
- [Technical Skills](#technical-skills)
- [Featured Projects](#featured-projects)
- [Open Source Contribution Timeline](#open-source-contribution-timeline)
- [GitHub Activity](#github-activity)
- [Writing & Content](#writing--content)
- [Mentorship & Community](#mentorship--community)
- [Currently Learning](#currently-learning)
- [Contact](#contact)

<br>

## Summary

Third-year Computer Engineering student and full-stack developer specializing in the **MERN stack**, based in Surat, Gujarat. Completed **Google Summer of Code 2026 with LibreHealth**, where I built a web-component-based drag-and-drop form designer for FHIR-compliant healthcare forms. Active contributor across multiple open-source communities with 100+ merged pull requests and a track record of shipping features end to end — from architecture decisions through implementation, testing, and mentor review.

Alongside development work, I run a small freelance practice building websites, branding, and marketing assets for local businesses, and I document my open-source and GSoC work through weekly progress reports and technical write-ups.

| | |
|---|---|
| **Location** | Surat, Gujarat, India (IST, UTC+5:30) |
| **Education** | 3rd-year, Computer Engineering, CKPCET, Surat |
| **Focus** | Full-Stack Development (MERN), Healthcare Interoperability (FHIR), Open-Source |
| **Program** | GSoC 2026 — LibreHealth (Completed) |
| **Availability** | Open to internships, freelance projects, and full-stack roles |
| **Working Style** | Async-friendly, documents progress weekly, comfortable with distributed teams |

<br>

## GSoC 2026 — LibreHealth

Selected as a **Google Summer of Code 2026 contributor** for LibreHealth to build a **Web Component-based Drag-and-Drop Form Designer** — a zero-framework, vanilla Web Components tool that lets non-developers assemble FHIR-compliant healthcare forms visually, without writing code.

**What I shipped:**

- **Drag-and-drop canvas & field palette** — built `<form-designer-canvas>`, `<form-field-wrapper>`, and a component palette using the native HTML5 Drag and Drop API, with click-to-select, hover states, and field removal.
- **Live FHIR data binding** — connected form fields to FHIR R4 resources so values populate and sync in real time against a Patient resource.
- **Properties panel & JSON schema sync** — a dedicated panel for editing field label, type, required state, and FHIR path bindings, kept in sync with an internal JSON schema after every canvas action.
- **Drag-and-drop reordering** — added SortableJS-based reordering of fields within groups as a progressive enhancement alongside existing up/down controls, with a DOM-desync fix to keep it compatible with Lit's re-render cycle.
- **Canvas/properties-panel architecture split** — refactored an 892-line monolithic component into three cleanly separated custom elements (canvas, properties panel, orchestrator) communicating via custom events, based on mid-term mentor feedback.
- **Export / Import** — serializes the canvas's form schema to a downloadable, spec-compliant JSON file and rebuilds the canvas from an imported file.
- **Preview Mode with live conditional logic** — a toggle that renders the design canvas as an actual interactive form, evaluating FHIR `enableWhen` conditions (`=`, `!=`, `exists`, `>`, `<`, across string/boolean/integer/decimal/date/coding answer types) live as the user fills it in, so conditional fields show and hide in real time.
- **Unit test coverage** — tests for canvas drop behavior, schema sync, properties panel updates, preview-mode rendering, and conditional field visibility, using `@web/test-runner`.

**Stack:** Lit / vanilla Web Components, native HTML5 Drag & Drop API, FHIR R4, GitLab CI.

<br>

## Experience Highlights

### Open-Source Contributions
Active contributor to several community-driven projects outside of GSoC:

- **Talawa Admin** (Palisadoes Foundation) — contributed JavaScript and web-component changes to the community management platform's admin dashboard, including UI fixes and test coverage improvements.
- **CircuitVerse** — contributed to the digital logic circuit simulator used by students and educators, working in Ruby on Rails and JavaScript.
- **6+ other repositories** — smaller fixes, documentation improvements, and issue triage across various open-source projects.

Across all of these, I've merged 100+ pull requests and resolved 50+ issues, and I write clear PR descriptions and technical documentation as a standard part of the workflow rather than an afterthought.

### Program Recognition

- **GSoC 2026** — Successfully completed as a contributor with LibreHealth; received program completion certificate and mentor verification letter.
- **Hacktoberfest 2025** — Recognized as a Super Contributor for quality contributions across multiple repositories during the event.
- **Social Winter of Code 2026 (SWOC)** — Ranked 3rd among participating contributors based on merged contributions and code quality.

### Freelance & Client Work
Built and shipped web applications and features for small businesses, including:

- A **transportation and lead-generation website**, adding booking and inquiry-capture features that directly supported the client's sales pipeline.
- Branding and promotional materials (logos, social media assets, short promotional videos) for multiple small-business clients, handling both the technical build and the visual design.

This client-facing work has meant handling the full lifecycle myself — requirements discovery, pricing conversations, build, deployment, and post-launch support — rather than just the coding portion.

<br>

## Technical Skills

| Category | Skills | Proficiency |
|---|---|---|
| **Frontend** | React, Next.js, Lit / Web Components, Redux, Tailwind CSS, Material UI, Framer Motion | Strong |
| **Backend** | Node.js, Express.js, REST APIs, GraphQL, JWT Auth | Strong |
| **Healthcare Interop** | FHIR R4 (Questionnaire, Patient, data binding, conditional logic) | Applied in production GSoC work |
| **Languages** | JavaScript, TypeScript, Python, Java, Go, C++ | Working knowledge across all; JS/TS strongest |
| **Databases** | MongoDB, PostgreSQL, MySQL, Redis, Firebase, Prisma | Comfortable |
| **DevOps / Cloud** | Docker, GitHub Actions, GitLab CI, Linux, AWS, Azure | Growing — Kubernetes in active study |
| **Testing** | @web/test-runner, Jest, React Testing Library, ESLint | Comfortable |
| **Tools** | Git, GitLab, GitHub, VS Code, Postman, Figma, Vercel, Netlify | Daily use |

<div align="center">

![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=ffdd54)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![React](https://img.shields.io/badge/React-20232a?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-black?style=flat-square&logo=next.js&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-6DA55F?style=flat-square&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-404d59?style=flat-square&logo=express&logoColor=61DAFB)
![MongoDB](https://img.shields.io/badge/MongoDB-4ea94b?style=flat-square&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0db7ed?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05033?style=flat-square&logo=git&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)

</div>

<br>

## Featured Projects

### LibreHealth Form Designer — GSoC 2026
Web-component-based drag-and-drop interface builder for assembling FHIR-compliant healthcare forms without writing code.
- **Stack:** Lit / Web Components, HTML5 Drag & Drop API, FHIR R4
- **Role:** GSoC 2026 Contributor
- **Highlights:** Live FHIR data binding, drag-to-reorder, export/import, live conditional logic (`enableWhen`) in Preview Mode
- **Link:** [gitlab.com/librehealth/toolkit/lh-toolkit-webcomponents](https://gitlab.com/librehealth/toolkit/lh-toolkit-webcomponents)
- **Status:** Completed — GSoC 2026

### Talawa Admin
Admin dashboard for a community management platform used by nonprofits and community organizations.
- **Stack:** React, TypeScript, GraphQL
- **Role:** Contributor — UI components, bug fixes, test coverage
- **Link:** [github.com/PalisadoesFoundation/talawa-admin](https://github.com/PalisadoesFoundation/talawa-admin)
- **Status:** Actively contributing

### CircuitVerse
Browser-based digital logic circuit simulator used in engineering education.
- **Stack:** Ruby on Rails, JavaScript
- **Role:** Contributor
- **Link:** [github.com/CircuitVerse/CircuitVerse](https://github.com/CircuitVerse/CircuitVerse)
- **Status:** Active

### Personal Portfolio
Personal site presenting projects, skills, and case studies of client work.
- **Stack:** Next.js, Tailwind CSS, Framer Motion
- **Role:** Sole developer and designer
- **Link:** [sujalprotfolio.netlify.app](https://sujalprotfolio.netlify.app/)
- **Status:** Live

### Transportation Lead-Generation Site
Client website with booking and inquiry-capture features to support sales.
- **Stack:** MERN stack
- **Role:** Feature developer
- **Status:** Delivered

<br>

## Open Source Contribution Timeline

| Period | Milestone |
|---|---|
| 2026 | **Completed GSoC 2026** — LibreHealth Form Designer, certificate + mentor verification received |
| 2026 | Ranked 3rd, Social Winter of Code (SWOC) |
| 2025 | Hacktoberfest Super Contributor |
| 2025 | Crossed 100+ merged pull requests across projects |
| 2024–2025 | Began contributing to Talawa Admin and CircuitVerse |
| 2024 | Started building client websites and freelance projects |

<br>

## GitHub Activity

<div align="center">

<img height="160em" src="https://github-readme-stats.vercel.app/api?username=SujalTripathi&show_icons=true&theme=default&hide_border=true&title_color=2563eb&icon_color=2563eb&text_color=333333" alt="GitHub Stats" />
<img height="160em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=SujalTripathi&layout=compact&theme=default&hide_border=true&title_color=2563eb&text_color=333333" alt="Top Languages" />

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=SujalTripathi&theme=minimal&hide_border=true&color=2563eb&line=1f2937&point=2563eb&area=true" alt="Contribution Graph" />

<img width="100%" src="https://github-profile-trophy.vercel.app/?username=SujalTripathi&theme=flat&no-frame=true&margin-w=8&row=1&column=6&title_color=2563eb&icon_color=2563eb" alt="GitHub Trophies"/>

</div>

## 🏆 Achievements & Recognition

<div align="center">

### 🎖️ Distinguished Achievements

<table align="center">
  <tr>
    <td align="center"><img src="https://img.shields.io/badge/GSoC%202026-LibreHealth-FF6B6B?style=for-the-badge&logo=google&logoColor=white" alt="GSoC 2026"/></td>
    <td align="center"><img src="https://img.shields.io/badge/Hacktoberfest%202025-Super%20Contributor-FFD700?style=for-the-badge&logo=hacktoberfest&logoColor=black" alt="Hacktoberfest"/></td>
    <td align="center"><img src="https://img.shields.io/badge/SWOC%202026-Rank%203-4ecdc4?style=for-the-badge&logo=github&logoColor=white" alt="SWOC"/></td>
    <td align="center"><img src="https://img.shields.io/badge/Open%20Source-150%2B%20Contributions-success?style=for-the-badge&logo=github&logoColor=white" alt="Contributions"/></td>
  </tr>
</table>

### 🎯 Recognition Badges

<p align="center">
  <img src="https://img.shields.io/badge/100%2B%20Pull%20Requests-Merged-success?style=flat-square&logo=github&logoColor=white&color=FF6B6B" alt="PRs"/>
  <img src="https://img.shields.io/badge/50%2B%20Issues-Resolved-blue?style=flat-square&logo=github&logoColor=white&color=4ecdc4" alt="Issues"/>
  <img src="https://img.shields.io/badge/10%2B%20Active-Projects-orange?style=flat-square&logo=git&logoColor=white" alt="Projects"/>
  <img src="https://img.shields.io/badge/Full-Stack%20Developer-purple?style=flat-square&logo=code&logoColor=white" alt="Full Stack"/>
</p>

### 🎖️ Holopin Badges
<a href="https://holopin.io/@sujaltripathi">
  <img src="https://holopin.me/sujaltripathi" alt="Holopin Board" width="100%"/>
</a>

</div>


<br>

## Writing & Content

I write about what I'm building and learning, both as documentation for myself and to help others navigating similar paths:

- **Weekly progress reports** — summarizing GSoC work, blockers, and what's shipped, shared with mentors and the community.
- **Technical tutorials** — blog posts covering web development concepts, FHIR/healthcare interoperability, open-source contribution workflows, and lessons from client projects.
- **Video content** — short tutorials and behind-the-scenes looks at development work, published on YouTube alongside dance and creative content.

<br>

## Mentorship & Community

- Regularly communicate with mentors and maintainers across open-source projects, treating code review feedback as a core part of the learning process rather than a formality.
- Help newcomers get started with their first pull requests in the communities I contribute to, based on my own experience going through that process.
- Participate in community programs (GSoC, Hacktoberfest, SWOC) partly to build the habit of working in distributed, async-first teams.

<br>

## Currently Learning

| Area | Why |
|---|---|
| System Design & Architecture | Needed to design services that scale past a single-developer project |
| Advanced DSA & Competitive Programming | Sharpening problem-solving for technical interviews |
| Kubernetes & Container Orchestration | Extending DevOps skills beyond Docker into orchestration |
| Microservices Design Patterns | Preparing to architect larger, decoupled systems |
| Cloud Infrastructure (AWS/Azure) | Deepening deployment and infra skills beyond basic hosting |

<br>

## Contact

- **Email:** [sujaltripathi816@gmail.com](mailto:sujaltripathi816@gmail.com)
- **LinkedIn:** [linkedin.com/in/sujaltripathi](https://www.linkedin.com/in/sujaltripathi)
- **Portfolio:** [sujalprotfolio.netlify.app](https://sujalprotfolio.netlify.app/)
- **Location:** Surat, Gujarat, India (IST, UTC+5:30)

I'm open to technical discussions, open-source collaboration, freelance web development work, and full-stack opportunities — feel free to reach out.

<div align="center">
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1f2937,50:2563eb,100:0ea5e9&height=100&section=footer" />
</div>
