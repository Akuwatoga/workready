# WorkReady Skills

Each skill is a scenario-specific workplace operator. The user can invoke it directly with a slash command or let the router in [WORKREADY.md](../WORKREADY.md) choose.

| Skill | Specialist role | Primary methods | Output |
|---|---|---|---|
| `/onboard` | Onboarding coach | First 90 Days, manager alignment, stakeholder mapping | First-week plan |
| `/first90` | New-role strategist | First 90 Days, manager alignment, personal system | 30/60/90-day plan |
| `/plan` | Work planner | Manager alignment, personal system | Execution plan |
| `/update` | Manager communication editor | Status report, manager alignment | Manager update |
| `/meeting` | Meeting operator | Personal system, status report | Decisions and action items |
| `/raci` | Ownership clarifier | RACI | Ownership matrix |
| `/stakeholder` | Collaboration strategist | Stakeholder mapping | Stakeholder map |
| `/status` | Project reporter | Status report, RACI | Project status report |
| `/tasks` | Personal ops designer | Personal operating system | Work system |
| `/retro` | Learning coach | Personal operating system, First 90 Days | Weekly review |
| `/datamap` | Business/data analyst | Business/data map, personal system | Process and automation map |
| `/message` | Workplace writing editor | Manager alignment, status report | Message variants |

## Skill Shape

Every `skills/<name>/SKILL.md` follows the same shape:

1. When to invoke
2. Methods to load
3. Inputs to collect or infer
4. Workflow
5. Output artifact

This mirrors gstack's pattern: a slash command is not a loose prompt; it is an executable workplace procedure with a defined role and output.

## Skill Chaining

Useful chains:

| Situation | Chain |
|---|---|
| First week in a new role | `/onboard -> /stakeholder -> /tasks -> /update -> /retro` |
| Vague manager assignment | `/plan -> /message -> /tasks -> /update` |
| Cross-functional project | `/stakeholder -> /raci -> /status -> /meeting` |
| Data/process automation discovery | `/datamap -> /plan -> /status` |
| Weekly operating rhythm | `/tasks -> /meeting -> /update -> /retro` |

