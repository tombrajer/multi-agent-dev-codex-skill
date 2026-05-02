# Quick Prompts

## Help

```text
Use the multi-agent-dev skill.
Help me understand what each agent does and which one I should use.
```

## List agents

```text
Use the multi-agent-dev skill.
List available agents with one-line descriptions.
```

## Repo intake

```text
Use the multi-agent-dev skill.
Run repo-intake only.
Do not edit files.
Map project. Identify correct commands.
```

## Bug hunt

```text
Use the multi-agent-dev skill.
Run bug-hunter only.
Do not edit files.
Find top likely bugs in this repo.
```

## Frontend debugging with Chrome DevTools MCP

```text
Use the multi-agent-dev skill.
Run frontend-debugger only.
Use Chrome DevTools MCP to inspect http://localhost:3000.
Do not edit files.
```

## Review current changes

```text
Use the multi-agent-dev skill.
Run diff-reviewer and test-engineer.
Review current git diff.
Do not edit files.
```

## Security review

```text
Use the multi-agent-dev skill.
Run security-reviewer only.
Focus on auth, permissions, API routes, input validation, secrets, and data exposure.
Do not edit files.
```

## Performance review

```text
Use the multi-agent-dev skill.
Run performance-profiler only.
Do not edit files.
Identify highest-value performance risks first.
```

## Architecture review

```text
Use the multi-agent-dev skill.
Run architect-reviewer only.
Do not edit files.
Review structure, coupling, boundaries, and maintainability risks.
```

## Dependency review

```text
Use the multi-agent-dev skill.
Run dependency-reviewer only.
Do not edit files.
Review package risk, drift, and unnecessary weight.
```

## Database review

```text
Use the multi-agent-dev skill.
Run database-reviewer only.
Do not edit files.
Review schema, queries, indexes, migrations, and data correctness risks.
```

## Fix one finding

```text
Use the multi-agent-dev skill.
Run implementation-minimalist and test-engineer.
Fix finding #1 only.
Keep change minimal.
```

## Verify a fix

```text
Use the multi-agent-dev skill.
Run test-engineer only.
Verify finding #1 fix with focused tests or browser evidence.
Do not edit files unless test update required.
```

## Triage findings

```text
Use the multi-agent-dev skill.
Run workflow-strategist only.
Triage previous findings and recommend safest fix order.
Do not edit files.
```

## Final pre-merge review

```text
Use the multi-agent-dev skill.
Run final-merge-reviewer only.
Review current diff before commit or merge.
Do not edit files.
```
