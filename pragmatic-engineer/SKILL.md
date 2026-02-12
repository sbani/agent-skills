---
name: pragmatic-engineer
description: Guides code and design toward simplicity, clarity, and incremental delivery. Use when writing or reviewing code, designing APIs, or when the user asks for pragmatic engineering advice, simple design, or references Go proverbs and XP/simple-design quotes.
---

# Pragmatic Engineer

Apply pragmatic engineering principles: favor the simplest thing that works,
clear over clever, and incremental improvement over big design upfront.

## Core quotes

- **Do the simplest thing that could possibly work.** (eXtreme Programming)
- **Make it work, make it good, make it fast.** — Kent Beck (do them in that
  order; avoid optimizing before it works and is good.)

## Coding Proverbs

Follow these when writing code and as general design guidance where they apply:

1. A little copying is better than a little dependency.
1. Clear is better than clever.
1. Don't communicate by sharing memory, share memory by communicating.
1. Concurrency is not parallelism.
1. Channels orchestrate; mutexes serialize.
1. The bigger the interface, the weaker the abstraction.
1. Reflection is never clear.
1. Don't just check errors, handle them gracefully.
1. Design the architecture, name the components, document the details.
1. Documentation is for users.

Source: [Go Proverbs](https://go-proverbs.github.io/) from Rob Pike, Gopherfest
SV 2015

---

## Instructions for the agent

When this skill is active:

1. Prefer the simplest implementation that could possibly work; avoid
   speculative complexity.
1. Apply "make it work, make it good, make it fast" — get correctness and
   clarity before optimizing.
1. Follow the coding proverbs above.
1. Prefer clear over clever; small interfaces over large ones; a little copying
   over unnecessary dependencies.
1. Suggest incremental, shippable steps rather than large rewrites when both are
   feasible.

## Principles

- **YAGNI** — You Aren't Gonna Need It. Don't add code for hypothetical future
  requirements.
- **KISS** — Keep It Simple, Stupid. Simplicity is a feature.
- **Naming** — Names should make behavior and intent obvious; rename when
  clarity improves.
- **Tests** — Prefer tests that lock in behavior and allow safe refactors; avoid
  testing implementation details.
- **APIs** — Design for the caller: small, focused surfaces; clear contracts;
  good defaults.
- **Refactoring** — Improve structure in small steps while keeping tests green;
  don't mix big refactors with new behavior in one change.
