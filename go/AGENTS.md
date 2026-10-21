# AGENTS.md
Instructions for AI coding agents (Codex, Claude Code, Cursor, Copilot, Aider...) working in this repository.
Stack: Go (modules, go test, golangci-lint). Replace the <placeholders>.

## Project overview
<One paragraph: what this project does, who uses it, main entry point.>

## Setup and commands
- Install: `go mod download`
- Test: `go test ./...`  (must pass before every commit)
- Lint / format: `gofmt -l . && golangci-lint run`

## Layout
- Source: `cmd/ (binaries), internal/ (private packages), pkg/ (public)`
- Tests: table-driven tests in *_test.go next to code

## Conventions
- Style: gofmt, wrap errors with %w, context as first arg
- Commits: imperative mood, first line <= 72 chars.
- Run `go mod tidy` after dependency changes; never vendor without asking.
- Do not add a dependency without explaining why in the PR description.

## Boundaries
- Never commit secrets, tokens or `.env` files.
- Ask a human before: public API changes, database migrations, deleting files, CI changes.
- Keep changes small and focused; add or update tests with every behaviour change.

## Definition of done
- [ ] tests pass  - [ ] lint passes  - [ ] docs/README updated if behaviour changed  - [ ] no unrelated edits
