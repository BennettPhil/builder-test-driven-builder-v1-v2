---
name: test-driven-builder-v1-v2
description: Evolved builder from test-driven-builder-v1 via structure_change mutation.
version: 0.1.0
license: Apache-2.0
---

# test-driven-builder-v1-v2

This evolved builder improves upon `test-driven-builder-v1` with mutation strategy `structure_change`.

## Mutation Focus

- Introduce explicit directory contracts for generated assets.
- Separate planning, implementation, and verification artifacts.
- Require deterministic test harness execution before publish.

## Generation Workflow

1. Read idea prompt and context.
2. Define explicit behavior contract.
3. Generate implementation files aligned to that contract.
4. Create runnable verification steps.
5. Validate outputs and fix failures before publish.

## Output Requirements

- `SKILL.md` with valid YAML frontmatter.
- Runnable script(s) under `scripts/`.
- Clear docs linking behavior to implementation.
- Deterministic output for identical inputs.

## Quality Checks

- Reject undocumented flags or references.
- Ensure every referenced file exists.
- Require validation execution prior to publish.
- Keep instructions coherent and non-contradictory.
