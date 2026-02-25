<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/multinex-ai/.github/main/assets/banner.jpg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/multinex-ai/.github/main/assets/banner.jpg">
    <img alt="Multinex AI" src="https://raw.githubusercontent.com/multinex-ai/.github/main/assets/banner.jpg" width="100%">
  </picture>
</p>

<p align="center">
  <strong>Federated intelligence infrastructure for sovereign AI systems.</strong><br>
  <sub>Open-source runtime, security tooling, and multi-agent orchestration.</sub>
</p>

<p align="center">
  <a href="https://github.com/multinex-ai"><img src="https://img.shields.io/badge/org-Multinex--AI-0D1117?style=flat-square&logo=github&logoColor=white" alt="GitHub Org"></a>
  <a href="https://github.com/multinex-ai?tab=repositories&q=&type=public"><img src="https://img.shields.io/badge/public_repos-2-00D4FF?style=flat-square" alt="Public Repos"></a>
  <a href="https://github.com/multinex-ai/omnipotent-commons/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-D4A843?style=flat-square" alt="License"></a>
  <img src="https://img.shields.io/badge/rust-%23000000.svg?style=flat-square&logo=rust&logoColor=white" alt="Rust">
  <img src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/deno-000000?style=flat-square&logo=deno&logoColor=white" alt="Deno">
</p>

---

## About

**Multinex AI** builds federated AI infrastructure — systems where agents operate with persistent memory, multi-model orchestration, and sovereign data ownership. Our stack is designed for teams that need AI tooling they fully control: no cloud lock-in, no black-box APIs, no data leaving your perimeter.

We maintain the **OAR** (Omnipotent Agentic Runtime) platform and a growing ecosystem of open-source security and orchestration tools.

---

## Open Source Projects

<table>
<tr>
<td width="50%">

### [Aegis](https://github.com/multinex-ai/aegis)

AI security firewall proxy — local, fast, no cloud.

![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=flat-square&logo=rust&logoColor=white)
![License](https://img.shields.io/github/license/multinex-ai/aegis?style=flat-square&color=D4A843)
![GitHub stars](https://img.shields.io/github/stars/multinex-ai/aegis?style=flat-square&color=00D4FF)

- Rules-based prompt injection detection
- PII leakage prevention
- Credential exposure blocking
- Zero external dependencies

</td>
<td width="50%">

### [OAR Commons](https://github.com/multinex-ai/omnipotent-commons)

Alliance template for shared plans, task boards, and collaboration.

![Shell](https://img.shields.io/badge/shell-%23121011.svg?style=flat-square&logo=gnu-bash&logoColor=white)
![GitHub stars](https://img.shields.io/github/stars/multinex-ai/omnipotent-commons?style=flat-square&color=00D4FF)

- Git-native markdown task boards
- PM tool sync (Linear, GitHub, Jira)
- Multi-agent config generation
- Alliance bootstrap workflow

</td>
</tr>
</table>

---

## Platform Architecture

```
                        ┌─────────────────────────────────────┐
                        │        OAR — Agentic Runtime        │
                        │   Multi-model  ·  Persistent memory │
                        │   Sovereign    ·  Federated         │
                        └──────────────────┬──────────────────┘
                                           │
              ┌────────────────────────────┼────────────────────────────┐
              │                            │                            │
     ┌────────▼────────┐         ┌─────────▼─────────┐       ┌─────────▼─────────┐
     │   Aegis          │         │   Airlock          │       │   Mnemosyne       │
     │   AI Firewall    │         │   Org Isolation    │       │   Memory Tiers    │
     │   Prompt Guard   │         │   Task Board Sync  │       │   Redis · Qdrant  │
     │   PII Detection  │         │   Alliance Mgmt    │       │   Graphiti · KG   │
     └──────────────────┘         └────────────────────┘       └───────────────────┘
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
| **CLI** | Rust (Clap 4) | `oar` command-line interface |
| **Runtime** | TypeScript, Deno | Agent orchestration, sync adapters |
| **Security** | Rust | Aegis firewall proxy |
| **Memory** | Redis, Qdrant, FalkorDB | Hot/warm/cold knowledge tiers |
| **Infra** | Docker Compose | Sovereign deployment stack |

---

## Getting Started

```bash
# Install the OAR CLI
cargo install --git https://github.com/multinex-ai/omnipotent oar

# Initialize a sector
oar init

# Boot the sovereign stack
oar up

# Connect to a realm
oar connect
```

---

## Contributing

We welcome contributions across all public repositories. See each project's `CONTRIBUTING.md` for guidelines.

- **Issues** — Bug reports and feature requests via GitHub Issues
- **PRs** — Fork, branch, PR workflow on all public repos
- **Security** — Report vulnerabilities via [GitHub Security Advisories](https://github.com/multinex-ai/aegis/security)

---

<p align="center">
  <sub>
    <strong>Multinex AI</strong> · Federated Intelligence Infrastructure<br>
    <a href="https://github.com/multinex-ai">GitHub</a>
  </sub>
</p>
