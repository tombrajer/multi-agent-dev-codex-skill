# AGENTS.md

## Project commands
- Install:
- Dev server:
- Tests:
- Lint:
- Typecheck:
- Build:

## Repo layout
- Source:
- Tests:
- Docs:
- Config:
- Generated files to avoid:

## Code style
- Follow existing style.
- Prefer minimal diffs.
- Avoid broad refactors unless requested.

## Testing rules
- Run narrow tests first.
- Add or update tests for bug fixes.
- Do not add brittle tests.

## Safety rules
- Do not edit generated files.
- Do not touch secrets or `.env` files unless explicitly asked.
- Do not run destructive commands.
- Ask before migrations, package installs, deploys, branch changes, commits, or pushes.

## Multi-agent workflow rules
- Inspect first.
- Triage findings.
- Fix one issue at a time.
- Verify with tests/browser evidence.
- Run final review before commit/merge.

## Definition of done
- Requested issue fixed or reviewed.
- Relevant tests/checks run or recommended.
- Remaining risks documented.
- No unrelated changes made.
