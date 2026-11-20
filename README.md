# Raphael Vieira

**AI Engineer** — agentic tooling, context architecture, LLM cost control
Full-stack: TypeScript, React/Next.js, .NET

Brazil · Open to remote international roles (B2B or full-time)
[LinkedIn](https://linkedin.com/in/raphaelvieiradev) · [Email](mailto:raphael5254@outlook.com)

---

## About

I build the systems other people build on: agents, skills, plugins and the guardrails around them, plus the front ends and services they run behind.

For 5+ years I've shipped production software at a marketing agency (ERPs, complex React page builders, large Next.js and Astro sites), working side by side with designers. My current focus is AI engineering:

- **Safe agents** — coding agents that run unattended with enforced scope, auditable changes and predictable cost.
- **Context architecture** — retrieval-ready knowledge pipelines with hard budget ceilings.
- **Measured, not guessed** — how context size drives hallucination, so retrieval stays cheap and accurate.

I decide the shape of each tool (agent, skill, plugin, hook or service), record the reasoning in numbered ADRs, and ship metrics, audit trails and benchmarks as part of the deliverable.

---

## Open source

### [Oathbound](https://github.com/RaphaelVSouza/Oathbound)

Governance layer for CLI coding agents. One source, native plugins for Claude Code, Codex CLI and Antigravity CLI.

- Coordinator agent with 7 specialized subagents and 10 engineering skills (ADRs, specs, API contracts, safe refactoring, test strategy).
- Deterministic guardrails in a native Rust hook binary: audit trail, read-only and destructive-command guards, read-size limits.
- Installer with SHA-256 manifests that preserves local edits and shows diffs on upgrade.

### [caipora](https://github.com/RaphaelVSouza/caipora)

Architecture inventory for Git repositories: a machine-readable `architecture.json`, an offline HTML report with dependency diagrams, and a Markdown index agents can read. Fails CI on complexity thresholds. Zero runtime dependencies.

### [pedido-hortifruti](https://github.com/RaphaelVSouza/pedido-hortifruti) · [live demo](https://raphaelvsouza.github.io/pedido-hortifruti/)

Offline-first PWA that turns a produce supplier's WhatsApp promo into a ready-to-send order. No backend or runtime dependencies, JSDoc types checked by TypeScript in CI, corpus-based parser tests and a Playwright E2E suite.

---

## Private work

Walkthroughs available on request.

| Project | What it is | Highlights |
| :--- | :--- | :--- |
| **Colheita** | Knowledge ingestion pipeline and RAG data lake | Tiered cost cascade (cache, deterministic, local parser, selective vision model), mandatory budget ledger, LLM judges calibrated against a gold set, hallucination measured against context size |
| **Mango Study** | Adaptive learning platform on Cloudflare Workers | Gateway with no public route (RPC via Service Binding), Cloudflare Access JWT, D1, LLM tutor, embeddings search |
| **Client Video Kit** | Branded video production for non-technical operators | AI voice-over, word-level captions, per-brand configuration, a Claude Code skill and desktop forms that guide each job, self-contained bundles for Windows, macOS and Linux |

---

## Stack

| Area | Technologies |
| :--- | :--- |
| AI engineering | Claude Code plugins, skills, subagents and hooks; Codex CLI; Antigravity CLI; RAG and embeddings; LLM-as-judge and evaluation sets; token budgets, quotas, caching, model fallback; Gemini and ElevenLabs APIs |
| Frontend | React, Next.js, Astro, TypeScript, Vite, Tailwind CSS, Sass |
| Backend | TypeScript/Node.js, Python, C#, .NET 8/10, ASP.NET Core, EF Core, Rust |
| Data | SQL Server, Redis, SQLite, Cloudflare D1 |
| Auth | SAML2, JWT, Okta, Cloudflare Access |
| Infra | Docker, Cloudflare Workers, GitHub Actions, Bitbucket Pipelines, PowerShell, Bash |
| Testing | xUnit, MSTest, Vitest, Playwright, node:test, pytest |

---

## Principles

1. Pick the smallest shape that solves the need. Sometimes the tool someone asked for should be a skill, a hook, or nothing at all.
2. Agents are untrusted contributors. Every change is scoped, verified and auditable.
3. Cost, latency and observability are part of the design, not a follow-up.
4. Explicit boundaries and low coupling over short-term shortcuts.
