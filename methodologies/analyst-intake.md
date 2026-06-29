# Analyst Intake Method

Use this method when a new data analyst receives a vague request and needs to turn it into scoped analytical work.

## Purpose

Prevent rework by clarifying business context, decision use, metric definitions, data sources, ownership, deliverable format, timeline, and risk before analysis starts.

## Core Insight

For a new analyst, the first failure usually happens before the query is written:

- the business question is vague
- the metric definition is assumed
- the data source is not confirmed
- the requester and decision owner are different people
- the deliverable format is unclear
- the analyst works silently until the deadline

Analyst intake exists to make the work legible before execution.

## Intake Questions

| Area | Questions |
|---|---|
| Business context | What decision or business problem triggered this request? |
| Requester | Who asked for this? Who will use the result? |
| Decision owner | Who will make a decision based on the analysis? |
| Metric | Which metric is involved? How is it defined? |
| Population | Which users/orders/stores/products/regions/time windows are included? |
| Data source | Which table, dashboard, CRM, log, spreadsheet, or system is the source of truth? |
| Owner | Who owns the metric or data source? |
| Deliverable | Is the output a quick answer, table, dashboard, slide, doc, or recommendation? |
| Timeline | When is the first checkpoint and final delivery? |
| Risk | What could make the answer misleading, late, or unusable? |

## Output Pattern

1. Restate the request as a business question.
2. Identify ambiguity and assumptions.
3. List clarifying questions in priority order.
4. Map likely metrics and data sources.
5. Flag risks and dependencies.
6. Create a first-pass analysis plan.
7. Draft a confirmation message.
8. Suggest memory updates.

## Readiness Gate

Before analysis starts, check:

- [ ] Requester is known.
- [ ] Final user or decision owner is known.
- [ ] Business decision/use is known.
- [ ] Metric definition is confirmed or flagged.
- [ ] Data source is confirmed or flagged.
- [ ] Deliverable format is known.
- [ ] Deadline or checkpoint is known.
- [ ] Major risks are visible.
- [ ] Confirmation message is ready.

If three or more items are missing, recommend clarification before execution.

