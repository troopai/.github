<div align="center">

<picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/troopai/.github/main/profile/troopai-logo-light.svg#gh-dark-mode-only">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/troopai/.github/main/profile/troopai-logo-dark.svg#gh-light-mode-only">
    <img alt="TroopAI Logo" src="https://raw.githubusercontent.com/troopai/.github/main/profile/troopai-logo-dark.svg" width="50%">
</picture>

# TroopAI

**Where language becomes action.**

An open-source **Agent Development Kit (ADK)** and its ecosystem —
built for engineers who want to *measure* their agents, not just demo them.

</div>

---

## The concept

An LLM produces language. An **agent** is what happens when language becomes
action: tool calls, state transitions, side effects in the real world.

A **troop** is what happens when agents stop acting alone — a coordinated unit
of specialized agents, moving in formation toward a single objective.

TroopAI is the development kit for building exactly that:

- **Code-first.** Agents, tools, and orchestration are plain Python —
  no YAML-defined "personalities," no prompt-soup DSLs.
- **Type-safe by construction.** Pydantic models at every boundary:
  agent inputs, tool schemas, inter-agent messages, run results.
  If it doesn't type-check, it doesn't ship.
- **Evals are a first-class citizen, not an afterthought.**
  A framework claim you can't benchmark is marketing.
  TroopAI ships its own evaluation harness and publishes its scores
  against other frameworks — including the uncomfortable results.
- **Production-shaped.** The cookbook isn't toy notebooks.
  It's advanced, end-to-end, deployable examples that use the ADK
  the way real systems do.

## Repositories

| Repository | What it is | Status |
|---|---|---|
| **[troopai-adk-python](https://github.com/troopai/troopai-adk-python)** | The core Agent Development Kit — agent abstractions, tool interface, orchestration runtime | 🚧 In development |
| **[troopai-evals-python](https://github.com/troopai/troopai-evals-python)** | The evaluation harness — benchmarks `troopai-adk-python` against other frameworks (crewai, openai-agents, …) on identical tasks, with reproducible scoring | 🚧 In development |
| **[troopai-cookbook-python](https://github.com/troopai/troopai-cookbook-python)** | Advanced and production-ready examples built on the ADK — real architectures, not hello-worlds | 🚧 In development |

> The three repositories form one loop: **build** with the ADK,
> **prove** it with the evals, **learn** it from the cookbook.

## Design tenets

1. **Explicit over magical.** Orchestration you can read, debug, and
   step through in a debugger beats orchestration hidden in a decorator.
2. **One obvious way.** The ADK has opinions. Fewer knobs, sharper edges.
3. **Everything is inspectable.** Every run emits structured traces —
   agent decisions, tool I/O, token costs — because you can't optimize
   what you can't see.
4. **Benchmarks or it didn't happen.** Performance and quality claims
   come with eval suite links, or they don't get made.

## Getting started

```bash
pip install troopai-adk-python
```

Until the first release, watch the repositories above — the ADK lands first,
the evals and cookbook follow close behind.

## Roadmap

- [ ] `troopai-adk-python` — core agent, tool, and orchestration primitives
- [ ] `troopai-evals-python` — first published benchmark vs. other frameworks
- [ ] `troopai-cookbook-python` — first production-grade example
