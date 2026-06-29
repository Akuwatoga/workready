---
name: workready
version: 0.1.0
description: Route workplace situations to scenario skills for onboarding, planning, collaboration, reporting, task systems, and first-90-days execution.
triggers:
  - workready
  - help me with work
  - new job plan
  - workplace skills
---

## When To Invoke

Use WorkReady when the user needs help operating at work: onboarding, planning, manager updates, meetings, RACI, stakeholder mapping, status reporting, personal task systems, retrospectives, business/data mapping, or workplace messaging.

## Start Here

Read `WORKREADY.md` and choose the best route. If the user already named a slash command, load that command's `skills/<name>/SKILL.md`.

## Priority Methods

Apply these methods in this order when relevant:

1. First 90 Days: establish credibility, learn the organization, align with the manager, create early wins.
2. Manager alignment: clarify success criteria, priority, cadence, quality bar, decision rights, escalation rules.
3. Atlassian-style collaboration tools: RACI, stakeholder mapping, status reporting.
4. Personal operating system: capture tasks, meetings, decisions, projects, and weekly reviews in structured notes.

## Global Rules

- Always produce a concrete workplace artifact.
- Preserve the user's facts and mark assumptions.
- Include owners, deadlines, dependencies, decisions, and next actions.
- Prefer concise manager-readable outputs.
- If the user is new to a role, bias toward first-90-days credibility and manager alignment.
- If cross-functional ownership is unclear, include RACI.
- If project health is unclear, include status report framing.
- If work may repeat, suggest a note/template location from `templates/`.

