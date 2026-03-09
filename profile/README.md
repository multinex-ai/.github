<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/multinex-ai/.github/main/assets/banner.jpg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/multinex-ai/.github/main/assets/banner.jpg">
    <img alt="Multinex" src="https://raw.githubusercontent.com/multinex-ai/.github/main/assets/banner.jpg" width="100%">
  </picture>
</p>

<p align="center">
  <strong>The Autonomous Operating System for the Sovereign Enterprise.</strong><br>
  <sub>Open-source runtime, security tooling, and multi-agent orchestration.</sub>
</p>

<p align="center">
  <a href="https://github.com/multinex-ai"><img src="https://img.shields.io/badge/org-Multinex-0D1117?style=flat-square&logo=github&logoColor=white" alt="GitHub Org"></a>
  <a href="https://github.com/multinex-ai?tab=repositories&q=&type=public"><img src="https://img.shields.io/badge/public_repos-2-00D4FF?style=flat-square" alt="Public Repos"></a>
  <a href="https://github.com/multinex-ai/omnipotent-commons/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-D4A843?style=flat-square" alt="License"></a>
  <img src="https://img.shields.io/badge/rust-%23000000.svg?style=flat-square&logo=rust&logoColor=white" alt="Rust">
  <img src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/deno-000000?style=flat-square&logo=deno&logoColor=white" alt="Deno">
</p>

---

## About

**Multinex AI** provides the complete infrastructure stack for enterprises to deploy, govern, and scale autonomous AI agents — on their own hardware, with their own data, under their own rules. 

We build the **Autonomous Operating System for the Sovereign Enterprise**. Our systems are designed for teams that need AI tooling they fully control: no cloud lock-in, no black-box APIs, and absolute data sovereignty.

We maintain the **MARS** (Multi-Agent Runtime System) platform and a growing ecosystem of open-source security, orchestration, and compliance tools.

---

## Products & Ecosystem

<table>
<tr>
<td width="50%">

### [Munx Aieges Shield](https://github.com/multinex-ai/munx-aieges-shield)

AI security firewall proxy — local, fast, no cloud.

![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=flat-square&logo=rust&logoColor=white)

- Rules-based prompt injection detection
- PII leakage prevention
- Credential exposure blocking
- Zero external dependencies

</td>
<td width="50%">

### [Munx Airlock Visa](https://github.com/multinex-ai/munx-airlock-visa)

Federated Sync and Alliance Management protocol.

![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white)

- Git-native markdown task boards
- PM tool sync (Linear, GitHub, Jira)
- Org Isolation & multi-agent config generation
- Alliance bootstrap workflow

</td>
</tr>
</table>

---

## Platform Architecture

```text
                        ┌─────────────────────────────────────┐
                        │        MARS — Agentic Runtime       │
                        │   Multi-model  ·  Persistent memory │
                        │   Sovereign    ·  Federated         │
                        └──────────────────┬──────────────────┘
                                           │
              ┌────────────────────────────┼────────────────────────────┐
              │                            │                            │
     ┌────────▼────────┐         ┌─────────▼─────────┐       ┌─────────▼─────────┐
     │ Munx Aieges     │         │ Munx Airlock Visa │       │ Munx MemoryStack  │
     │ Shield          │         │ Org Isolation     │       │ Memory Tiers      │
     │ Prompt Guard    │         │ Task Board Sync   │       │ Redis · Qdrant    │
     │ PII Detection   │         │ Alliance Mgmt     │       │ Graphiti · KG     │
     └─────────────────┘         └───────────────────┘       └───────────────────┘
```

**Key design principles:**

- **Sovereign-first** — Everything runs on your infrastructure. No cloud dependency.
- **Federated** — Teams share plans through Alliances without merging codebases.
- **Memory-native** — Agents accumulate knowledge across sessions via a 4-tier memory architecture.
- **Multi-model** — Claude, Gemini, GPT, and local models orchestrated through a unified protocol.

---

## Tech Stack

| Layer | Technology | Purpose |
|-------|-----------|---------|
| **CLI** | Rust (Clap 4) | `munx` command-line interface |
| **Runtime** | TypeScript, Deno | Agent orchestration, sync adapters |
| **Security** | Rust | Aieges Shield firewall proxy |
| **Memory** | Redis, Qdrant, FalkorDB | Hot/warm/cold knowledge tiers |
| **Infra** | Docker Compose | Sovereign deployment stack |

---

## Getting Started

```bash
# Install the MUNX CLI
cargo install --git https://github.com/multinex-ai/munxclaw munx

# Initialize a sector
munx init

# Boot the sovereign stack
munx up

# Connect to a realm
munx connect
```

---

## Contributing

We welcome contributions across all public repositories. See each project's `CONTRIBUTING.md` for guidelines.

- **Issues** — Bug reports and feature requests via GitHub Issues
- **PRs** — Fork, branch, PR workflow on all public repos
- **Security** — Report vulnerabilities via GitHub Security Advisories on the respective repositories.

---

<p align="center">
  <sub>
    <strong>Multinex AI</strong> · The Autonomous Operating System for the Sovereign Enterprise<br>
    <a href="https://github.com/multinex-ai">GitHub</a>
  </sub>
</p>
