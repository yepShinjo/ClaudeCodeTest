# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Status

This repository is freshly initialized — it currently contains only `README.md`
and `.gitignore`. There is no build system, test suite, or application code yet.
Update this file with build/test/run commands and architecture notes once code
is added.

## GitHub workflow (required)

This project follows the user's standing convention: never lose progress, keep
changes reversible.

- **Branches, not direct-to-main.** Do substantive work on a feature branch, not
  on `main`. Branch naming: `feat/…`, `fix/…`, `chore/…`, `docs/…`.
- **Ship via pull request.** Push the branch and open a PR against `main` with
  `gh pr create --fill --base main`. Do not merge automatically — leave merging
  (or closing) to the user.
- **Slash commands** (defined globally in `~/.claude/commands/`):
  - `/ship` — branch the current changes, commit, push, and open a PR.
  - `/new-gh-project` — set up a new folder as its own public GitHub repo.
- Remote `origin` → https://github.com/yepShinjo/ClaudeCodeTest (public).
