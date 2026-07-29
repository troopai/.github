# Contributing to TroopAI

> This is the **organization-wide default** contributing guide.
> A repository with its own `CONTRIBUTING.md` overrides this one.

Thanks for your interest in contributing. TroopAI is early —
which means contributions have outsized influence right now.

## Ground rules

1. **Code-first, type-safe.** All public APIs are fully type-annotated,
   with Pydantic models at every boundary. PRs that introduce untyped
   surfaces will be asked to add types.
2. **An eval beats an argument.** Performance or quality claims in a PR
   description should be backed by a benchmark run, not adjectives.
3. **Explicit over magical.** If a reviewer can't trace the execution
   path by reading the code, the abstraction is too clever. Simplify it.

## How to contribute

- **Bug reports** — open an issue in the relevant repository
  (`troopai-adk-python`, `troopai-evals-python`, or `troopai-cookbook-python`)
  with a minimal reproduction.
- **Discussions / design proposals** — open a discussion before writing
  large amounts of code. An hour of design talk saves a week of rewrite.
- **Pull requests** — keep them small and single-purpose.
  Include tests; include eval results when behavior changes.
- **Credit** — every contribution earns attribution. Add your name to
  the `AUTHORS` file with your first merged PR. Contributors are
  protected by the same NOTICE attribution requirement as the creator:
  anyone redistributing TroopAI code must preserve all credits.