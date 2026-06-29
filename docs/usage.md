# Usage

## Basic Pattern

Use a command and paste your raw notes:

```text
/analyst-intake

Here are my notes:
- My manager asked me to look into why retention dropped last week.
- I am a new data analyst.
- I do not know which retention metric they mean.
```

The skill should turn the notes into an analyst intake artifact with clarifying questions, metric/data-source risks, kickoff plan, and confirmation message.

## Analyst Workflow

Use this when you are a data analyst, business analyst, BI analyst, or operations analyst handling vague data requests:

1. Start with `/analyst-intake`.
2. Use `/datamap` if metric definition, data source, owner, access, or quality is unclear.
3. Use `/update` while executing the analysis.
4. Use `/retro` weekly to turn work into probation evidence.
5. Later, use `/promotion-pack` when that skill exists.

## First Month Workflow

| Time | Recommended skills | Purpose |
|---|---|---|
| Before day 1 | `/onboard`, `/stakeholder` | Understand role, people, and questions |
| Week 1 | `/onboard`, `/tasks`, `/update` | Build a first-week operating rhythm |
| Week 2 | `/analyst-intake`, `/meeting`, `/message` | Convert data requests and meetings into action |
| Week 3 | `/raci`, `/status`, `/datamap` | Clarify ownership, reporting, and systems |
| Week 4 | `/first90`, `/retro` | Turn learning into a 30/60/90 plan |

## Daily Workflow

1. Start the day with `/tasks`.
2. Use `/analyst-intake` for vague data-analysis requests.
3. Use `/plan` for non-analyst vague assignments.
4. Use `/meeting` after every important discussion.
5. Use `/message` before sending sensitive messages.
6. Use `/update` before manager syncs.

## Weekly Workflow

1. Run `/retro` on Friday or Sunday.
2. Convert unfinished work into `/tasks`.
3. Turn project risk into `/status`.
4. Update stakeholder communication plans with `/stakeholder`.

## Suggested Note Folders

```text
work/
  inbox/
  daily/
  meetings/
  projects/
  people/
  decisions/
  reports/
  data/
  retros/
  memory/
```

The templates in [templates/](../templates/) are designed to work with this structure.
