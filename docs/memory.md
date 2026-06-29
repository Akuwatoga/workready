# WorkReady Memory

WorkReady should get better as the user works with it, but the memory model must be explicit, local, and inspectable.

## Principle

Do not silently assume that every chat message becomes permanent memory. Durable memory exists only when the agent writes structured files into the user's workspace or another user-approved local location.

## Memory Goals

WorkReady memory should help the agent remember:

- who the user is
- what role and probation stage they are in
- how their manager prefers updates
- what business metrics and data sources they use
- what mistakes or lessons have already appeared
- what work evidence can support probation or promotion review

## Suggested Memory Structure

```text
memory/
  user-profile.md
  manager-preferences.md
  work-patterns.md
  data-sources.md
  metric-definitions.md
  lessons-learned.md
  analyst-intake-history/
  promotion-evidence/
```

## Read-Write Contract

Every skill that supports memory should follow this loop:

1. Read relevant memory files if they exist.
2. Use memory as context, not as unquestionable truth.
3. Produce the requested workplace artifact.
4. Suggest exact memory updates.
5. Write updates only when the user asks or the skill explicitly owns that memory file.

## Memory Safety Rules

- Keep memory local by default.
- Do not store secrets, passwords, private credentials, salary details, or sensitive company data unless the user explicitly chooses to.
- Prefer summaries over raw chat transcripts.
- Mark assumptions and stale information.
- Include dates on manager preferences, metric definitions, and lessons.
- Allow the user to edit memory manually.

## Analyst Memory Files

For the analyst wedge, these files matter most:

### `memory/user-profile.md`

```markdown
# User Profile

- Role:
- Company/team type:
- Probation stage:
- Current goal:
- Main anxiety:
- Current skill gaps:
```

### `memory/manager-preferences.md`

```markdown
# Manager Preferences

| Date | Preference | Evidence | Confidence |
|---|---|---|---|
```

### `memory/data-sources.md`

```markdown
# Data Sources

| Source | Owner | Key fields | Access | Known issues | Last verified |
|---|---|---|---|---|---|
```

### `memory/metric-definitions.md`

```markdown
# Metric Definitions

| Metric | Definition | Source | Owner | Caveats | Last verified |
|---|---|---|---|---|---|
```

### `memory/lessons-learned.md`

```markdown
# Lessons Learned

| Date | Situation | Lesson | Next behavior |
|---|---|---|---|
```

### `memory/promotion-evidence/`

Store weekly and project evidence that can later feed `/promotion-pack`.

## Skill Integration Pattern

Every analyst skill should include a memory section:

```markdown
## Memory Context

Read if present:

- `memory/user-profile.md`
- `memory/manager-preferences.md`
- `memory/data-sources.md`
- `memory/metric-definitions.md`
- `memory/lessons-learned.md`

After producing the artifact, output:

### Suggested Memory Updates

| File | Update | Reason |
|---|---|---|
```

