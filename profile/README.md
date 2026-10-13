# Building Safe Agentic AI for Enterprise Systems

Companion code repositories for **Building Safe Agentic AI for Enterprise Systems** by [Mohit Aggarwal](https://github.com/mohitagr18).

Each repository corresponds to a chapter in the book and contains runnable, production-grade implementations covering agentic system design, idempotency patterns, race condition settlement, multimodal RAG pipelines, and safe shutdown architectures.

---

## 🗺️ Production Architecture & Companion Code Map

Follow a single production agent request from initial user query to an idempotent, race-free committed write. Every node in the diagram below corresponds to a companion repository in this organization.

[![Interactive Architecture Map](https://img.shields.io/badge/Architecture-Explore_Interactive_Map-4F46E5?style=for-the-badge&logo=google-cloud&logoColor=white)](https://the-write-path-code.github.io/.github/)
[![Fail-Closed Security Rail](https://img.shields.io/badge/Safety-Fail--Closed_Safe_Stop-E11D48?style=for-the-badge)](https://the-write-path-code.github.io/.github/)

<a href="https://the-write-path-code.github.io/.github/" target="_blank">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/the-write-path-code/.github/main/profile/assets/architecture-map-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/the-write-path-code/.github/main/profile/assets/architecture-map-light.png">
    <img alt="Production-Grade Agentic Systems Architecture Map" src="https://raw.githubusercontent.com/the-write-path-code/.github/main/profile/assets/architecture-map-dark.png" width="100%">
  </picture>
</a>

> 💡 **Interactive Exploration:** Click the diagram above or open the [Interactive Map](https://the-write-path-code.github.io/.github/) to trace live request flows, filter by system layer, switch color themes, and jump directly to each chapter repository.

---

## 📚 Repository Map by Part

| Part / Layer | Chapter | Companion Repository | Key Capability & Invariant |
|---|---|---|---|
| **Fail-Closed Rail** | — | — | **Safe Stop Sink**: Every layer halts ungrounded or unsafe mutations before execution |
| **Part I · Scripts → Stateful Systems** | Ch 1 | [`ch01-production-reality`](https://github.com/the-write-path-code/ch01-production-reality) | Deterministic guardrails for irreversible systems & watchman trail |
| | Ch 2 | [`ch02-agent-monolith-trap`](https://github.com/the-write-path-code/ch02-agent-monolith-trap) | Moving from single-prompt monoliths to distributed Google ADK state machines |
| **Part II · Grounding the Agent** | Ch 6 | [`ch06-multimodal-perception`](https://github.com/the-write-path-code/ch06-multimodal-perception) | Grounded multimodal perception & `PerceptionChunk` contract |
| | Ch 3 | [`ch03-taming-hallucination-puzzle`](https://github.com/the-write-path-code/ch03-taming-hallucination-puzzle) | Dense and sparse hybrid retrieval with BGE-M3 & Qdrant |
| | Ch 5 | [`ch5-curing-enterprise-hallucination-crisis`](https://github.com/the-write-path-code/ch5-curing-enterprise-hallucination-crisis) | 3-state CRAG gatekeeper & SR-RAG recursive critique loops |
| | Ch 4 | [`ch04-debugging-hallucinations-math`](https://github.com/the-write-path-code/ch04-debugging-hallucinations-math) | 5-layer mathematical evaluation stack & calibrated grounding thresholds |
| **Part III · Context-Aware Actuation** | Ch 7 | [`ch07-proactive-event-driven-agents`](https://github.com/the-write-path-code/ch07-proactive-event-driven-agents) | Event-driven agents, spatial privacy with H3 indexing & local execution |
| | Ch 8 | [`ch8-model-context-protocol`](https://github.com/the-write-path-code/ch8-model-context-protocol) | Model Context Protocol (MCP) typed schema boundaries & tool execution |
| | Ch 9 | [`ch09-plant-doctor`](https://github.com/the-write-path-code/ch09-plant-doctor) | End-to-end case study: Multimodal diagnosis & Cloud Run deployment |
| **Part IV · Hardened Persistence Boundary** | Ch 10 | [`ch10-cloud-agent-patterns`](https://github.com/the-write-path-code/ch10-cloud-agent-patterns) | Stateless FastAPI workers decoupled from volatile in-memory cache |
| | Ch 14 | [`ch14-enterprise-ai-assistant`](https://github.com/the-write-path-code/ch14-enterprise-ai-assistant)<br>[`ch14-homecare-visit-triage-agent`](https://github.com/the-write-path-code/ch14-homecare-visit-triage-agent) | Deny-by-default action boundaries, policy gates & approval holds |
| | Ch 11–13 | [`ch11-13-ucp-a2a-payment-integrity`](https://github.com/the-write-path-code/ch11-13-ucp-a2a-payment-integrity) | Request identity, durable idempotency ledgers & optimistic concurrency control (OCC) |
| **Part V · Continuous Verification** | Ch 15 | [`ch15-agentic-cicd`](https://github.com/the-write-path-code/ch15-agentic-cicd) | Offline eval merge gates, prompt drift detection & automated red-teaming in CI/CD |

---

**Author:** [Mohit Aggarwal](https://github.com/mohitagr18)
