<h1 align="center">Sushant Shambharkar</h1>

<p align="center">
  <strong>AI Architect · Agentic AI Platform Engineer · MLOps · Distributed Systems</strong>
</p>

<p align="center">
  Building production AI platforms, agentic systems, and LLM infrastructure at Google.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/sushant-shambharkar-b6242658"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://github.com/sam1064max?tab=repositories"><img src="https://img.shields.io/badge/Repos-35-181717?style=for-the-badge&logo=github&logoColor=white" alt="Repos"></a>
  <img src="https://img.shields.io/badge/Followers-4-181717?style=for-the-badge&logo=github&logoColor=white" alt="Followers">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <a href="https://github.com/sam1064max/rag-platform-qwen3/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License"></a>
</p>

---

## About

I design and build **production AI platforms** — not prototypes, not notebooks, not demos.

Over 10+ years in ML/AI, I've shipped systems across AdTech, NLP, distributed data, and now **agentic AI infrastructure**. My work spans the full stack: from vector databases and inference runtimes to guardrails, evaluation frameworks, and observability pipelines.

Currently at **Google**, building agentic AI platforms with multi-agent orchestration, RAG systems, and LLM ops infrastructure.

**What I build:**
- End-to-end RAG platforms (ingestion → retrieval → generation → evaluation)
- Multi-agent orchestration systems (Supervisor, Router, Planner-Executor patterns)
- LLM guardrails and safety infrastructure
- Production observability for AI systems (traces, metrics, dashboards)
- Self-hosted AI infrastructure (vLLM, Qdrant, MinIO, on-prem deployments)

**What I don't do:**
- Build models — I build the platforms that run them
- Ship without tests — 90-96% coverage on LLM systems
- Ignore security — STRIDE threat modeling, prompt injection defense
- Skip documentation — full architecture diagrams before code

---

## Current Focus

```
Agentic AI Platforms    AI Evaluation    LLMOps
Multi-Agent Systems     Inference Optimization    AI Platform Engineering
```

---

## Core Expertise

| Domain | Depth |
|---|---|
| **AI Architecture** | End-to-end platform design — retrieval, generation, guardrails, evaluation, observability |
| **Agentic AI** | Multi-agent orchestration with LangGraph — Supervisor, Router, Hierarchical, Planner-Executor |
| **LLMOps** | LLM observability (Langfuse, OTel), evaluation (RAGAS, DeepEval), prompt management |
| **MLOps** | Model serving (vLLM), feature stores, pipeline orchestration, CI/CD for ML |
| **Distributed Systems** | Self-hosted infrastructure, container orchestration, secrets management |
| **Data Engineering** | NLP2SQL, analytics pipelines, AdTech intelligence platforms |

---

## Featured Projects

### rag-platform-qwen3 — Production RAG Platform

> Self-hosted, production-grade Retrieval-Augmented Generation platform with agent orchestration, hybrid retrieval, and comprehensive safety infrastructure.

**Architecture:** FastAPI → Guardrails → Agent Runtime → Hybrid Retrieval → Reranking → Generation

| Component | Technology |
|---|---|
| LLM Inference | vLLM + Qwen3-32B-Instruct |
| Embeddings | Qwen3-Embedding-8B |
| Vector Store | Qdrant (dense) + BM25 (sparse) + RRF fusion |
| Guardrails | NeMo Guardrails (prompt injection, PII, toxicity) |
| Agent Runtime | LangGraph (plan → act → observe) |
| Evaluation | RAGAS + DeepEval with golden datasets |
| Observability | OpenTelemetry + Langfuse + Prometheus + Grafana |
| Secrets | OpenBao (self-hosted Vault) |
| Infrastructure | Docker, Terraform (HCL), Makefile |

[Architecture Docs](https://github.com/sam1064max/rag-platform-qwen3/blob/main/docs/architecture.md) · [Security Spec](https://github.com/sam1064max/rag-platform-qwen3/blob/main/docs/security.md) · [API Spec](https://github.com/sam1064max/rag-platform-qwen3/blob/main/docs/spec.md) · [Repository](https://github.com/sam1064max/rag-platform-qwen3)

---

### enterprise-nested-langgraph — Hierarchical Multi-Agent System

> Production-grade multi-agent research and analytics system with nested LangGraph architecture, typed state, and defense-in-depth guardrails.

**Architecture:** Supervisor → Research Subgraph | Analytics Subgraph | Reporting Subgraph

| Metric | Value |
|---|---|
| Tests | 140 passed |
| Coverage | 90% |
| Type Hints | 100% |
| Linter | Ruff clean |
| Type Checker | Mypy clean |

[Repository](https://github.com/sam1064max/enterprise-nested-langgraph)

---

### supervisor — Supervisor Pattern Reference Implementation

> Reference implementation of the Supervisor Pattern for multi-agent LLM systems. Dynamic routing, parallel fan-out, bounded reflection, and human-in-the-loop checkpoints.

**Architecture:** Input Guardrail → Supervisor → Research / Analytics / Calculator → Writer ↔ Reviewer → Output Guardrail

| Metric | Value |
|---|---|
| Tests | 111 passed |
| Coverage | 96% |
| All LLM calls mocked | Yes (hermetic tests) |

[Repository](https://github.com/sam1064max/supervisor)

---

### NLP2SQL — Natural Language Analytics for AdTech

> NLP2SQL Analytics Copilot — natural language interface for AdTech intelligence. Translates business questions into SQL queries against complex analytics schemas.

[Repository](https://github.com/sam1064max/NLP2SQL) *(private)*

---

### ai-audiobook-generator — TTS Pipeline

> Production-quality audiobook generation pipeline converting markdown lectures into narrated audio using Kokoro and Chatterbox-Turbo.

[Repository](https://github.com/sam1064max/ai-audiobook-generator)

---

### Agent Pattern Library

| Pattern | Repository | Description |
|---|---|---|
| Router Agent | [RouterAgent](https://github.com/sam1064max/RouterAgent) | LLM-based routing to specialist agents |
| Router (No LLM) | [Router-Agent-NoLLM](https://github.com/sam1064max/Router-Agent-NoLLM) | Deterministic routing without LLM overhead |
| Planner-Executor | [Planner-Executor](https://github.com/sam1064max/Planner-Executor) | Plan decomposition and task execution |

---

## Architecture Portfolio

Six production platforms, each with full architecture documentation:

| Platform | Components | Documentation |
|---|---|---|
| **RAG Platform** | Ingestion, Hybrid Retrieval, Reranking, Generation, Guardrails, Evaluation, Observability | [architecture.md](https://github.com/sam1064max/rag-platform-qwen3/blob/main/docs/architecture.md) |
| **Agent Platform** | Supervisor, Router, Hierarchical Subgraphs, Tool Selection, HITL | [supervisor](https://github.com/sam1064max/supervisor) |
| **Evaluation Platform** | RAGAS, DeepEval, Golden Datasets, Acceptance Criteria | [spec.md#evaluation](https://github.com/sam1064max/rag-platform-qwen3/blob/main/docs/spec.md) |
| **Guardrails Platform** | NeMo, Prompt Injection, PII, Toxicity, Citation Verification | [security.md](https://github.com/sam1064max/rag-platform-qwen3/blob/main/docs/security.md) |
| **Observability Platform** | OpenTelemetry, Langfuse, Prometheus, Grafana | [architecture.md#observability](https://github.com/sam1064max/rag-platform-qwen3/blob/main/docs/architecture.md) |
| **Self-Hosted Infrastructure** | vLLM, Qdrant, MinIO, OpenBao, Gitea, Docker Compose | [homelab](https://github.com/sam1064max/homelab) |

---

## Technology Map

### AI & LLMs
`Qwen3` · `vLLM` · `LangGraph` · `LangChain` · `NeMo Guardrails` · `HuggingFace` · `RAGAS` · `DeepEval`

### Vector & Retrieval
`Qdrant` · `BM25` · `RRF Fusion` · `Hybrid Search` · `Reranking`

### MLOps & LLMOps
`MLflow` · `Langfuse` · `OpenTelemetry` · `Prometheus` · `Grafana` · `LangSmith`

### Data & Analytics
`NLP2SQL` · `FastAPI` · `Pydantic v2` · `PostgreSQL` · `MinIO`

### Cloud & Infrastructure
`Docker` · `Terraform (HCL)` · `GitHub Actions` · `Gitea` · `OpenBao` · `NVIDIA A100`

### Engineering Quality
`Python 3.10+` · `Ruff` · `Mypy` · `Pytest` · `100% Type Hints` · `MIT License`

---

## Selected Impact

| Outcome | Context |
|---|---|
| Built end-to-end self-hosted RAG platform | 6+ components, production-grade, full observability stack |
| Shipped multi-agent systems with 96% test coverage | LLM systems with hermetic test suites (no network calls) |
| Designed hierarchical agent architecture | Parent → child subgraph composition with typed state |
| Implemented comprehensive AI safety infrastructure | NeMo guardrails, STRIDE threat modeling, prompt injection defense |
| Delivered NLP2SQL analytics for AdTech | Natural language interface for complex analytics schemas |
| Built production TTS pipelines | Markdown → narrated audio with Kokoro and Chatterbox-Turbo |
| Created self-hosted AI infrastructure | vLLM + Qdrant + MinIO + OpenBao on commodity hardware |
| Reduced LLM evaluation cycle from days to minutes | RAGAS + DeepEval with golden datasets and CI integration |

---

## Speaking & Leadership

**Technical Leadership**
- Architecture owner for AI platform initiatives
- Led multi-agent system design across research, analytics, and reporting domains
- Established engineering standards: type safety, test coverage, structured logging, documentation-first

**Mentoring**
- Guided teams on LangGraph adoption and multi-agent orchestration patterns
- Established testing practices for LLM systems (mocking, hermetic suites, coverage targets)

**Architecture Ownership**
- Full platform architecture: system context → container → component → deployment diagrams
- Security architecture: threat modeling, guardrail design, secrets management

---

## Current Learning

```
Multi-Agent Orchestration    AI Evaluation Frameworks    Inference Optimization
LLMOps Platform Design       Agentic AI Patterns         Self-Hosted AI Infrastructure
```

---

## Open Source

All key projects are open source under MIT License:

| Project | License | Status |
|---|---|---|
| rag-platform-qwen3 | MIT | Active |
| enterprise-nested-langgraph | MIT | Active |
| supervisor | MIT | Active |
| ai-audiobook-generator | MIT | Active |

---

## Contact

<p align="center">
  <a href="https://www.linkedin.com/in/sushant-shambharkar-b6242658"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://github.com/sam1064max"><img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"></a>
  <a href="mailto:sam1064max@gmail.com"><img src="https://img.shields.io/badge/Email-sam1064max@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

---

<p align="center">
  <sub>Built with production-grade intent. No templates. No fluff. Just systems.</sub>
</p>

<!-- profile:version:v1.0.1 -->
