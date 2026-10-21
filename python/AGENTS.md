# AGENTS.md
Instructions for AI coding agents (Codex, Claude Code, Cursor, Copilot, Aider...) working in this repository.
Stack: Python (uv/pip, pytest, ruff). Replace the <placeholders>.

## Project overview
<One paragraph: what this project does, who uses it, main entry point.>

## Setup and commands
- Install: `pip install -e '.[dev]'  # or: uv sync`
- Test: `pytest -q`  (must pass before every commit)
- Lint / format: `ruff check . && ruff format --check .`

## Layout
- Source: `src/<pkg>/`
- Tests: tests/ mirrors src/ paths; use pytest fixtures, no network in unit tests

## Conventions
- Style: ruff format, line length 88, type hints on public functions
- Commits: imperative mood, first line <= 72 chars.
- Do not edit `uv.lock`/`requirements*.txt` by hand; regenerate.
- Do not add a dependency without explaining why in the PR description.

## Boundaries
- Never commit secrets, tokens or `.env` files.
- Ask a human before: public API changes, database migrations, deleting files, CI changes.
- Keep changes small and focused; add or update tests with every behaviour change.

## Definition of done
- [ ] tests pass  - [ ] lint passes  - [ ] docs/README updated if behaviour changed  - [ ] no unrelated edits
