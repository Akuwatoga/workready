# Analyst Lifecycle

WorkReady Analyst follows this lifecycle:

```text
Intake -> Clarify -> Map Data -> Analyze -> Update -> Review -> Evidence
```

## 1. Intake

Use `/analyst-intake` when a request is vague.

Output:

- business question
- requester and decision owner
- expected deliverable
- metric questions
- data-source questions
- timeline
- risk
- confirmation message

## 2. Clarify

Use the confirmation message to align with the requester, manager, or stakeholder.

Readiness gate:

- requester identified
- final user identified
- metric definition confirmed or flagged
- data source confirmed or flagged
- deadline known
- deliverable format known

## 3. Map Data

Use `/datamap` when data source, owner, access, quality, or reporting dependency is unclear.

Output:

- source map
- owner map
- key field map
- known quality issues
- access gaps

## 4. Analyze

Use `/analysis-plan` after intake is clear.

Output:

- hypothesis tree
- data pull plan
- analysis method
- chart/table plan
- conclusion structure

## 5. Update

Use `/update` during execution.

Output:

- conclusion first
- progress
- risk
- decision/support needed
- next step

## 6. Review

Use `/retro` weekly.

Output:

- completed work
- evidence
- lessons
- missed risks
- next week priorities

## 7. Evidence

Use `/promotion-pack` near probation review.

Output:

- project impact
- capability growth
- feedback
- evidence log
- next-stage plan

