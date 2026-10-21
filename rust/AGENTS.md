# AGENTS.md
Instructions for AI coding agents (Codex, Claude Code, Cursor, Copilot, Aider...) working in this repository.
Stack: Rust (cargo, clippy). Replace the <placeholders>.

## Project overview
<One paragraph: what this project does, who uses it, main entry point.>

## Setup and commands
- Install: `cargo build`
- Test: `cargo test`  (must pass before every commit)
- Lint / format: `cargo fmt --check && cargo clippy -- -D warnings`

## Layout
- Source: `src/ (lib.rs, main.rs), tests/ (integration)`
- Tests: unit tests in `mod tests` in the same file, integration tests in tests/

## Conventions
- Style: rustfmt defaults, no `unwrap()` outside tests
- Commits: imperative mood, first line <= 72 chars.
- Do not bump MSRV or edition without asking.
- Do not add a dependency without explaining why in the PR description.

## Boundaries
- Never commit secrets, tokens or `.env` files.
- Ask a human before: public API changes, database migrations, deleting files, CI changes.
- Keep changes small and focused; add or update tests with every behaviour change.

## Definition of done
- [ ] tests pass  - [ ] lint passes  - [ ] docs/README updated if behaviour changed  - [ ] no unrelated edits
