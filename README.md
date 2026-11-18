<p align="center">
  <img src="./assets/profile-banner.svg" width="100%" alt="Varun Saxena — full-stack product engineer focused on end-to-end system design, AI products, and technical leadership" />
</p>

<p align="center">
  <a href="https://my-portfolio-one-puce-63.vercel.app/">
    <img src="https://img.shields.io/badge/Hi%2C%20I'm-Varun%20Saxena-111827?style=for-the-badge&labelColor=111827" alt="Hi, I'm Varun Saxena" />
  </a>
  <a href="https://chalk-ai-tan.vercel.app/">
    <img src="https://img.shields.io/badge/AI-Groq%20%2B%20GPT--OSS-F55036?style=for-the-badge&logo=groq&logoColor=white" alt="Groq and GPT-OSS" />
  </a>
  <a href="https://github.com/2yb/chalk-ai">
    <img src="https://img.shields.io/badge/Focus-Generative%20AI-6E56CF?style=for-the-badge&logo=openai&logoColor=white" alt="Generative AI" />
  </a>
</p>

---

### 🛠️ Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=react,nextjs,ts,js,html,css,tailwind,mui,express,jest,vercel,git,github,figma" alt="React, Next.js, TypeScript, JavaScript, HTML, CSS, Tailwind, Material UI, Express, Jest, Vercel, Git, GitHub, and Figma" />
</p>

### 🤖 AI in Practice

<p>
  <img src="https://img.shields.io/badge/Groq-LLM%20inference-F55036?style=flat-square&logo=groq&logoColor=white" alt="Groq" />
  <img src="https://img.shields.io/badge/OpenAI-GPT--OSS%20model-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI GPT-OSS model" />
  <img src="https://img.shields.io/badge/Zod-Structured%20validation-3E67B1?style=flat-square&logo=zod&logoColor=white" alt="Zod structured validation" />
</p>

---

### 🚀 Featured Projects

#### [ChalkAI](https://chalk-ai-tan.vercel.app/) · [Source](https://github.com/2yb/chalk-ai)

AI-powered visual lessons with narrated playback and an interactive whiteboard.

`Next.js` `React` `TypeScript` `Groq` `Zod`

#### [TrialFlow](https://trialflow-tau.vercel.app/overview) · [Source](https://github.com/2yb/trialflow)

A clinical-trial site-readiness prototype for study monitoring, document review, and operational work queues.

`Next.js` `React` `TypeScript` `Tailwind CSS` `Vitest`

#### [Paste App](https://lobster-git-main-2ybs-projects.vercel.app/)

A fast pastebin clone with real-time UI sharing.

#### [Hi There](https://hi-there-hyjkk6uh7-2ybs-projects.vercel.app/)

A personal portfolio with smooth animations, light/dark themes, and SEO optimization.

---

### 🧭 Architecture at a Glance

#### ChalkAI · AI lesson pipeline

```mermaid
%%{init: {"theme": "base", "themeVariables": {"darkMode": true, "background": "#080b18", "primaryColor": "#172554", "primaryTextColor": "#e2e8f0", "primaryBorderColor": "#22d3ee", "lineColor": "#a78bfa", "secondaryColor": "#271447", "tertiaryColor": "#111827", "fontFamily": "Inter, Segoe UI, sans-serif"}}}%%
flowchart LR
    learner([Learner]) --> studio["Tutor Studio<br/>Next.js + React"]
    studio -->|Topic and level| api["Generate lesson API"]
    api --> service["Lesson service"]
    service --> cache{"Lesson cache"}
    cache -->|Miss| groq["Groq API<br/>GPT-OSS model"]
    groq --> validate["Zod validation"]
    validate --> visuals["Build whiteboard actions"]
    cache -->|Hit| lesson["Lesson"]
    visuals --> lesson
    lesson --> timeline["Playback timeline"]
    timeline --> speech["Browser speech"]
    timeline --> board["Animated whiteboard"]
    studio -->|Follow-up question| followup["Follow-up API"]
    followup --> groq

    classDef client fill:#101a2d,stroke:#22d3ee,color:#e2e8f0
    classDef ai fill:#3b1d12,stroke:#fb923c,color:#fff7ed
    classDef logic fill:#21133a,stroke:#c084fc,color:#f5f3ff
    class learner,studio,board,speech client
    class groq ai
    class service,cache,validate,visuals,timeline,followup logic
```

#### TrialFlow · shared workflow state

```mermaid
%%{init: {"theme": "base", "themeVariables": {"darkMode": true, "background": "#080b18", "primaryColor": "#172554", "primaryTextColor": "#e2e8f0", "primaryBorderColor": "#22d3ee", "lineColor": "#a78bfa", "secondaryColor": "#123329", "tertiaryColor": "#111827", "fontFamily": "Inter, Segoe UI, sans-serif"}}}%%
flowchart LR
    operator([Operations team]) --> app["Next.js application"]
    app --> pages["Overview · Studies · Sites<br/>Documents · Work queue"]
    pages <--> store["Shared client-side store"]
    seed["Fictional seed data"] --> store
    store --> actions["Review documents<br/>Update tasks"]
    actions --> store
    store --> derived["Readiness and dashboard metrics"]
    derived --> pages

    classDef user fill:#101a2d,stroke:#22d3ee,color:#e2e8f0
    classDef workflow fill:#122b27,stroke:#34d399,color:#ecfdf5
    classDef data fill:#2b2040,stroke:#c084fc,color:#f5f3ff
    class operator,app,pages user
    class store,actions,derived workflow
    class seed data
```

---

### 📫 Let's Connect

<p align="center">
  <a href="https://www.linkedin.com/in/varunsaxena1912/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin" alt="Connect on LinkedIn" />
  </a>
  <a href="https://my-portfolio-one-puce-63.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-Visit-2b72e0?style=for-the-badge&logo=vercel" alt="Visit portfolio" />
  </a>
  <a href="mailto:varunsaxena1912@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-Mail-red?style=for-the-badge&logo=gmail" alt="Email Varun" />
  </a>
</p>
