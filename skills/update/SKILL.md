---
name: update
version: 0.1.0
description: Convert raw work notes into concise manager-ready updates with progress, risks, asks, and next actions.
triggers:
  - manager update
  - status update
  - report my progress
  - weekly update
---

## When To Invoke

Use `/update` before manager syncs, weekly reports, chat updates, or any situation where the user needs to make work visible.

## Load Methods

Read and apply:

- `methodologies/status-report.md`
- `methodologies/manager-alignment.md`

## Workflow

1. Extract completed work, evidence, impact, risks, blockers, and asks from the user's notes.
2. Choose the right status level if project health is mentioned.
3. Put the most important point first.
4. Make decisions and support requests explicit.
5. Provide multiple formats if useful.

## Output

### One-Line Summary

One sentence that captures the most important update.

### Concise Chat Update

Short version suitable for Slack, Feishu, DingTalk, WeChat, or Teams.

### Structured Manager Update

1. Progress
2. Evidence/impact
3. Risks or blockers
4. Decision/support needed
5. Next actions

### Decision Or Support Request

| Need | Owner | Deadline | Recommendation |
|---|---|---|---|

