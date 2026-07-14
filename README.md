<h1 align="center">Hi 👋, I'm Rohit Rai</h1>
<h3 align="center">Generative AI Engineer | Agentic Systems & RAG | Full-Stack Foundation (React · React Native · Node · Python)</h3>

<p align="center">
  I build LLM systems that hold up in production — agents, RAG pipelines, and the evaluation layers that make them trustworthy.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/rohit-rai-700980258/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:rohitrai275101@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://twitter.com/now_rohit"><img src="https://img.shields.io/badge/Twitter-Follow-1DA1F2?style=for-the-badge&logo=x&logoColor=white" alt="Twitter"/></a>
</p>

---

## 🚀 Featured Projects

### 📊 AI Investor Intelligence Platform
**Python · FastAPI · RAG · ChromaDB · PostgreSQL · Docker** — *Live on Hugging Face Spaces*

An end-to-end RAG system that ingests company annual-report PDFs and turns them into trustworthy, structured intelligence.

- **Pipeline:** OCR → semantic chunking → local `sentence-transformers` embeddings → ChromaDB → LLM extraction of **8 financial KPIs** with JSON-schema (Pydantic) validation
- **Grounded chat:** answers only from ingested documents, with explicit refusal behavior when the answer isn't in the source
- **Production observability:** every request traced with a `request_id`; per-stage latency, token, and cost metrics persisted to Postgres
- **Evaluation as a first-class citizen:** automated eval harness — deterministic checks + **LLM-as-judge groundedness scoring** — that **gates CI**: below 80% pass rate, or any hallucination regression failure, deployment is blocked
- Born from a real incident: the model once fabricated a citation to a document that was never ingested. That exact failure is now a permanent adversarial regression test.

🔗 **Live demo:** *coming soon* &nbsp;|&nbsp; 📁 **Repo:** *link coming soon*

---

### 🤖 LeadRadar — Agentic Business-Audit System
**Python · Playwright · Multi-Provider LLM Router · Vision LLM** — *32 passing tests*

An autonomous multi-step agent pipeline: discovers local businesses via the Google Places API, audits their websites with Playwright + a vision-capable LLM, and scores each as a lead — fully dynamic CLI.

- **Fault-tolerant multi-provider LLM router** across Groq / Gemini / OpenRouter: per-key cooldowns, in-provider key rotation, automatic cross-provider failover — the pipeline **survived real quota exhaustion mid-run** without the caller ever seeing a failure
- **Normalized failure handling:** providers returning HTTP 200 with malformed payloads trigger failover exactly like 429s — because in multi-provider systems, you validate the payload, not the status code
- **Deliberate agent boundaries:** LLM judgment only where judgment is needed (visual verdicts); scoring is deterministic, explainable math; humans stay in the loop for irreversible actions
- Built via a formal SRS with **checkpoint-based milestones** and a `CLAUDE.md` project-memory workflow — every checkpoint shipped runnable, tested code before the next began

📁 **Repo:** *link coming soon*

---

## 🧠 What I Work With

**GenAI / Agentic:** LLM applications · RAG pipelines · agentic tool-calling loops · multi-provider LLM routing · embeddings & vector databases (ChromaDB) · LLM evals (LLM-as-judge, groundedness, CI gating) · prompt engineering · Anthropic API · Claude Code *(Anthropic Skilljar Certified, 2026)*

**Backend:** Python (FastAPI, Pydantic, Playwright, pytest) · Node.js · REST APIs · PostgreSQL · MongoDB · Firebase · Docker · AWS (EC2)

**Frontend & Mobile:** React.js · React Native (CLI & Expo) · TypeScript · Next.js · Redux Toolkit · EAS Build & OTA Updates

**Delivery:** GitHub Actions CI/CD · agentic coding workflows · SRS-driven, checkpoint-based builds

---

## 🔭 Currently

- Building and shipping agentic AI systems — currently adding **LangGraph orchestration**, **re-ranking / hybrid search**, and **Langfuse tracing** to my stack
- Exploring where LLMs meet real business workflows: document intelligence, autonomous audit pipelines, and evaluation-driven development
- Open to **Generative AI / Applied AI / Forward Deployed** engineering roles

> My working belief: **evaluation is what separates AI demos from AI products.** If you can't measure groundedness, you're shipping vibes.

---

## 📈 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=rohit-rai-0101rm&show_icons=true&theme=default&hide_border=true" alt="GitHub stats" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=rohit-rai-0101rm&layout=compact&hide_border=true" alt="Top languages" height="165"/>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=rohit-rai-0101rm&hide_border=true" alt="Streak stats"/>
</p>

---

<p align="center">
  ⚡ <i>Fun fact: I once debugged for hours… only to find the bug was in a comment.</i>
</p>

<p align="center">
  📫 Reach me: <b>rohitrai275101@gmail.com</b>
</p>
