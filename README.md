# Building Safe Agentic AI for Enterprise Systems

Companion code for **Building Safe Agentic AI for Enterprise Systems** by [Mohit Aggarwal](https://github.com/mohitagr18) · Wiley-IEEE Press.

There's no undo button once an AI agent touches enterprise state — a network retry becomes a duplicate charge, a confident hallucination becomes a corrupted customer record. Each repository below corresponds to a chapter in the book and contains runnable implementations of the patterns that keep write-path agents safe: deterministic guardrails, idempotency keys, optimistic concurrency control, grounded multimodal retrieval, and fail-closed shutdown.

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

> 💡 **Interactive Exploration:** Click the diagram above or open the [Interactive Map](https://the-write-path-code.github.io/.github/) to trace the request flow and jump directly to each chapter's repository.

---

## 📚 Repository Map by Part

A fail-closed rail runs through every layer below: ungrounded or unsafe mutations are halted before execution.

| Part | Chapter | Companion Repository | Key pattern |
|---|---|---|---|
| **Part I · Scripts → Stateful Systems** | Ch 1 | [`ch01-production-reality`](https://github.com/the-write-path-code/ch01-production-reality) | Deterministic guardrails for irreversible systems & the watchman trail |
| | Ch 2 | [`ch02-agent-monolith-trap`](https://github.com/the-write-path-code/ch02-agent-monolith-trap) | From single-prompt monoliths to distributed state machines with Google ADK |
| **Part II · Grounding the Agent** | Ch 3 | [`ch03-taming-hallucination-puzzle`](https://github.com/the-write-path-code/ch03-taming-hallucination-puzzle) | Hybrid retrieval (dense + sparse) that stops missing exact part numbers and account IDs |
| | Ch 4 | [`ch04-debugging-hallucinations-math`](https://github.com/the-write-path-code/ch04-debugging-hallucinations-math) | A 5-layer evaluation stack that pinpoints where a hallucination actually happened |
| | Ch 5 | [`ch05-curing-enterprise-hallucination-crisis`](https://github.com/the-write-path-code/ch05-curing-enterprise-hallucination-crisis) | Corrective RAG that repairs incomplete or stale evidence instead of guessing |
| | Ch 6 | [`ch06-multimodal-perception`](https://github.com/the-write-path-code/ch06-multimodal-perception) | Typed perception contracts (`PerceptionChunk`) across PDFs, images, and audio |
| **Part III · Context-Aware Actuation** | Ch 7 | [`ch07-proactive-event-driven-agents`](https://github.com/the-write-path-code/ch07-proactive-event-driven-agents) | Event-driven agents with spatial privacy via H3 indexing and local execution |
| | Ch 8 | [`ch08-model-context-protocol`](https://github.com/the-write-path-code/ch08-model-context-protocol) | MCP typed schema boundaries that sandbox tool definitions |
| | Ch 9 | [`ch09-plant-doctor`](https://github.com/the-write-path-code/ch09-plant-doctor) | End-to-end case study: multimodal diagnosis deployed to Cloud Run |
| **Part IV · Hardened Persistence Boundary** | Ch 10 | [`ch10-cloud-agent-patterns`](https://github.com/the-write-path-code/ch10-cloud-agent-patterns) | Stateless agents that survive container restarts — retrieval decoupled from volatile memory |
| | Ch 11–13 | [`ch11-13-ucp-a2a-payment-integrity`](https://github.com/the-write-path-code/ch11-13-ucp-a2a-payment-integrity) | Idempotency keys and optimistic concurrency control — retries never become duplicate charges |
| | Ch 14 | [`ch14-enterprise-ai-assistant`](https://github.com/the-write-path-code/ch14-enterprise-ai-assistant)<br>[`ch14-homecare-visit-triage-agent`](https://github.com/the-write-path-code/ch14-homecare-visit-triage-agent) | Deny-by-default action boundaries, policy gates, and approval holds |
| **Part V · Continuous Verification** | Ch 15 | [`ch15-agentic-cicd`](https://github.com/the-write-path-code/ch15-agentic-cicd) | Merge gates that block accuracy regressions before they reach production |

---

**Author:** [Mohit Aggarwal](https://github.com/mohitagr18)
