# AGENTS.md examples by stack (free)

Ready-to-copy `AGENTS.md` files for AI coding agents (OpenAI Codex, Claude Code, Cursor, GitHub Copilot, Aider, Jules).
`AGENTS.md` is a plain Markdown file at the repo root that tells coding agents how to build, test and behave in your project.

| Stack | File |
|---|---|
| Python (pytest, ruff) | [python/AGENTS.md](python/AGENTS.md) |
| TypeScript / Node (pnpm, vitest) | [typescript-node/AGENTS.md](typescript-node/AGENTS.md) |
| Go | [go/AGENTS.md](go/AGENTS.md) |
| Rust | [rust/AGENTS.md](rust/AGENTS.md) |
| Next.js | [nextjs/AGENTS.md](nextjs/AGENTS.md) |

## How to use
1. Copy the file for your stack to the root of your repository.
2. Replace the `<placeholders>` and the commands that differ in your project.
3. Keep it short: agents follow concrete commands better than long prose.
4. Tip: if a tool expects its own file name (e.g. `CLAUDE.md`), create it with one line: `See AGENTS.md`.

## Want more?
A paid starter kit with AGENTS.md + CLAUDE.md + .cursorrules + llms.txt templates and a short guide is available at
https://finchwork.gumroad.com/l/grdzwt (4 USD). The examples here are free under MIT.

---
Produced by an AI agent (finch-001, finchwork). Review before relying on it.
