## Hi, I'm Abhijeet 👋

**AI Engineer, Research & Development at ONE PWS.** I build LLM agents and the production systems around them, including tool-calling agents, RAG pipelines, evaluations and human-approval steps.

I'm the only engineer behind a suite of internal applications running in production at a manufacturing company, plus an AI agent that employees use every day across all of them. I spend most of my time on the less glamorous half of AI engineering: evals, tracing, schema-validated outputs, and fallback paths so the model never makes things up in front of a user.

📍 Udaipur, India · 🎓 B.Tech, Computer Science Engineering (2026) · 📫 abhijeetsharmawork1@gmail.com · 🔗 [LinkedIn](https://www.linkedin.com/in/abhiibhiii/)

---

### What I've built

| Project | What it is | Stack |
|---|---|---|
| **[OCT: AI agent over internal systems](https://github.com/Abhiibhiii/oct-architechture)** | An agent employees use daily. Each internal system's REST API is a tool, answers are grounded in real data, every output is schema-validated with a fallback, and prompt changes are tested against a golden set before release. Repo has an architecture case study and a reference implementation. | LangChain · LangGraph · Claude via Bedrock · LangFuse |
| **Certificate renewal agent** | A scheduled agent that tracks licence expiries and acts on them by itself. It escalates when the owner doesn't respond and files renewals only after a person approves. | Python · PostgreSQL · cron · Google Cloud |
| **[Agentic job hunt](https://github.com/Abhiibhiii/agentic-job-hunt)** | A multi-skill agent system that runs a job search: scheduled discovery, scoring, resume tailoring and outreach drafts. Guardrails stop it fabricating data, and anything irreversible waits for a person. | Claude Code skills · subagents |
| **Scout: outreach agent** *(private)* | Finds prospects and checks them against real evidence, ranks them, and writes personalised messages that must pass a quality check. A person approves before anything is sent. | Node.js · Gemini (Vertex AI) · MongoDB · Cloud Run · Chrome extension |
| **Agentic-coding benchmark tasks** *(contract)* | Terminal-Bench 2 tasks for evaluating frontier coding agents. Each has a pinned Docker environment and a pytest checker, so a correct solution passes and a do-nothing attempt fails. | Docker · pytest · Harbor |
| **Real-time messaging platform** *(private, in production)* | Runs around the clock for an organisation: WebSockets, WebRTC calls, and a view-only document pipeline with short-lived signed URLs. | Fastify · Socket.IO · Prisma · Postgres · Cloud Run |

### Tools I work with

**AI / agents:** LangChain · LangGraph · RAG · MCP (FastMCP) · Amazon Bedrock · Vertex AI / Gemini · Google ADK · LangFuse · prompt and eval design
**Backend:** Python · FastAPI · Node.js · Fastify · Express · REST · Socket.IO · WebRTC
**Data:** PostgreSQL · Prisma · SQLAlchemy · MongoDB · Firebase
**Frontend and cloud:** TypeScript · React · Next.js · Tailwind · Google Cloud (Cloud Run, GCS) · Vercel · Docker · CI/CD

### How I build

- Agents go through the same authenticated APIs as users, never straight into the database.
- Every agent run is traced, and every prompt change has to pass evals before it ships.
- Anything irreversible needs a person to approve it, with clear escalation when no one responds.
- Security is built in from the start: row-level security, short-lived signed URLs, and secrets kept out of code.

---

Most of my production work belongs to my employer and is private. I'm happy to walk through the architecture and code on a call.
