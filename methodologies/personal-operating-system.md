# Personal Operating System Method

Use this method when the user needs to manage tasks, meetings, decisions, notes, projects, and weekly reviews.

This method is inspired by structured notes workflows such as Obsidian Tasks and Dataview. The core idea is to write work in a consistent, queryable shape.

## Core Objects

| Object | Purpose | Required fields |
|---|---|---|
| Task | Track actionable work | owner, project, status, next action, due date |
| Project | Group related work | goal, owner, stakeholders, status, next milestone |
| Meeting | Capture discussion | date, attendees, decisions, action items |
| Decision | Preserve context | date, decision, owner, rationale, follow-up |
| Person | Track relationship context | role, cares about, last contact, next touch |
| Weekly review | Convert activity into learning | wins, evidence, misses, lessons, next priorities |

## Suggested Metadata

```yaml
type:
project:
status:
owner:
due:
priority:
stakeholders:
tags:
```

## Task Syntax

```markdown
- [ ] Task description
  project:
  owner:
  due:
  next:
  waiting_on:
```

## Operating Rules

- Every task must have a next action.
- Every waiting item must have an owner.
- Every meeting should produce decisions, action items, and open questions.
- Every week should end with evidence of work completed and a top-three plan for next week.
- Do not keep important commitments only in chat history.

## Weekly Review Loop

1. Review completed tasks.
2. Review missed or stale tasks.
3. Review decisions and open questions.
4. Review stakeholder follow-ups.
5. Choose next week's top three priorities.
6. Draft a manager-facing update.

