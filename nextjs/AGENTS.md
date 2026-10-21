# AGENTS.md
Instructions for AI coding agents (Codex, Claude Code, Cursor, Copilot, Aider...) working in this repository.
Stack: Next.js app (App Router, pnpm, Playwright). Replace the <placeholders>.

## Project overview
<One paragraph: what this project does, who uses it, main entry point.>

## Setup and commands
- Install: `pnpm install`
- Test: `pnpm test && pnpm exec playwright test`  (must pass before every commit)
- Lint / format: `pnpm lint && pnpm typecheck`

## Layout
- Source: `app/ (routes), components/, lib/`
- Tests: unit tests with vitest, e2e in e2e/ with Playwright

## Conventions
- Style: Server Components by default; add 'use client' only when needed
- Commits: imperative mood, first line <= 72 chars.
- Never commit `.env*`; new env vars must be added to `.env.example`.
- Do not add a dependency without explaining why in the PR description.

## Boundaries
- Never commit secrets, tokens or `.env` files.
- Ask a human before: public API changes, database migrations, deleting files, CI changes.
- Keep changes small and focused; add or update tests with every behaviour change.

## Definition of done
- [ ] tests pass  - [ ] lint passes  - [ ] docs/README updated if behaviour changed  - [ ] no unrelated edits
