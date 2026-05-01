[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# open-memory

**The Global Marketplace for AI Agent Context.** A centralized, public registry of Agent Skills, Workflows, Rules, and Templates for the RND-PRO ecosystem — anyone can contribute universal skills here. Install them via the Agent Portal → sync to your private Team Memory → **empower your AI agents**.

```
┌─────────────────────────────────┐
│  IDE Agent                      │  ← Claude, GPT, Gemini, etc.
│  (Antigravity / Cursor / ...)   │
└────────────┬────────────────────┘
             │ MCP (stdio)
┌────────────▼────────────────────┐
│  mcp-agent-portal               │
│  (MCP aggregator + web UI)      │
└──┬──────────────────────────────┘
   │ Context Layer Synchronization
┌──▼──────────────────────────────┐
│  context-x-mcp                  │  ← The Memory Engine
└──┬────────────────────┬─────────┘
   │ Sync               │ Sync
   ▼                    ▼
[open-memory]        [team-memory]
Layer 1 (Public)     Layer 2 (Private)
```

> [!TIP]
> Agents can dynamically discover and "install" universal skills from `open-memory` directly into a project's `.agents/skills` folder.

### The 3-Tier Context Architecture

The RND-PRO ecosystem isolates context into three distinct layers to prevent token bloat and maintain strict security boundaries:

1. **Layer 1: Open Memory** (This repository) — Global marketplace of public, reusable skills.
2. **Layer 2: Team Memory** (`rnd-pro/team-memory`) — Private team rules and internal knowledge.
3. **Layer 3: Local Context** (`.ctx` files via `project-graph-mcp`) — AST-based codebase structural knowledge.

## Features

- **Standardized Skills** — Universal agent patterns (e.g., *React component generation*, *Docker optimization*).
- **Abbreviated Dialect** — All rules are written in a token-optimized, pseudo-code format to maximize LLM context windows.
- **Workflow Automation** — Complex CI/CD, testing, and deployment sequences formatted for autonomous execution.
- **Cross-Platform** — Usable by any MCP-compatible agent or orchestrator.

## Directory Structure

- `rules/` — Global behavioral standards for agents.
- `skills/` — Actionable, universal agent skills.
- `workflows/` — Multi-step sequences and pipelines.
- `templates/` — Standard code templates.
- `configs/` — Public configurations.

> [!IMPORTANT]
> When contributing to Open Memory, you **must** adhere to the **Abbreviated English Dialect**. Do not use conversational sentences. Write instructions as logical flows (`1file+no_risk -> P2`).

## MCP Ecosystem

Best used as part of [**mcp-agent-portal**](https://github.com/rnd-pro/mcp-agent-portal) — a unified MCP aggregator that bundles agent-pool, project-graph, and context-x behind a single config entry.

## Related Projects
- [mcp-agent-portal](https://github.com/rnd-pro/mcp-agent-portal) — Unified MCP aggregator + web dashboard + AI agent runtime
- [agent-pool-mcp](https://github.com/nicholasgriffintn/agent-pool-mcp) — Multi-agent orchestration via parallel workers
- [project-graph-mcp](https://github.com/rnd-pro/project-graph-mcp) — AST-based codebase analysis for AI agents
- [Symbiote.js](https://github.com/symbiotejs/symbiote.js) — Isomorphic Reactive Web Components framework

## License

MIT © [RND-PRO.com](https://rnd-pro.com)

---

**Made with ❤️ by the RND-PRO team**
