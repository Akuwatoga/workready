---
name: status
version: 0.1.0
description: Prepare project status reports that show progress, risks, blockers, decisions, owners, and recommendations.
triggers:
  - project status
  - status report
  - risk update
  - escalation
---

## When To Invoke

Use `/status` for project reporting, escalation, steering updates, delivery reviews, or any work where managers need a clear health signal.

## Load Methods

Read and apply:

- `methodologies/status-report.md`
- `methodologies/raci.md`

## Workflow

1. Determine green/yellow/red status from facts.
2. Put the key message first.
3. Show evidence for completed work.
4. Name risks, blockers, owners, and mitigation.
5. Ask for decisions with a recommendation.

## Output

### Status Summary

- Overall status: Green / Yellow / Red
- One-line summary:

### Progress

| Completed | Evidence | Impact |
|---|---|---|

### Next Actions

| Action | Owner | Deadline | Output |
|---|---|---|---|

### Risks And Blockers

| Risk/blocker | Impact | Owner | Mitigation |
|---|---|---|---|

### Decisions Needed

| Decision | Decision owner | Deadline | Recommendation |
|---|---|---|---|

