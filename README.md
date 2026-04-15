<p align="center">
  <h1 align="center">Claude Code Game Studios (Enhanced)</h1>
  <p align="center">
    Turn a single Claude Code session into a full game development studio.<br />
    49 agents. 81 skills. 12 hooks. Token-optimized.
  </p>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License"></a>
  <a href=".claude/agents"><img src="https://img.shields.io/badge/agents-49-blueviolet" alt="49 Agents"></a>
  <a href=".claude/skills"><img src="https://img.shields.io/badge/skills-81-green" alt="81 Skills"></a>
  <a href=".claude/hooks"><img src="https://img.shields.io/badge/hooks-12-orange" alt="12 Hooks"></a>
  <a href=".claude/rules"><img src="https://img.shields.io/badge/rules-11-red" alt="11 Rules"></a>
  <a href="https://docs.anthropic.com/en/docs/claude-code"><img src="https://img.shields.io/badge/built%20for-Claude%20Code-f5f5f5?logo=anthropic" alt="Built for Claude Code"></a>
</p>

---

## What Is This?

An enhanced fork of [Claude Code Game Studios](https://github.com/Donchitos/Claude-Code-Game-Studios) with **9 additional skills** focused on token optimization, systematic development methodology, and creative tooling.

The base framework gives you a full AI game studio with 49 specialized agents, organized into a real studio hierarchy (directors, leads, specialists). This fork adds skills cherry-picked from the best Claude Code community projects to reduce costs and improve development quality.

---

## What's Added (9 Extra Skills)

### Token Optimization (from [everything-claude-code](https://github.com/affaan-m/everything-claude-code))

| Skill | Purpose |
|-------|---------|
| `cost-aware-llm-pipeline` | Model routing by task complexity (Haiku for simple, Sonnet for standard, Opus for architecture) |
| `context-budget` | Audit context window consumption, detect bloat, get prioritized savings recommendations |
| `content-hash-cache-pattern` | SHA-256 content hash caching to avoid redundant file processing |

### Development Methodology (from [superpowers](https://github.com/obra/superpowers))

| Skill | Purpose |
|-------|---------|
| `verification-before-completion` | No "done" claims without evidence — run verification, read output, then report |
| `systematic-debugging` | 4-phase root cause methodology instead of guess-and-check |
| `subagent-driven-development` | Model-tiered subagent dispatch with review cycles |

### Creative & Research (from [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) & [Anthropic](https://github.com/anthropics/claude-code))

| Skill | Purpose |
|-------|---------|
| `frontend-design` | Production-grade UI design (Anthropic official) — bold aesthetics, no AI slop |
| `artifacts-builder` | React 18 + Tailwind + shadcn/ui single-file HTML artifact builder |
| `deep-research` | Multi-step research with citations |

---

## What's Included (Base Framework)

| Category | Count | Description |
|----------|-------|-------------|
| **Agents** | 49 | Specialized subagents across design, programming, art, audio, narrative, QA, and production |
| **Skills** | 72 + 9 | Base slash commands + token optimization and methodology skills |
| **Hooks** | 12 | Automated validation on commits, pushes, assets, session lifecycle, agent audit trail |
| **Rules** | 11 | Path-scoped coding standards for gameplay, engine, AI, UI, network code |
| **Templates** | 39 | Document templates for GDDs, UX specs, ADRs, sprint plans, and more |

## Studio Hierarchy

```
Tier 1 — Directors (Opus)
  creative-director    technical-director    producer

Tier 2 — Department Leads (Sonnet)
  game-designer        lead-programmer       art-director
  audio-director       narrative-director    qa-lead
  release-manager      localization-lead

Tier 3 — Specialists (Sonnet/Haiku)
  gameplay-programmer  engine-programmer     ai-programmer
  network-programmer   tools-programmer      ui-programmer
  systems-designer     level-designer        economy-designer
  technical-artist     sound-designer        writer
  world-builder        ux-designer           prototyper
  performance-analyst  devops-engineer       analytics-engineer
  security-engineer    qa-tester             accessibility-specialist
  live-ops-designer    community-manager
```

### Engine Specialists

| Engine | Lead Agent | Sub-Specialists |
|--------|-----------|-----------------|
| **Godot 4** | `godot-specialist` | GDScript, Shaders, GDExtension, C# |
| **Unity** | `unity-specialist` | DOTS/ECS, Shaders/VFX, Addressables, UI Toolkit |
| **Unreal Engine 5** | `unreal-specialist` | GAS, Blueprints, Replication, UMG/CommonUI |

---

## Getting Started

### Prerequisites

- [Git](https://git-scm.com/)
- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) (`npm install -g @anthropic-ai/claude-code`)

### Setup

1. **Clone**:
   ```bash
   git clone https://github.com/batoner/Claude-Code-Game-Studios.git my-game
   cd my-game
   ```

2. **Open Claude Code**:
   ```bash
   claude
   ```

3. **Run `/start`** — guided onboarding that detects where you are and leads you forward.

---

## Attribution

This project is built on the work of these open-source projects:

| Project | Author | License | What We Used |
|---------|--------|---------|-------------|
| [Claude Code Game Studios](https://github.com/Donchitos/Claude-Code-Game-Studios) | Donchitos | MIT | Base framework (49 agents, 72 skills, 12 hooks, 11 rules, 39 templates) |
| [superpowers](https://github.com/obra/superpowers) | Jesse Vincent | MIT | verification-before-completion, systematic-debugging, subagent-driven-development |
| [everything-claude-code](https://github.com/affaan-m/everything-claude-code) | affaan-m | MIT | cost-aware-llm-pipeline, context-budget, content-hash-cache-pattern |
| [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) | ComposioHQ | Apache 2.0 | artifacts-builder, deep-research |
| [claude-code (frontend-design)](https://github.com/anthropics/claude-code) | Anthropic | Apache 2.0 | frontend-design skill |

---

## License

MIT License. See [LICENSE](LICENSE) for details.

Original framework by [Donchitos](https://github.com/Donchitos). Enhanced by [batoner](https://github.com/batoner).
