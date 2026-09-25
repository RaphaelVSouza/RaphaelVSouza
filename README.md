# Raphael Vieira

Senior Fullstack Engineer — .NET · React/Next.js · Distributed Systems · AI Agent Orchestration

Brazil · Open to remote international roles (B2B or full-time)

---

## About

I build backend services in .NET, web frontends in React/Next.js, and the infrastructure that runs them.
Recently I've been working on a narrower problem: making coding agents (Claude Code, Codex, OpenCode, Antigravity CLI) safe to run unattended, with enforced scope, auditable changes and predictable cost.

## Focus areas

- **Backend:** ASP.NET Core APIs and background workers, Clean Architecture, DDD, EF Core
- **Frontend:** React, Next.js, TypeScript
- **Distributed systems:** RabbitMQ, event-driven design, Redis, PostgreSQL / SQL Server
- **Infrastructure:** Docker, Terraform, AWS (EC2, RDS, S3), CI/CD, Linux
- **Agent systems:** multi-agent orchestration, sandboxing, tool whitelisting, prompt-cache optimization

---

## Featured project

### [agent-governance-kit](https://github.com/RaphaelVSouza/agent-governance-kit)

Runner-agnostic framework for running coding agents with enforced boundaries.

**Problem:** coding agents drift out of scope, collide when run in parallel, and waste tokens on cache misses.

**How it addresses it:**

- **Scope enforcement** — git state is audited before and after each run; AST-level checks reject edits outside the declared boundary.
- **Parallel execution** — task queue on transactional `node:sqlite` with process-level mutexes and stale-claim reclamation. No external dependencies.
- **Cache efficiency** — prompts ordered static-to-volatile for byte-exact KV cache reuse; per-task reasoning-effort control.
- **Single agent definition, multiple runners** — canonical Markdown definitions compiled to Claude Code tool whitelists, OpenCode permissions and AGY agent schemas.

Supported runners: Claude Code, OpenAI Codex, OpenCode, Antigravity CLI, custom.

---

## Stack

| Area | Technologies |
| :--- | :--- |
| Backend | C#, .NET 8/9, ASP.NET Core, EF Core, LINQ |
| Frontend | React, Next.js, TypeScript, Vite, Tailwind CSS, Sass |
| Data | PostgreSQL, SQL Server, Redis, SQLite |
| Messaging | RabbitMQ |
| Infra | Docker, Docker Compose, Terraform, AWS, GitHub Actions, Bash |
| Testing | Unit, integration and mutation testing |

---

## Principles

- Explicit boundaries and low coupling over short-term shortcuts.
- Agents are treated as untrusted contributors: every change is scoped, verified and auditable.
- Technical decisions are weighed against operational cost and business impact.

---

## Contact

[LinkedIn](https://linkedin.com/in/raphaelvieiradev) · [Email](mailto:raphael5254@outlook.com)
