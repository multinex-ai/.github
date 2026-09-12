<p align="center">
  <strong>AI infrastructure that remembers, aligns, and protects.</strong><br>
  <sub>MemQ for shared agent memory. Crosswalk for trusted business meaning. Shield for local AI protection.</sub>
</p>

<p align="center">
  <a href="https://multinex.ai"><img src="https://img.shields.io/badge/site-multinex.ai-D4A843?style=flat-square" alt="Website"></a>
  <a href="https://multinex.ai/docs/"><img src="https://img.shields.io/badge/docs-product_guides-FFC857?style=flat-square" alt="Docs"></a>
  <a href="https://billing.multinex.ai/signup"><img src="https://img.shields.io/badge/start-free_trial-10B981?style=flat-square" alt="Start free"></a>
  <a href="https://status.multinex.ai"><img src="https://img.shields.io/badge/status-operational-0EA5E9?style=flat-square" alt="Status"></a>
  <a href="https://github.com/multinex-ai"><img src="https://img.shields.io/badge/org-multinex--ai-0D1117?style=flat-square&logo=github&logoColor=white" alt="GitHub Org"></a>
</p>

---

## What Multinex Builds

**Multinex AI** builds the operating layer around AI work that cannot afford to lose context, trust the wrong business definition, or leak sensitive data into unmanaged tools.

The current product surface is intentionally focused:

- **MemQ** keeps approved context available across agents, tools, sessions, and teams.
- **Crosswalk** aligns CRM, lakehouse, semantic-layer, and operational definitions before AI acts on them.
- **Shield** classifies and redacts sensitive prompts, files, browser activity, and memory writes before they leave the device.
- **Billing Manager** handles workspace signup, API keys, subscriptions, entitlements, and product access.

---

## Product Surface

<table>
<tr>
<td width="33%">

### [MemQ](https://multinex.ai/memq/)

Shared memory for AI agents.

MemQ is the hosted MCP-native memory layer for AI tools that need durable recall, team handoff, retrieval, and checkpoint continuity.

- Hosted endpoint: `https://mcp.multinex.ai/mcp/v1`
- Works with MCP-compatible clients and agent workflows
- Namespaces, quotas, checkpoints, and governed retrieval
- Public proof: [benchmark harness](https://github.com/multinex-ai/memq-benchmark)

</td>
<td width="33%">

### Crosswalk

Business context alignment before AI acts.

Crosswalk is the product-preview workflow for mapping business definitions across CRM, lakehouse, semantic models, and AI operations.

- Review source fields, owners, grain, and evidence
- Mark definitions as approved, blocked, or needing review
- Preserve approved decisions into MemQ-ready context
- Designed for revenue, data, and operations teams

</td>
<td width="33%">

### [Shield](https://multinex.ai/shield/)

Local AI classifier and prompt guard.

Shield inspects prompts, files, browser activity, and MCP tool calls before sensitive data reaches AI providers or shared memory.

- Local-first inspection and redaction
- Prompt, file, browser, and memory-write protection paths
- Audit posture for regulated workflows
- Public security surface: [aieges-shield](https://github.com/multinex-ai/aieges-shield)

</td>
</tr>
</table>

---

## How The Pieces Fit

```text
          people, teams, IDEs, automations, agents
                         │
                         ▼
       ┌──────────────────────────────────────────┐
       │ Shield                                   │
       │ local classification, redaction, audit   │
       └──────────────────┬───────────────────────┘
                          │ protected prompts, files, tool calls
                          ▼
       ┌──────────────────────────────────────────┐
       │ Crosswalk                                │
       │ reviewed business meaning and evidence   │
       └──────────────────┬───────────────────────┘
                          │ approved context
                          ▼
       ┌──────────────────────────────────────────┐
       │ MemQ                                     │
       │ shared memory, retrieval, checkpoints    │
       └──────────────────┬───────────────────────┘
                          │
                          ▼
       agents resume with the same protected context

       Billing Manager provisions accounts, API keys,
       subscriptions, product access, and entitlements.
```

**Operating principles**

- **Context first** — AI work should resume with the right decisions, not restart from scratch.
- **Meaning before memory** — Business definitions must be reviewed before they become reusable context.
- **Protection at the edge** — Sensitive prompts, files, and memory writes should be screened locally before exposure.
- **Proof over claims** — Benchmarks, docs, and runtime checks matter more than generic AI-platform language.

---

## Developer Entry Points

| Need | Start here |
|------|------------|
| Connect an MCP client to MemQ | [MemQ docs](https://multinex.ai/docs/memq/quickstart/) |
| Install MemQ client/plugin surfaces | [MemQ editor setup](https://multinex.ai/docs/memq/editors/) |
| Review Crosswalk product fit | Product preview; start through [Billing Manager](https://billing.multinex.ai/signup) |
| Review Shield product fit | [Shield product page](https://multinex.ai/shield/) |
| Compare memory behavior | [MemQ benchmark repository](https://github.com/multinex-ai/memq-benchmark) |
| Try a starter project | [memq-mcp-starter](https://github.com/multinex-ai/memq-mcp-starter) |
| Manage account/API keys | [Billing Manager](https://billing.multinex.ai) |

---

## Public Repositories

| Repository | Purpose |
|------------|---------|
| [memq-connect](https://github.com/multinex-ai/memq-connect) | MCP registry manifest and client setup assets for MemQ |
| [memq-mcp](https://github.com/multinex-ai/memq-mcp) | Public MCP-facing MemQ package surface |
| [memq-benchmark](https://github.com/multinex-ai/memq-benchmark) | Reproducible memory and retrieval benchmark proof |
| [memq-mcp-starter](https://github.com/multinex-ai/memq-mcp-starter) | Minimal MCP starter for MemQ-backed agents |
| [memq-cursor-claude-starter](https://github.com/multinex-ai/memq-cursor-claude-starter) | Starter workflow for Cursor and Claude-style agent memory |
| [memq-team-handoff-starter](https://github.com/multinex-ai/memq-team-handoff-starter) | Team handoff pattern using shared agent memory |
| [memq-n8n-agent-starter](https://github.com/multinex-ai/memq-n8n-agent-starter) | n8n automation starter with MemQ continuity |
| [aieges-shield](https://github.com/multinex-ai/aieges-shield) | Public Shield security gateway and AI firewall surface |
| [multinex-skills](https://github.com/multinex-ai/multinex-skills) | Skills for MemQ memory, Shield protection, and workflow guidance |

---

## Getting Started

1. Create a workspace at [billing.multinex.ai/signup](https://billing.multinex.ai/signup).
2. Generate a MemQ API key in Billing Manager.
3. Connect your MCP client to `https://mcp.multinex.ai/mcp/v1`.
4. Use Crosswalk when AI depends on business definitions that need review.
5. Add [Shield](https://multinex.ai/shield/) when prompts, files, tool calls, or memory writes may contain sensitive data.

---

## Links

| Surface | URL |
|---------|-----|
| Main site | [multinex.ai](https://multinex.ai) |
| Docs | [multinex.ai/docs](https://multinex.ai/docs/) |
| MemQ | [multinex.ai/memq](https://multinex.ai/memq/) |
| Crosswalk | Product preview |
| Shield | [multinex.ai/shield](https://multinex.ai/shield/) |
| Billing Manager | [billing.multinex.ai](https://billing.multinex.ai) |
| Status | [status.multinex.ai](https://status.multinex.ai) |

---

<p align="center">
  <sub>
    <strong>Multinex AI</strong> · AI infrastructure that remembers, aligns, and protects<br>
    <a href="https://multinex.ai">multinex.ai</a> ·
    <a href="https://multinex.ai/docs/">Docs</a> ·
    <a href="https://billing.multinex.ai/signup">Start free</a> ·
    <a href="https://status.multinex.ai">Status</a>
  </sub>
</p>
