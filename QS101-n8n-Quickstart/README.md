# QS101 — n8n Quickstart

[![Course](https://img.shields.io/badge/course-QS101-EA4B71)](https://learn.n8n.io/courses/course-v1:n8n+QS101+2026H2/about)
[![Track](https://img.shields.io/badge/track-fast%20track-blue)]()
[![Time](https://img.shields.io/badge/est.%20time-3--5h-informational)]()
[![Status](https://img.shields.io/badge/status-in%20progress-orange)]()

> *The fastest way in.* QS101 takes you from your very first trigger to a working AI agent in one short sitting. It is the standalone fast-track course of the n8n Academy — a condensed path that touches the same core ideas as the full Foundations program, refreshed with a new AI section.

This folder holds my projects, graded assessments, and notes for QS101.

---

## What this course is about

QS101 walks you through building **real workflows** in n8n — not toy examples. You start with the basics (triggers, scheduling, HTTP requests), move into transforming data and handling errors, and finish by building an **AI agent** that looks up customer records and answers questions against real data.

By the end you should be able to:

- Build and run basic n8n workflows from scratch.
- Trigger workflows manually and on a schedule.
- Call external APIs and manage credentials safely.
- Transform, split, merge, filter, and summarize data between nodes.
- Handle errors gracefully with dedicated error workflows.
- Build a functioning AI agent connected to real data.

---

## Course structure

QS101 is organized into three progressive sections, each ending in a concrete build.

### Section 1 — Getting started
**Build:** your first workflows.

| Topic | What it covers |
|-------|----------------|
| **Triggers** | How a workflow starts — manual triggers and event-based triggers. |
| **Scheduling** | Running workflows automatically on a time-based (cron-style) schedule. |
| **HTTP Requests** | Fetching and sending data to external services with the `HTTP Request` node. |
| **Expressions** | Referencing and manipulating data dynamically between nodes. |
| **API credentials** | Storing and reusing authentication for app/service nodes securely. |

### Section 2 — Working with data
**Build:** a data pipeline with error handling.

| Topic | What it covers |
|-------|----------------|
| **Data structure** | How n8n represents items — arrays of objects, each under a `json` key. |
| **Splitting & merging** | Breaking data into items and recombining streams. |
| **Filtering** | Keeping only the items that match a condition. |
| **Summarizing** | Aggregating and condensing datasets. |
| **Error workflows** | Catching and responding to failures without breaking the run. |
| **File operations** | Reading from and writing to files (binary data handling). |

### Section 3 — Building an AI agent
**Build:** a customer-service chatbot.

| Topic | What it covers |
|-------|----------------|
| **AI Agent node** | The orchestrator that reasons and decides which tools to call. |
| **Chat models** | Connecting an LLM (OpenAI, Anthropic, Gemini, Groq, DeepSeek, …) as the agent's "brain." |
| **Memory** | Giving the agent conversational context across turns. |
| **Tool connections** | Letting the agent look up real data (e.g. customer records). |
| **System prompts** | Shaping the agent's behavior, scope, and tone. |

---

## Prerequisites

- **No coding experience required.** Some familiarity with **APIs** and **JSON** is helpful.
- A publicly accessible **n8n instance** — n8n Cloud (free trial) or self-hosted (free).
- An **API key** from a chat-model provider (OpenAI, Anthropic, Google Gemini, DeepSeek, or Groq) for the AI agent section. Free trial credits are usually enough.
- Optional: join the n8n Discord / community for help.

---

## Grading & certificate

| Component | Weight |
|-----------|-------:|
| Section quizzes | 10% |
| Hands-on workflow exercises | 55% |
| Final exam | 35% |
| **Passing grade** | **70%** overall |

> **Recommended order:** finish the hands-on workflow exercises *before* the quizzes — several quiz questions assume you already have a working workflow or agent.

Passing earns a **badge** (assigned automatically; first-time recipients get an email from the badges platform) and a **certificate of completion**. Note that QS101 is **not a formal certification**.

**Estimated completion time:** 3–5 hours.

---

## My progress

| Section | Build | Status |
|---------|-------|--------|
| 1 — Getting started | First workflows | ⬜ Not started |
| 2 — Working with data | Data pipeline + error handling | ⬜ Not started |
| 3 — Building an AI agent | Customer-service chatbot | ⬜ Not started |
| — | Final exam | ⬜ Not started |

*(Update the status icons — ⬜ → 🟠 → ✅ — as you go.)*

---

## Folder contents

```
QS101-n8n-quickstart/
├── README.md          # This file
├── projects/          # Workflows built in each section (.json exports)
├── assessments/       # Graded hands-on exercises (.json exports)
└── notes/             # Concept notes, screenshots, and gotchas
```

---

## References

- QS101 course page — <https://learn.n8n.io/courses/course-v1:n8n+QS101+2026H2/about>
- n8n Academy — <https://learn.n8n.io/>
- n8n docs — <https://docs.n8n.io/>

---

*Part of the [n8n Academy repository](../README.md) · Maintained by [Milton Valle](https://github.com/MiltonValleL).*
