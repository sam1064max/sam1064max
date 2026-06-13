# Profile Strategy — sam1064max

## Positioning

**Target Identity**: Staff/Principal AI Platform Engineer operating at the intersection of AI Architecture, Agentic Systems, and Production Infrastructure.

**Not**: A generic full-stack developer, a notebook practitioner, or an ML researcher.

**Is**: An engineer who builds entire AI platforms — from inference to retrieval to guardrails to observability — and ships them to production.

---

## Strengths

| Strength | Evidence |
|---|---|
| Full-stack AI platform ownership | `rag-platform-qwen3`: RAG + agents + guardrails + eval + observability in one system |
| Production-grade agentic systems | `enterprise-nested-langgraph` (140 tests, 90% coverage), `supervisor` (111 tests, 96% coverage) |
| Multi-agent orchestration | LangGraph hierarchical graphs, Supervisor pattern, Planner-Executor, Router Agent |
| Infrastructure maturity | Docker, Terraform (HCL), CI/CD, self-hosted stack (Qdrant, vLLM, MinIO, OpenBao) |
| Observability & evaluation | OpenTelemetry, Langfuse, Prometheus, Grafana, RAGAS, DeepEval |
| Security consciousness | NeMo Guardrails, STRIDE threat modeling, prompt injection defense |
| AdTech domain expertise | NLP2SQL Analytics Copilot for AdTech intelligence |
| Google-level engineering rigor | 100% type hints, Ruff, Mypy, Pydantic v2, structured logging |

---

## Differentiators

1. **Platform thinker** — doesn't just build models; builds the infrastructure around them
2. **Architecture-first** — full Mermaid diagrams, component docs, security specs before code
3. **Test-obsessed** — 90-96% coverage on LLM systems (rare in the industry)
4. **Self-hosted conviction** — builds on-prem AI platforms, not just cloud-managed services
5. **Agentic depth** — multiple agent patterns (Supervisor, Router, Planner-Executor, hierarchical) not just a single LangChain call

---

## Target Audience

| Audience | What they look for | What we show |
|---|---|---|
| Engineering Directors | Can this person own a platform? | End-to-end RAG platform with 6+ components |
| CTOs | Does this person think in systems? | Architecture diagrams, security docs, evaluation strategy |
| Staff Engineers | Is the code production-grade? | 96% test coverage, type hints, structured logging |
| Founders | Can this person build from 0→1? | Self-hosted infra, full stack ownership |
| Recruiters (senior roles) | Does this match Staff/Principal bar? | Google tenure, platform scope, technical depth |

---

## Positioning Statement

> 10+ years building ML systems, AI platforms, distributed data products, and production-grade LLM applications. Currently building agentic AI platforms at Google. Specializing in RAG systems, multi-agent orchestration, LLMOps, and production AI infrastructure.

---

## Commit Strategy

Phase 1: `docs(profile): define profile strategy`
Phase 2-13: `feat(profile): ...` (per section)
Phase 14: `feat(profile): automate profile maintenance`
Phase 15: `docs(profile): document landing page architecture`
Phase 16: `docs(pr): document profile redesign` → merge → `chore(release): v1.0.0`
