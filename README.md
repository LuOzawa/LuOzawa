<div align="center">

# LuOzawa

**AI Agent Engineer · AI Product Manager · FDE (Forward Deployed Engineer)**

Guangzhou, China · 23 · `Go` `Python` `TypeScript`

*I turn model capability into products that actually run in production — and can be measured.*

[Email](mailto:linlin700573@gmail.com)

</div>

---

## What I do

I work across three roles at once: I find the use case, I design the product, I write the code, and I sit on-site to make it land.

| Area | In practice |
|---|---|
| **Agent engineering** | Multi-agent orchestration, tool/skill systems, MCP integration, task queues & state machines, resumable long-running execution |
| **AI product** | Scenario diagnosis → solution design → POC → canary → launch. Owning requirements, metrics and iteration cadence end to end |
| **FDE delivery** | On-site requirement translation: turning "the customer can't articulate it" into deliverable architecture, exception branches and human-in-the-loop fallbacks |

Currently an **AI Agent Engineer** on a team building for Alibaba-related business (customer projects, details under NDA).

## Stack

![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=white)

**Engineering** — Go · Python · TypeScript / React / Next.js · PostgreSQL · Redis · Docker Compose · Playwright
**AI** — agent orchestration & skill systems · function calling / MCP · RAG · LLM-as-judge evaluation · prompt engineering · multi-model routing

## Selected work

### geo-lite — GEO (Generative Engine Optimization) platform
`Go control plane + Python browser executors`

An end-to-end system for making a brand *visible inside AI answers*: the Go service owns keyword/question pools, LLM content generation, LLM-as-judge scoring, task orchestration and a REST API; Python executors drive Playwright to publish across platforms and to query AI assistants (Doubao / DeepSeek / Tongyi).

- Executor protocol: `poll → claim → heartbeat → payload → start → result` with claim locks, TTL and a `manual_required` branch for captchas / anti-bot
- Record state machine: `pending → publishing → success / failed / skipped`
- Closes the loop *generate → distribute → verify citation* with an evaluation report

### xhs-inspiration — content discovery & rewriting workspace
`Next.js · Prisma · PostgreSQL · LLM`

An in-house topic library and AI rewriting tool for a content team: import from URL or raw text, structured material library, LLM hit-analysis plus multi-version rewrite suggestions, comments, favorites and a usage dashboard.

- Spec → plan → implementation → E2E acceptance; Prisma migrations and accessibility (aria-label) from day one
- Built from zero: data model, auth, AI routes, file service, analytics

## How I deliver (FDE playbook)

1. **Diagnose the scenario** — is this worth doing with AI at all? data availability, tolerance for error, share of manual cost. I say no when the answer is no.
2. **Smallest working loop** — a running POC within a week, validated on real data, not demo data.
3. **Define the metric first** — accuracy / automation rate / cost per item / latency, before launch. "Feels smart" is not a metric.
4. **Iterate on-site** — translate what the customer says into state machines, exception branches and human fallbacks.
5. **Hand over** — docs, scripts, runbooks, so their team can run it without me.

## Now

- 🔭 Building: reliability for long-running agent tasks — retries, idempotency, human takeover
- 🌱 Learning: agent evaluation and observability
- 💬 Happy to talk about: AI adoption decisions, GEO / AI search visibility, FDE methodology, agent engineering
- 📫 Reach me: **linlin700573@gmail.com**
