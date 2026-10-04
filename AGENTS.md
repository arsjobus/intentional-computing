# Intentional Computing — AI Development Instructions

## Primary Instruction

Before making any change in this repository, read:

`QUICK_RULES.md`

This is the primary engineering contract for the Intentional Computing project.

## Context Loading Policy

Use `QUICK_RULES.md` as the default and sufficient Intentional Computing context for normal development tasks.

Do **not** automatically load:

* `MANIFESTO.md`
* `PRINCIPLES.md`
* `DESIGN.md`
* files under `philosophy/`
* files under `standards/`

unless the task specifically requires them.

Load additional documentation only when:

1. The user explicitly asks for it.
2. The task concerns a principle not adequately covered by `QUICK_RULES.md`.
3. The task requires modifying the relevant documentation itself.
4. A project-specific specification explicitly references additional Intentional Computing documentation.

## Priority

When making implementation decisions, use this priority:

1. User's explicit request
2. Project-specific requirements
3. `QUICK_RULES.md`
4. Relevant detailed Intentional Computing documentation
5. General engineering judgment

Do not invent additional Intentional Computing requirements that are not supported by these sources.

## Development Behavior

Before implementing a meaningful change:

1. Understand the requested behavior.
2. Check it against `QUICK_RULES.md`.
3. Implement the smallest appropriate solution.
4. Test the result.
5. Check user control, attention cost, ownership, reversibility, and failure behavior.
6. Document the change when appropriate.

## Keep Context Small

Do not read large portions of the repository unnecessarily.

Prefer targeted retrieval of the smallest relevant file or section.

The purpose of this instruction is to keep AI context efficient while preserving the project's core principles.

## Core Rule

`QUICK_RULES.md` is the default Intentional Computing context.

When in doubt, start there.
