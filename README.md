# n8n Academy — Projects & Practical Assessments

[![Platform](https://img.shields.io/badge/platform-n8n%20Academy-EA4B71)](https://learn.n8n.io/)
[![Courses](https://img.shields.io/badge/courses-5-blue)]()
[![Cost](https://img.shields.io/badge/cost-free-brightgreen)]()
[![Status](https://img.shields.io/badge/in%20progress-QS101-orange)]()

This repository collects my work as I move through the **[n8n Academy](https://learn.n8n.io/)** — n8n's official, hands-on learning platform. It is a working log of every **workflow I build** and every **practical assessment** required to earn each course badge and certificate of completion.

n8n is an open-source workflow automation platform: it connects apps, moves data between services, and orchestrates logic and AI without writing code for every step. The Academy teaches it by *building*, not just reading — each course ends with hands-on exercises, quizzes, and a final exam.

> **Note:** The n8n Academy replaced the older text-based Level 1 / Level 2 courses that lived on `docs.n8n.io`. Those legacy courses were retired on June 30, 2026.

<br>

---

## Repository purpose

- **Projects** — the real workflows I create throughout each course, exported as `.json` files (*n8n workflows are portable JSON, not binaries*).
- **Assessments** — the practical, hands-on exercises the platform grades to award the completion certificate.
- **Notes** — short write-ups of key concepts and gotchas per course.

Workflows can be re-imported into any n8n instance via **Import from File** or **Import from URL**.

<br>

---

## Course snapshot (as of November 24, 2026)

The Academy currently offers **5 courses**: one standalone fast track (**QS101**), the three-course **n8n Foundations** program (**N8N101 → N8N102 → N8N103**), and a newer standalone agents course (**AI201**).

| Code | Course | Track | Published | Est. time | Status |
|------|--------|-------|--------|-----------|--------|
| **QS101** | n8n Quickstart | Fast Track (standalone) | Jun 16, 2026 | 3–5 h | 🟠 In progress |
| **N8N101** | Essentials: Your First Workflows | Foundations (1 of 3) | Jun 16, 2026 | 2–4 h | ⬜ Planned |
| **N8N102** | Integrations: APIs & Connected Workflows | Foundations (2 of 3) | Jun 16, 2026 | 4–6 h | ⬜ Planned |
| **N8N103** | In Practice: AI, Testing & Best Practices | Foundations (3 of 3) | Jun 16, 2026 | 3–4 h | ⬜ Planned |
| **AI201** | Introduction to Agents | Standalone | Oct 1, 2026 | TBC | ⬜ Planned |

> **Two ways in, same reward:** The **Fast Track** (QS101 alone) and the **Deep Dive** (the full Foundations program) are both free, both graded the same way, and both award a badge and certificate. Completing the entire Foundations program also earns a **program-level certificate and badge**.

<br>

---

## The courses in detail

### 🚀 QS101 — n8n Quickstart
*The fastest way in.* Builds a working workflow in one short sitting, from first trigger to a functioning AI agent. Based on n8n's original text courses, refreshed with a new AI section.

- **You build:** your first workflows → a data pipeline with error handling → a customer-service AI agent.
- **Covers:** triggers, scheduling, HTTP requests, expressions, API credentials, data transformation, error handling, and connecting AI to real data.
- 📄 Detailed syllabus: [`QS101-n8n-quickstart`](.//QS101-n8n-Quickstart)

<br>

### 📘 N8N101 — Essentials: Your First Workflows
The starting point of the Foundations program. No prior experience required.

- **Section 1 — Getting started with n8n:** platform orientation, triggers, and credentials.
- **Section 2 — Data flow & Transformation:** n8n data structures, transformations, expressions, and binary data.
- **Outcomes:** navigate the canvas; understand nodes, connections, and executions; build and run a first workflow; use triggers and scheduling; map, transform, and merge data between nodes.

<br>

### 🔌 N8N102 — Integrations: APIs & Connected Workflows
The technical core — described by n8n as *the most technically dense course in the Foundations program.*

- **Section 1 — Workflow execution and logic:** execution order (sequential and parallel paths), sub-workflows, logic control with `IF` / `Switch` / `Loop Over Items` / `Wait`, and error handling with the `Error Trigger` and `Stop and Error` nodes.
- **Section 2 — APIs, authentication, and integration patterns:** `HTTP Request` calls (GET, POST, PUT, PATCH, DELETE), authentication with API keys, OAuth2, and Bearer tokens, pagination, the `Webhook` trigger, credential management, Data Tables, data reshaping (`Merge`, `Split Out`, `Aggregate`, `Filter`, `Summarize`), custom code (JavaScript or Python), and a capstone integration.

<br>

### 🤖 N8N103 — In Practice: AI, Testing & Best Practices
The production-ready course — moving from workflows that only work in development to automations that hold up in production.

- **Section 1 — AI Introduction:** AI in n8n, AI nodes, the `AI Agent` node, chains vs. agents, and AI best practices.
- **Section 2 — Testing & Debugging:** development best practices, the execution log and debugger, and error handling (e.g. Try/Catch).
- **Section 3 — Workflow Organization & Best Practices:** naming conventions, canvas organization, folders and tags, sub-workflows, documentation, and production readiness (publishing, scheduling, monitoring, recovery, templates, and version control).

### 🧠 AI201 — Introduction to Agents
A newer standalone course focused on building AI agents in n8n (started October 1, 2026).

> ⚠️ **Preliminary:** The official detailed syllabus for AI201 is not yet published. Expected to cover the fundamentals of AI agents in n8n — the LLM "brain," memory, tool integrations, and safe automation patterns. This section will be updated once I enroll and the full outline is available.

<br>

---

## How grading & certification work

The four structured courses (QS101, N8N101, N8N102, N8N103) share the same grading model:

| Component | Weight |
|-----------|-------:|
| Section quizzes | 10% |
| Hands-on workflow exercises | 55% |
| Final exam | 35% |
| **Passing grade** | **70%** |

> **Tip from the platform:** complete the hands-on workflow exercises *before* the quizzes — some quiz questions require a working workflow or agent to answer.

On passing, you receive a **verifiable badge** (issued via the badges platform) and a **certificate of completion**. n8n is explicit that this is **not a formal certification**.

<br>

---

## What you need

- A publicly accessible **n8n instance** — n8n Cloud (*free trial*) or self-hosted (*free*).
- Most exercises use **practice APIs hosted by n8n Academy**, so no external accounts are required.
- For the AI sections (QS101, N8N103, AI201): an **API key** from a chat-model provider such as OpenAI, Anthropic, Google Gemini, DeepSeek, or Groq — providers with free tiers work fine.

<br>

---

## Repository structure

```
.
├── README.md                        # This file — Academy & course overview
├── QS101-n8n-quickstart/
│   ├── README.md                    # Detailed QS101 syllabus & progress
│   ├── projects/                    # Workflows built during the course (.json)
│   ├── assessments/                 # Graded hands-on exercises (.json)
│   └── notes/                       # Concept notes & takeaways
├── N8N101-essentials/               # (added when the course begins)
├── N8N102-integrations/
├── N8N103-in-practice/
└── AI201-intro-to-agents/
```

<br>

---

## References

- n8n Academy — <https://learn.n8n.io/>
- n8n Education overview — <https://n8n.io/education/>
- Academy launch announcement (community) — <https://community.n8n.io/t/the-n8n-academy-is-here/299695>
- Course "about" pages — QS101, N8N101, N8N102, N8N103 on `learn.n8n.io`

---

<br>

*Maintained by [Milton Valle](https://github.com/MiltonValleL) · Learning in public.*

