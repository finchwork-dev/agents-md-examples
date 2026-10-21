# AGENTS.md
Instructions for AI coding agents (Codex, Claude Code, Cursor, Copilot, Aider...) working in this repository.
Stack: TypeScript / Node.js (pnpm, vitest, eslint). Replace the <placeholders>.

## Project overview
<One paragraph: what this project does, who uses it, main entry point.>

## Setup and commands
- Install: `pnpm install`
- Test: `pnpm test`  (must pass before every commit)
- Lint / format: `pnpm lint && pnpm typecheck`

## Layout
- Source: `src/`
- Tests: *.test.ts next to the file under test; vitest

## Conventions
- Style: Prettier defaults, strict TS, no `any` without a comment
- Commits: imperative mood, first line <= 72 chars.
- Never edit `dist/` or `pnpm-lock.yaml` by hand.
- Do not add a dependency without explaining why in the PR description.

## Boundaries
- Never commit secrets, tokens or `.env` files.
- Ask a human before: public API changes, database migrations, deleting files, CI changes.
- Keep changes small and focused; add or update tests with every behaviour change.

## Definition of done
- [ ] tests pass  - [ ] lint passes  - [ ] docs/README updated if behaviour changed  - [ ] no unrelated edits
