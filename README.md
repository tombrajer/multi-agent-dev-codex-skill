![Multi-Agent Dev banner](./assets/banner.svg)

# Multi-Agent Dev Codex Skill

Reusable Codex skill for running senior-dev-style specialist agents inside Codex.

Natural-language first. Senior-dev-style roles. One skill, sixteen specialists, practical workflows.

> Built for repo intake, bug hunting, frontend debugging, testing, security review, performance review, architecture review, docs, accessibility, dependency review, database review, diff review, final merge review, focused fixing, and workflow triage.

`natural-language first` `16 specialist roles` `GitHub-ready` `practical review + fix workflows`

## Jump To

[Quickstart](#quickstart) | [Featured Agents](#featured-agents) | [Installation](#installation) | [Invocation](#invocation) | [All Agents](#all-agents) | [Workflows](#recommended-workflows)

## Quickstart

| Start here | Use when | Prompt |
| --- | --- | --- |
| Help | Need orientation | `Use the multi-agent-dev skill. Help me understand what each agent does and which one I should use.` |
| Inspect | Need fast repo mapping | `Use the multi-agent-dev skill. Run repo-intake only. Do not edit files. Map the project and identify the correct commands.` |
| Review | Need eyes on current changes | `Use the multi-agent-dev skill. Run diff-reviewer and test-engineer. Review the current git diff. Do not edit files.` |
| Fix | Need one issue solved carefully | `Use the multi-agent-dev skill. Run implementation-minimalist and test-engineer. Fix finding #1 only. Keep the change minimal.` |

## Featured Agents

<table>
  <tr>
    <td valign="top" width="33%">
      <img alt="" src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='420' height='170' viewBox='0 0 420 170'%3E%3Cdefs%3E%3ClinearGradient id='g1' x1='18' y1='12' x2='402' y2='158' gradientUnits='userSpaceOnUse'%3E%3Cstop stop-color='%23F8FBFF'/%3E%3Cstop offset='1' stop-color='%23E8F4FF'/%3E%3C/linearGradient%3E%3C/defs%3E%3Crect width='420' height='170' rx='18' fill='url(%23g1)'/%3E%3Crect x='14' y='14' width='392' height='142' rx='14' fill='%23FFFFFF' stroke='%23BFDBFE'/%3E%3Crect x='30' y='30' width='74' height='8' rx='4' fill='%2306B6D4'/%3E%3Ctext x='30' y='62' fill='%230891B2' font-family='Segoe UI,Arial,sans-serif' font-size='14' font-weight='700'%3Erepo-intake%3C/text%3E%3Ctext x='30' y='95' fill='%230F172A' font-family='Segoe UI,Arial,sans-serif' font-size='28' font-weight='800'%3EMap repo fast%3C/text%3E%3Ctext x='30' y='123' fill='%23334155' font-family='Segoe UI,Arial,sans-serif' font-size='16'%3Ecommands, layout, risks, constraints%3C/text%3E%3Ccircle cx='370' cy='48' r='18' fill='%23DBEAFE'/%3E%3Cpath d='M362 48H378' stroke='%232563EB' stroke-width='3' stroke-linecap='round'/%3E%3Cpath d='M370 40V56' stroke='%232563EB' stroke-width='3' stroke-linecap='round'/%3E%3C/svg%3E" />
    </td>
    <td valign="top" width="33%">
      <img alt="" src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='420' height='170' viewBox='0 0 420 170'%3E%3Cdefs%3E%3ClinearGradient id='g2' x1='18' y1='12' x2='402' y2='158' gradientUnits='userSpaceOnUse'%3E%3Cstop stop-color='%23F6FDFF'/%3E%3Cstop offset='1' stop-color='%23E0F2FE'/%3E%3C/linearGradient%3E%3C/defs%3E%3Crect width='420' height='170' rx='18' fill='url(%23g2)'/%3E%3Crect x='14' y='14' width='392' height='142' rx='14' fill='%23FFFFFF' stroke='%23BAE6FD'/%3E%3Crect x='30' y='30' width='74' height='8' rx='4' fill='%232563EB'/%3E%3Ctext x='30' y='62' fill='%232563EB' font-family='Segoe UI,Arial,sans-serif' font-size='14' font-weight='700'%3Ebug-hunter%3C/text%3E%3Ctext x='30' y='95' fill='%230F172A' font-family='Segoe UI,Arial,sans-serif' font-size='28' font-weight='800'%3EFind likely defects%3C/text%3E%3Ctext x='30' y='123' fill='%23334155' font-family='Segoe UI,Arial,sans-serif' font-size='16'%3Eevidence-first review, top risks first%3C/text%3E%3Ccircle cx='370' cy='48' r='18' fill='%23DBEAFE'/%3E%3Cpath d='M363 49L368 54L378 42' stroke='%232563EB' stroke-width='3' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E" />
    </td>
    <td valign="top" width="33%">
      <img alt="" src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='420' height='170' viewBox='0 0 420 170'%3E%3Cdefs%3E%3ClinearGradient id='g3' x1='18' y1='12' x2='402' y2='158' gradientUnits='userSpaceOnUse'%3E%3Cstop stop-color='%23F8FBFF'/%3E%3Cstop offset='1' stop-color='%23EEF2FF'/%3E%3C/linearGradient%3E%3C/defs%3E%3Crect width='420' height='170' rx='18' fill='url(%23g3)'/%3E%3Crect x='14' y='14' width='392' height='142' rx='14' fill='%23FFFFFF' stroke='%23C7D2FE'/%3E%3Crect x='30' y='30' width='74' height='8' rx='4' fill='%2306B6D4'/%3E%3Ctext x='30' y='62' fill='%230891B2' font-family='Segoe UI,Arial,sans-serif' font-size='14' font-weight='700'%3Esecurity-reviewer%3C/text%3E%3Ctext x='30' y='95' fill='%230F172A' font-family='Segoe UI,Arial,sans-serif' font-size='28' font-weight='800'%3EReview attack surface%3C/text%3E%3Ctext x='30' y='123' fill='%23334155' font-family='Segoe UI,Arial,sans-serif' font-size='16'%3Eauth, permissions, secrets, exposure%3C/text%3E%3Ccircle cx='370' cy='48' r='18' fill='%23E0F2FE'/%3E%3Cpath d='M370 40L378 44V50C378 56 374 61 370 63C366 61 362 56 362 50V44L370 40Z' fill='%232563EB'/%3E%3C/svg%3E" />
    </td>
  </tr>
  <tr>
    <td valign="top" width="33%">
      <img alt="" src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='420' height='170' viewBox='0 0 420 170'%3E%3Cdefs%3E%3ClinearGradient id='g4' x1='18' y1='12' x2='402' y2='158' gradientUnits='userSpaceOnUse'%3E%3Cstop stop-color='%23F8FBFF'/%3E%3Cstop offset='1' stop-color='%23E8F4FF'/%3E%3C/linearGradient%3E%3C/defs%3E%3Crect width='420' height='170' rx='18' fill='url(%23g4)'/%3E%3Crect x='14' y='14' width='392' height='142' rx='14' fill='%23FFFFFF' stroke='%23BFDBFE'/%3E%3Crect x='30' y='30' width='74' height='8' rx='4' fill='%232563EB'/%3E%3Ctext x='30' y='62' fill='%232563EB' font-family='Segoe UI,Arial,sans-serif' font-size='14' font-weight='700'%3Etest-engineer%3C/text%3E%3Ctext x='30' y='95' fill='%230F172A' font-family='Segoe UI,Arial,sans-serif' font-size='28' font-weight='800'%3EVerify behavior fast%3C/text%3E%3Ctext x='30' y='123' fill='%23334155' font-family='Segoe UI,Arial,sans-serif' font-size='16'%3Efocused tests, coverage, regression proof%3C/text%3E%3Ccircle cx='370' cy='48' r='18' fill='%23DBEAFE'/%3E%3Cpath d='M361 49L367 55L379 42' stroke='%2306B6D4' stroke-width='3' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E" />
    </td>
    <td valign="top" width="33%">
      <img alt="" src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='420' height='170' viewBox='0 0 420 170'%3E%3Cdefs%3E%3ClinearGradient id='g5' x1='18' y1='12' x2='402' y2='158' gradientUnits='userSpaceOnUse'%3E%3Cstop stop-color='%23F6FDFF'/%3E%3Cstop offset='1' stop-color='%23E8F4FF'/%3E%3C/linearGradient%3E%3C/defs%3E%3Crect width='420' height='170' rx='18' fill='url(%23g5)'/%3E%3Crect x='14' y='14' width='392' height='142' rx='14' fill='%23FFFFFF' stroke='%23BAE6FD'/%3E%3Crect x='30' y='30' width='74' height='8' rx='4' fill='%2306B6D4'/%3E%3Ctext x='30' y='62' fill='%230891B2' font-family='Segoe UI,Arial,sans-serif' font-size='14' font-weight='700'%3Eperformance-profiler%3C/text%3E%3Ctext x='30' y='95' fill='%230F172A' font-family='Segoe UI,Arial,sans-serif' font-size='28' font-weight='800'%3ESpot bottlenecks%3C/text%3E%3Ctext x='30' y='123' fill='%23334155' font-family='Segoe UI,Arial,sans-serif' font-size='16'%3Ehot paths, waste, slow queries, runtime cost%3C/text%3E%3Ccircle cx='370' cy='48' r='18' fill='%23E0F2FE'/%3E%3Cpath d='M370 58V49L376 43' stroke='%232563EB' stroke-width='3' stroke-linecap='round' stroke-linejoin='round'/%3E%3Ccircle cx='370' cy='49' r='9' stroke='%232563EB' stroke-width='3' fill='none'/%3E%3C/svg%3E" />
    </td>
    <td valign="top" width="33%">
      <img alt="" src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='420' height='170' viewBox='0 0 420 170'%3E%3Cdefs%3E%3ClinearGradient id='g6' x1='18' y1='12' x2='402' y2='158' gradientUnits='userSpaceOnUse'%3E%3Cstop stop-color='%23F8FBFF'/%3E%3Cstop offset='1' stop-color='%23E0F2FE'/%3E%3C/linearGradient%3E%3C/defs%3E%3Crect width='420' height='170' rx='18' fill='url(%23g6)'/%3E%3Crect x='14' y='14' width='392' height='142' rx='14' fill='%23FFFFFF' stroke='%23BFDBFE'/%3E%3Crect x='30' y='30' width='74' height='8' rx='4' fill='%232563EB'/%3E%3Ctext x='30' y='62' fill='%232563EB' font-family='Segoe UI,Arial,sans-serif' font-size='14' font-weight='700'%3Eworkflow-strategist%3C/text%3E%3Ctext x='30' y='95' fill='%230F172A' font-family='Segoe UI,Arial,sans-serif' font-size='28' font-weight='800'%3EChoose next safe step%3C/text%3E%3Ctext x='30' y='123' fill='%23334155' font-family='Segoe UI,Arial,sans-serif' font-size='16'%3Etriage findings, order work, reduce risk%3C/text%3E%3Ccircle cx='370' cy='48' r='18' fill='%23DBEAFE'/%3E%3Cpath d='M363 54L370 47L375 51L379 42' stroke='%2306B6D4' stroke-width='3' stroke-linecap='round' stroke-linejoin='round' fill='none'/%3E%3C/svg%3E" />
    </td>
  </tr>
</table>

## Installation

Skill installs by copying whole `multi-agent-dev` folder into Codex skills directory.

Windows:

```powershell
mkdir "$env:USERPROFILE\.codex\skills" -Force
Copy-Item ".\skills\multi-agent-dev" "$env:USERPROFILE\.codex\skills\multi-agent-dev" -Recurse -Force
```

macOS/Linux:

```bash
mkdir -p ~/.codex/skills
cp -R ./skills/multi-agent-dev ~/.codex/skills/multi-agent-dev
```

Restart Codex CLI / reload VS Code Codex extension after installing.

## Invocation

Agents are roles inside one Codex skill, not separate executables or separate UI buttons.

Start with:

```text
Use the multi-agent-dev skill.
Help me understand what each agent does and which one I should use.
```

List agents:

```text
Use the multi-agent-dev skill.
List available agents with one-line descriptions.
```

Repo intake:

```text
Use the multi-agent-dev skill.
Run repo-intake only.
Do not edit files.
Map the project and identify the correct commands.
```

Bug hunt:

```text
Use the multi-agent-dev skill.
Run bug-hunter only.
Do not edit files.
Find the top likely bugs in this repo.
```

Review current diff:

```text
Use the multi-agent-dev skill.
Run diff-reviewer and test-engineer.
Review the current git diff.
Do not edit files.
Afterward, ask me if I want workflow-strategist.
```

Fix one finding:

```text
Use the multi-agent-dev skill.
Run implementation-minimalist and test-engineer.
Fix finding #1 only.
Keep the change minimal.
Add or update tests if appropriate.
Run relevant tests if safe.
Afterward, recommend whether workflow-strategist should run next.
```

Workflow triage:

```text
Use the multi-agent-dev skill.
Run workflow-strategist only.
Triage the previous findings and recommend the safest fix order.
Do not edit files.
```

## All Agents

| Agent | Focus |
| --- | --- |
| `repo-intake` | Map repo shape, commands, risks, and working constraints before deeper work. |
| `codebase-cartographer` | Trace code paths, ownership boundaries, and subsystem relationships. |
| `bug-hunter` | Find highest-probability defects and rank them by severity and evidence. |
| `frontend-debugger` | Investigate browser/UI issues with DOM, network, console, and rendering evidence. |
| `test-engineer` | Design, add, update, and validate targeted test coverage. |
| `implementation-minimalist` | Fix one issue with smallest safe diff and low regression risk. |
| `security-reviewer` | Inspect auth, permissions, validation, secrets, and exposure risks. |
| `performance-profiler` | Look for hot paths, wasted work, slow queries, and runtime bottlenecks. |
| `architect-reviewer` | Review structure, coupling, abstractions, and long-term maintainability. |
| `docs-maintainer` | Improve docs, examples, onboarding guidance, and missing operational context. |
| `accessibility-reviewer` | Check keyboard flow, semantics, contrast, labels, and assistive support. |
| `workflow-strategist` | Triage findings, choose safest order, and recommend next workflow step. |
| `diff-reviewer` | Review current diff for bugs, regressions, missing tests, and scope drift. |
| `final-merge-reviewer` | Perform final pre-commit or pre-merge review across code, tests, and risks. |
| `dependency-reviewer` | Audit packages for risk, drift, unnecessary weight, and upgrade concerns. |
| `database-reviewer` | Review schema, queries, migrations, indexes, and data correctness risks. |

## Recommended Workflows

Inspect first:

```text
Use the multi-agent-dev skill.
Run repo-intake and bug-hunter.
Do not edit files.
Afterward, ask me if I want workflow-strategist.
```

Review changes:

```text
Use the multi-agent-dev skill.
Run diff-reviewer and test-engineer.
Review the current git diff.
Do not edit files.
```

Frontend/browser debugging:

```text
Use the multi-agent-dev skill.
Run frontend-debugger only.
Use Chrome DevTools MCP to inspect http://localhost:3000.
Do not edit files.
```

Security review:

```text
Use the multi-agent-dev skill.
Run security-reviewer only.
Focus on auth, permissions, API routes, input validation, secrets, and data exposure.
Do not edit files.
```

Fix one issue:

```text
Use the multi-agent-dev skill.
Run implementation-minimalist and test-engineer.
Fix finding #1 only.
Keep the change minimal.
```

Final review:

```text
Use the multi-agent-dev skill.
Run final-merge-reviewer only.
Review the current diff before commit or merge.
Do not edit files.
```

## Notes

- Skill can recommend stronger model for high-risk tasks, but cannot switch models automatically.
- Invocation banner appears when skill explicitly invoked.

## Contributing

- Keep `SKILL.md` natural-language first.
- Do not add fake commands unless documented as plain prompts.
- Preserve safety rules.
- Prefer small, practical agent additions.

## License

MIT. See [LICENSE](./LICENSE).
