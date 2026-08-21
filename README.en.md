# Six Strategies (LT)

[中文](./README.md)

Six Strategies is a software-engineering collaboration protocol for Codex. It turns complex build, repair, refactoring, and long-term maintenance work into an execution loop that is traceable, verifiable, and recoverable.

It is not a framework or a standalone prompt. It is a lightweight set of working constraints: freeze the goal and boundaries first, select architecture gates, implementation batches, verification, and audit depth according to risk, then leave precise project memory so future changes only need the relevant context.

## What it solves

Large software tasks usually become difficult when requirements, architecture, implementation, tests, and history drift apart. Six Strategies connects them with stable identifiers and explicit gates:

- `R-` records observable requirements and acceptance criteria.
- `A-` records architecture, boundaries, invariants, and key trade-offs.
- `F-` divides work into implementation batches with clear file ownership.
- `T-` fixes the tests, commands, and reviewable evidence.
- Dedicated gates cover foundational architecture, public contracts, permissions, migrations, IPC, plugins, build, and release infrastructure.
- Major changes leave an integration-level log for incremental maintenance by feature, path, or contract.

## Core workflow

```text
Freeze goals → assess impact → choose minimal architecture → batch implementation
    → verify immediately → update project memory → unified audit → delivery log
```

Six Strategies follows a minimum-sufficient principle: reuse existing code, the standard library, and installed capabilities first. Add modules, interfaces, dependencies, or abstractions only when the actual task requires them. A local change is not automatically expanded into an unrelated architectural rewrite.

## SOL / Luna collaboration

- **SOL** handles unfrozen critical architecture, public contracts, indivisible critical implementation, and independent final audits.
- **Luna** handles fact collection, bounded implementation with frozen decisions, precise verification, and mechanical logging.

Luna writes only after the fact scope, product behavior, trust boundaries, state transitions, write set, and verification commands are explicit. Unresolved product or architecture choices are not delegated to a bounded implementation batch.

## Installation

Download the complete skill package from the [Release asset](https://github.com/Taian1738/six-strategies/releases/download/v2026.08.21/ltskill-20260821-142646.zip), extract it into the Codex skills directory, and preserve this structure:

```text
<CODEX_HOME>/skills/ltskill/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── audit-routing.md
    ├── change-log.md
    ├── dispatch-contracts.md
    ├── foundation-gate.md
    ├── project-memory.md
    └── sol-cost-controls.md
```

After installation, invoke it explicitly with `$ltskill`.

You can also browse [SKILL.md](./SKILL.md), [agent configuration](./agents/openai.yaml), and the [references](./references/) directory directly in the repository.

## Version

- Protocol: `LT-2026-08-21.11`
- Release: [v2026.08.21](https://github.com/Taian1738/six-strategies/releases/tag/v2026.08.21)
- Direct download: [ltskill-20260821-142646.zip](https://github.com/Taian1738/six-strategies/releases/download/v2026.08.21/ltskill-20260821-142646.zip)
- SHA-256: `20829445328F11803C781BC56C427D0E4DF284DB39939F552CA1816EF0844393`

## Scope

Six Strategies governs how software work is organized, routed, verified, and maintained. It does not replace a project's own requirements, tests, permission policies, or release approvals. Installing dependencies, publishing artifacts, changing production environments, and other external state changes still require explicit authorization and project-specific rules.

