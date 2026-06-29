---
name: analyst-intake
version: 0.1.0
description: Turn vague business or data analysis requests into scoped analyst work with clarifying questions, metric/data-source risks, kickoff plan, and confirmation message.
triggers:
  - analyst intake
  - data analysis request
  - business analysis task
  - metric question
  - dashboard request
  - look into the data
---

## When To Invoke

Use `/analyst-intake` when a new data analyst receives a vague business, metric, dashboard, reporting, investigation, or data pull request.

Typical user:

- new graduate data analyst
- business analyst
- operations analyst
- BI analyst
- strategy analyst
- intern doing data work

Typical raw requests:

- "Can you look into why retention dropped?"
- "Help me analyze this campaign."
- "Check whether GMV is abnormal this week."
- "Make a dashboard for the sales team."
- "看看最近转化率为什么不太对。"

## Load Methods

Read and apply:

- `methodologies/analyst-intake.md`
- `methodologies/business-data-map.md`
- `methodologies/manager-alignment.md`
- `docs/memory.md`
- `role-packs/analyst/checklist.md`

## Memory Context

Read if present:

- `memory/user-profile.md`
- `memory/manager-preferences.md`
- `memory/data-sources.md`
- `memory/metric-definitions.md`
- `memory/lessons-learned.md`

Use memory to personalize assumptions and questions. Do not treat memory as always current. If a memory item may be stale, flag it.

After producing the artifact, include suggested memory updates. Do not silently store sensitive company data.

## Inputs To Ask For Or Infer

- raw request
- requester
- manager or decision owner
- business background
- expected output
- known metrics
- known data sources
- deadline/checkpoint
- current assumptions
- user's probation context

If information is missing, create a draft with assumptions and mark unknowns.

## Workflow

1. Restate the raw request as a business question.
2. Identify requester, decision owner, final user, and stakeholder gaps.
3. Extract or infer metrics, population, time window, and deliverable format.
4. Map likely data sources and data owners.
5. Flag ambiguity, risk, and dependencies.
6. Produce a first-pass kickoff plan.
7. Draft a confirmation message the analyst can send before starting.
8. Run the readiness gate.
9. Suggest memory updates.

## Output

### Intake Brief

| Area | Current understanding | Evidence | Unknown | Next action |
|---|---|---|---|---|

### Business Question

Rewrite the request as a clear decision-oriented question.

### Clarifying Questions

| Priority | Question | Who to ask | Why it matters |
|---|---|---|---|

### Metric And Definition Risks

| Metric | Current definition | Unknowns | Owner/source | Risk |
|---|---|---|---|---|

### Data Source Map

| Source | Owner | Access | Key fields | Quality/access risks |
|---|---|---|---|---|

### Assumptions And Risks

| Assumption/risk | Impact | Mitigation |
|---|---|---|

### Kickoff Plan

| Step | Action | Output | Owner | Deadline/checkpoint |
|---|---|---|---|---|

### Confirmation Message

Draft a concise message to the requester or manager that confirms:

- goal
- scope
- metric/data-source questions
- expected output
- timeline
- first checkpoint

### Readiness Gate

Mark each item as Ready / Missing / Risk:

| Gate | Status | Note |
|---|---|---|
| Requester is known | | |
| Decision owner/final user is known | | |
| Business decision/use is known | | |
| Metric definition is confirmed or flagged | | |
| Data source is confirmed or flagged | | |
| Deliverable format is known | | |
| Deadline/checkpoint is known | | |
| Major risks are visible | | |
| Confirmation message is ready | | |

### Suggested Memory Updates

| File | Update | Reason |
|---|---|---|

