<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/multinex-ai/.github/master/assets/banner.jpg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/multinex-ai/.github/master/assets/banner.jpg">
    <img alt="Multinex" src="https://raw.githubusercontent.com/multinex-ai/.github/master/assets/banner.jpg" width="100%">
  </picture>
</p>

<p align="center">
  <strong>The Security, Identity, and Audit Layer for the Agentic Generation.</strong><br>
  <sub>Solving the AI Trust Crisis with mandatory infrastructure for production-grade AI agents.</sub>
</p>

<p align="center">
  <a href="https://multinex.ai"><img src="https://img.shields.io/badge/site-multinex.ai-D4A843?style=flat-square" alt="Website"></a>
  <a href="https://billing.multinex.ai/signup"><img src="https://img.shields.io/badge/sign_up-free_trial-10B981?style=flat-square" alt="Sign Up"></a>
  <a href="https://status.multinex.ai"><img src="https://img.shields.io/badge/status-operational-FFC857?style=flat-square" alt="Status"></a>
  <a href="https://github.com/multinex-ai"><img src="https://img.shields.io/badge/org-multinex--ai-0D1117?style=flat-square&logo=github&logoColor=white" alt="GitHub Org"></a>
  <img src="https://img.shields.io/badge/rust-%23000000.svg?style=flat-square&logo=rust&logoColor=white" alt="Rust">
  <img src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/deno-000000?style=flat-square&logo=deno&logoColor=white" alt="Deno">
</p>

---

## About

**Multinex AI** builds the infrastructure layer that production AI stacks are missing: memory, identity, security, policy, billing, and runtime orchestration — unified in a single ecosystem.

AI models and autonomous agents introduce a radical new attack surface — prompt injection, PII leakage, and model poisoning. Multinex solves this through:

- **Zero Trust Architecture** — Every agent action is verified. Prompts, secrets, and tool calls are secured before sensitive data reaches a model.
- **Memory-Native Infrastructure** — Agents accumulate knowledge across sessions via MemQ's tiered architecture (HOT → WARM → COLD).
- **Agent Identity** — Strong cryptographic identity (VISA verification) for autonomous actors.
- **Immutable Audit** — Tamper-proof logs of all model and memory interactions.

---

## Products & Ecosystem

<table>
<tr>
<td width="50%">

### 🛡️ [Multinex Aieges Shield](https://github.com/multinex-ai/munx-aieges-shield)

Zero-trust AI security suite — prompt injection defense, PII/secret protection, local scanning, and policy enforcement.

![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=flat-square&logo=rust&logoColor=white)

- `<1ms` latency via the ~6.5 MB Rust-native proxy
- 65+ prompt injection patterns out of the box
- Desktop daemon + browser extension
- Zero external dependencies, on-prem first

</td>
<td width="50%">

### 🧠 [MemQ — Sovereign Memory for AI](https://multinex.ai/memq)

Hosted MCP-native memory and retrieval plane for AI agents with namespaces, quotas, durable checkpoints, and inference-backed promotion.

![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white)

- **+42 pts** primary@1 vs Mem0 OSS in retrieval benchmarks
- **-2498 ms** avg latency delta vs Mem0 OSS
- 25+ auto-discovered MCP tools
- Hosted endpoint: `mcp.multinex.ai`

</td>
</tr>
<tr>
<td width="50%">

### ⚔️ [Munx Legion](https://github.com/multinex-ai/munx-legion)

Agent governance, swarm visualization, policy routing, evidence capture, and operator-facing runtime surfaces.

![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white)

- Swarm process management
- Git-in-the-Loop stacked PR protocol
- Multi-agent task boards & config generation
- VISA identity-aware orchestration

</td>
<td width="50%">

### 🔧 [Munx CLI](https://github.com/multinex-ai/multinex)

Rust command interface for realm bootstrap, product audit, memory calls, tool schemas, planning, and operator workflows.

![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=flat-square&logo=rust&logoColor=white)

- Realm bootstrap & product audit
- MemQ memory operations from the terminal
- Swarm process orchestration (tmux-native)
- Legion compliance & planning tools

</td>
</tr>
</table>

---

## Platform Architecture

```text
                         ┌───────────────────────────────────────┐
                         │    MARS — Multi-Agent Runtime System   │
                         │   Planning · Execution · Reflection   │
                         │   VISA Identity · Airlock Governance   │
                         └──────────────────┬────────────────────┘
                                            │
               ┌────────────────────────────┼────────────────────────────┐
               │                            │                            │
      ┌────────▼────────┐         ┌─────────▼─────────┐       ┌─────────▼─────────┐
      │ Aieges Shield   │         │ MemQ              │       │ Legion            │
      │ Prompt Guard    │         │ Sovereign Memory  │       │ Swarm Governance  │
      │ PII Detection   │         │ HOT · WARM · COLD │       │ Policy Routing    │
      │ Secret Blocking │         │ MCP-native        │       │ Evidence Capture  │
      └─────────────────┘         └───────────────────┘       └───────────────────┘
               │                            │                            │
               └────────────────────────────┼────────────────────────────┘
                                            │
                              ┌─────────────▼─────────────┐
                              │ Billing Manager            │
                              │ Signup · Stripe · API Keys │
                              │ OAuth · Entitlements       │
                              └────────────────────────────┘
```

**Key design principles:**

- **Sovereign-first** — Everything can run on your infrastructure. No cloud lock-in.
- **Memory-native** — Agents accumulate knowledge across sessions via MemQ's tiered architecture.
- **Multi-model** — Claude, Gemini, GPT, and local models orchestrated through a unified protocol.
- **Proof-backed** — Every claim is backed by benchmarks, telemetry, or audit data.

---

## Quick Links

| Surface | URL |
|---------|-----|
| **Main site** | [multinex.ai](https://multinex.ai) |
| **Sign up / Free trial** | [billing.multinex.ai/signup](https://billing.multinex.ai/signup) |
| **Billing Manager** | [billing.multinex.ai](https://billing.multinex.ai) |
| **MemQ MCP endpoint** | `https://mcp.multinex.ai/mcp/v1` |
| **Status page** | [status.multinex.ai](https://status.multinex.ai) |
| **Marketing platform** | [marketing.multinex.ai](https://marketing.multinex.ai) |

---

## Tech Stack

| Layer | Technology | Purpose |
|-------|-----------|---------|
| **CLI** | Rust (Clap 4) | `munx` command-line interface |
| **Security** | Rust | Aieges Shield firewall proxy and desktop daemon |
| **Runtime** | TypeScript, Deno 2.x | Agent orchestration, sync adapters |
| **Memory** | Qdrant, FalkorDB, Redis | MemQ HOT/WARM/COLD knowledge tiers |
| **Billing** | Next.js, Supabase, Stripe | Billing Manager, OAuth, API keys |
| **Workers** | Cloudflare Workers, AI | Marketing platform, MemQ gateway |
| **Infra** | Docker, Akash, CloudRun | Production deployment surfaces |

---

## Getting Started

### Sign up for the platform

1. Register at **[billing.multinex.ai/signup](https://billing.multinex.ai/signup)** — 14-day free trial, no credit card required.
2. Generate your **MemQ API key** from the Billing Manager dashboard.
3. Connect your MCP client to `https://mcp.multinex.ai/mcp/v1`.

### Install the Aieges Shield

```bash
# Download the latest binary for your platform
curl -sSL https://get.multinex.ai/shield | bash

# Or install via the Billing Manager after checkout
# https://billing.multinex.ai/checkout?product=aieges
```

### Install the Munx CLI

```bash
# Install from source
cargo install --git https://github.com/multinex-ai/multinex munx

# Bootstrap a realm
munx init

# Audit product health
munx product:audit
```

---

## Contributing

We welcome contributions across all public repositories. See each project's `CONTRIBUTING.md` for guidelines.

- **Issues** — Bug reports and feature requests via GitHub Issues
- **PRs** — Fork, branch, PR workflow on all public repos
- **Security** — Report vulnerabilities via GitHub Security Advisories

---

<p align="center">
  <sub>
    <strong>Multinex AI</strong> · The Security, Identity, and Audit Layer for the Agentic Generation<br>
    <a href="https://multinex.ai">multinex.ai</a> · <a href="https://billing.multinex.ai/signup">Sign up</a> · <a href="https://github.com/multinex-ai">GitHub</a> · <a href="https://status.multinex.ai">Status</a>
  </sub>
</p>
