# AI Engineering Portfolio

Selected engineering work by
[Giacomo Germano](https://github.com/giack891811), Junior AI Engineer based in
Lugano, Switzerland.

Public landing page for Instagram, LinkedIn and access requests:
[Governed Enterprise Agents](./index.html)

Mobile link hub for Instagram bio:
[Official links](./links.html)

> The source repositories are private. This public portfolio documents the
> problems addressed, architecture, technology choices, safety boundaries and
> validation evidence without exposing proprietary code, credentials or data.

## Portfolio overview

| Project | Domain | Main stack | Status |
|---|---|---|---|
| [MirrorSkills](#flagship-mirrorskills) | Enterprise agentic AI and governance | Next.js, TypeScript, PostgreSQL/pgvector, LangGraph, Ollama | Flagship private MVP |
| [AI & ML Agent](#ai--ml-agent) | Applied AI / ML platform | Python, FastAPI, LangGraph, pgvector, Redis | Validated private project |
| [VisibilAI](#visibilai) | GEO/AEO analytics | TypeScript, Python, PostgreSQL, ClickHouse | Active private project |
| [Realtime Translator](#realtime-translator) | Speech AI | faster-whisper, NLLB, FastAPI, React | Local MVP |
| [Agentic Trader](#agentic-trader) | Agentic analysis | Python, FastAPI, IBKR, TradingView | Active advisory system |
| [RedBenchOps](#redbenchops) | LLM evaluation | FastAPI, Next.js, Redis, pgvector | Advanced prototype |
| [Syntropiix Control Plane](#syntropiix-control-plane) | Agent orchestration | React, Python, Claude Agent SDK | Active private project |
| [Syntrocyber](#syntrocyber) | AI security | Python, policies, audit and testing | Defensive R&D suite |
| [Quantum / Willow Lab](#quantum--willow-lab) | Quantum experiments | Python, Cirq, Claude Agent SDK | Experimental lab |

---

## Flagship: MirrorSkills

**Role in the portfolio:** MirrorSkills is the principal engineering project
behind the SYNTROPIIX product vision. It is a private enterprise agentic-AI
platform designed for organizations that require useful automation without
giving agents uncontrolled authority.

**Problem:** Enterprise agents must operate across company data, tools and
workflows while preserving human accountability, tenant isolation,
traceability, cost control and European data-governance requirements.

**Platform capabilities:**

- assigns personal or profession-scoped AI agents to employees;
- organizes eight vertical-agent profiles around business functions;
- routes sensitive actions through an OODA-H human-approval workflow;
- applies more than 250 risk-graded permissions and organization-level policy
  controls;
- separates execution and review through a Doer/Critic architecture;
- supports hybrid model routing across self-hosted Ollama and explicitly
  enabled cloud providers;
- combines multi-tenant PostgreSQL, pgvector knowledge retrieval, agent
  workflows and operational services;
- provides audit-oriented records, governance gates and controls designed
  around EU AI Act, GDPR and Swiss FADP concerns;
- includes deployment, monitoring, backup and launch-readiness assets.

**Main engineering stack:** Next.js, TypeScript, PostgreSQL, Drizzle ORM,
pgvector, LangGraph, LiteLLM, Ollama, Redis, Docker, Playwright and GitHub
Actions.

**Engineering evidence:** The local private workspace contains 368 test files,
13 workflow definitions and 20 Docker-related assets. Recent launch-readiness
work records more than 2,500 passing automated checks, while known failures
remain explicitly tracked rather than hidden.

**Current maturity:** Advanced private MVP under continued infrastructure,
coverage and launch-readiness hardening. It is not presented as formally
certified for regulatory compliance or as a finished customer-production
deployment.

**Confidentiality:** Source code, operating configuration and proprietary
product documentation remain private. This case study intentionally exposes
only capabilities, architecture and verifiable engineering evidence.

---

## AI & ML Agent

**Problem:** AI demos often stop at a single prompt and do not provide
production controls, evaluation, persistence or a repeatable data-science
workflow.

**Solution:** A production-oriented agent runtime combining:

- FastAPI REST and WebSocket interfaces;
- LangGraph orchestration and controlled tool execution;
- hybrid RAG with PostgreSQL/pgvector;
- Redis-backed runtime services;
- AWS Bedrock with a configurable provider fallback;
- EDA, AutoML, model registry and prediction endpoints;
- Docker and infrastructure-as-code assets.

**Engineering evidence:** 59 automated tests verified locally, CI workflows,
mock providers for credential-free development, and documented security and
disaster-recovery boundaries.

**Source:** Private repository.

---

## VisibilAI

**Problem:** Companies cannot easily measure how often answer engines cite
their brand or translate visibility gaps into concrete technical and editorial
actions.

**Solution:** A B2B GEO/AEO platform that:

- tracks visibility across answer engines;
- verifies domain ownership before crawling;
- audits AI-bot accessibility, structured data and content architecture;
- generates `llms.txt`, JSON-LD, content briefs and prioritized action plans;
- supports deterministic local fallbacks when provider keys are unavailable.

**Stack:** TypeScript monorepo, Python pipeline, PostgreSQL, Redis, ClickHouse,
Docker and Playwright.

**Engineering evidence:** 18 commits, 195 source files, 75 test files, CI,
Docker configuration, a documented demo flow and dashboard screenshots.

**Source:** Private repository.

---

## Realtime Translator

**Problem:** Real-time multilingual conversation requires reliable segmentation,
ASR, translation and TTS while preventing incomplete speech from being sent
prematurely.

**Solution:** A local Windows MVP for Italian, English and German:

- faster-whisper ASR;
- NLLB-200 translation through CTranslate2;
- WebSocket streaming;
- explicit voice-send gate;
- optional TTS;
- consent, audit and diagnostic export;
- sandboxed voice-cloning interfaces disabled by default.

**Engineering evidence:** 223 tests passed and 2 skipped in the latest local
verification.

**Source:** Private repository.

---

## Agentic Trader

**Problem:** Market screeners often produce opaque signals and mix analysis
with execution risk.

**Solution:** A read-only strategy scanner that:

- screens multi-market data;
- converts strategies and approved educational material into structured rules;
- evaluates market structure and volume evidence;
- ranks matches and explains why they qualify;
- supports backtesting and a knowledge-grounded assistant;
- never places, changes or cancels orders.

**Safety boundary:** Trading remains manual. The execution path is isolated and
disabled, while the application focuses on evidence-based advisory output.

**Engineering evidence:** 745 tests passed in the latest local verification.

**Source:** Private repository.

---

## RedBenchOps

**Problem:** LLM robustness work needs repeatability, authorization, budgets and
responsible reporting—not only collections of prompts.

**Solution:** An asynchronous testing platform with:

- Tree of Attacks with Pruning workflows;
- semantic similarity and persisted pruning evidence;
- Redis queues and live dashboard events;
- campaign budgets, rate limits and circuit breakers;
- allowlisted targets and authorization records;
- human review, audit logs and responsible-disclosure workflow;
- exportable vendor reports and monitoring.

**Status:** Advanced private prototype. Repository hardening and CI publication
are in progress.

**Source:** Private repository.

---

## Syntropiix Control Plane

**Problem:** Multiple specialized agents need a consistent knowledge layer,
orchestration controls and an operational dashboard.

**Solution:** A control plane combining:

- an administrative React dashboard;
- profession-scoped agents built with the Claude Agent SDK;
- a reproducible IT knowledge-base pipeline;
- monitoring and reflective orchestration;
- read-only integration boundaries with MirrorSkills.

**Source:** Private organization repository.

---

## Syntrocyber

**Problem:** Agentic applications introduce risks such as prompt injection,
excessive tool access, poisoned knowledge, memory leakage and weak auditability.

**Solution:** A defensive suite covering:

- input inspection and output sanitization;
- tool allowlists and capability controls;
- namespaced memory and retention policies;
- knowledge-base integrity and drift detection;
- defensive red-team campaigns;
- regression generation and evidence reports;
- CRS audit-portal integration.

**Engineering evidence:** 33 test files detected across the consolidated local
suite. Benchmark publication is a planned next step.

**Source:** Private repository.

---

## Quantum / Willow Lab

**Purpose:** A small experimental laboratory for learning quantum-circuit
construction and exploring how an AI assistant can explain experiment results.

**Stack:** Python, Cirq, Cirq Google, local web UI and Claude Agent SDK.

**Status:** Experimental private repository. It is presented as a learning lab,
not as quantum-hardware research.

---

## Additional private work

- **AI Job Search Agent:** tested Claude Agent SDK application for aggregating,
  ranking and reviewing remote AI opportunities.
- **TradingView–IBKR Bridge:** paper-first webhook bridge with authentication,
  replay prevention, risk limits and a kill switch.
- **PATENTOM:** patent-intelligence and code-IP analysis platform.
- **PR_Soraya:** reproducible scientific-run and evidence-management R&D.

## Background and contact

I bring more than 15 years of experience troubleshooting security,
electromechanical and electronic access-control systems. I am currently
completing a Computer Engineering degree and hold the IBM Generative AI
Engineering Professional Certificate, the IBM RAG and Agentic AI Professional
Certificate and the Claude with Amazon Bedrock certificate.

[LinkedIn](https://www.linkedin.com/in/giacomo-germano-4079491b9/) ·
[GitHub profile](https://github.com/giack891811)
