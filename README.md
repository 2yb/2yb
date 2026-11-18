<h1 align="center">Hi 👋, I'm Varun</h1>
<h3 align="center">Frontend developer building polished web apps and AI-assisted products</h3>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=22&pause=1000&center=true&vCenter=true&width=560&lines=React+%26+Next.js+experiences;AI-powered+learning+tools;Thoughtful+workflow+products" alt="Building React and Next.js experiences, AI-powered learning tools, and thoughtful workflow products" />
</p>

<p align="center">
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
```

#### TrialFlow · shared workflow state

```mermaid
flowchart LR
    operator([Operations team]) --> app["Next.js application"]
    app --> pages["Overview · Studies · Sites<br/>Documents · Work queue"]
    pages <--> store["Shared client-side store"]
    seed["Fictional seed data"] --> store
    store --> actions["Review documents<br/>Update tasks"]
    actions --> store
    store --> derived["Readiness and dashboard metrics"]
    derived --> pages
```

---

### 📊 GitHub Activity

<p align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=2yb&show_icons=true&hide_border=true&theme=transparent" alt="GitHub activity statistics" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=2yb&layout=compact&hide_border=true&theme=transparent" alt="Most used programming languages" />
</p>

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
