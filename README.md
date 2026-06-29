# WorkReady

Scenario-driven AI skills for students, interns, new graduates, and new employees who need to become reliable workplace operators.

WorkReady turns common workplace situations into slash-command skills. Each skill combines a practical method with a concrete output, so the user does not just get advice. They get a plan, update, message, decision log, stakeholder map, RACI matrix, or operating system they can use at work.

## Positioning

gstack is a skill stack for the software development lifecycle.

WorkReady is a skill stack for the early workplace lifecycle:

**Onboard -> Learn -> Align -> Plan -> Collaborate -> Report -> Operate -> Review**

## Quick Start

Use the root router in [WORKREADY.md](WORKREADY.md), or invoke a specific skill:

| Command | Use when | Main artifact |
|---|---|---|
| `/onboard` | You just joined a team or company | First-week map and onboarding plan |
| `/first90` | You need a 30/60/90-day plan | First 90 days operating plan |
| `/plan` | You received a vague assignment | Clarified work plan |
| `/update` | You need to report progress to a manager | Manager-ready update |
| `/meeting` | You need to turn notes into action | Decisions, owners, follow-up |
| `/raci` | Ownership is unclear | RACI matrix |
| `/stakeholder` | You need to understand key people | Stakeholder map |
| `/status` | You need a project status report | Green/yellow/red status report |
| `/tasks` | You need a personal work system | Task, project, and review system |
| `/retro` | You need a weekly review | Evidence-based retro and next week plan |
| `/datamap` | You need to map process, data, and automation | Process/data/AI opportunity map |
| `/message` | You need to write workplace messages | Clear, professional message variants |

## Methodology Stack

WorkReady intentionally combines four proven workplace methods:

- First 90 Days: learn fast, align expectations, create early wins, and build credibility.
- Manager Tools style new-job operating discipline: understand your manager, clarify success criteria, set a communication cadence, and ask better questions.
- Atlassian-style collaboration tools: RACI, stakeholder mapping, and status reporting.
- Obsidian Tasks + Dataview style personal operations: capture work as structured notes, tasks, projects, meetings, and reviews.

The method files live in [methodologies/](methodologies/). Skills reference them directly so every command has a mature work pattern behind it.

## Repository Structure

```text
workready/
  README.md
  WORKREADY.md
  commands/        # Short slash-command entrypoints
  skills/          # Agent-loadable SKILL.md files
  methodologies/   # Reusable workplace methods
  templates/       # Markdown templates users can copy into notes
  docs/            # Usage and design notes
  examples/        # Example workflows
```

## Design Principles

- Always produce a workplace artifact.
- Make uncertainty explicit.
- Separate effort from outcome.
- Clarify owners, deadlines, dependencies, and decision makers.
- Prefer short, manager-readable outputs over long essays.
- Turn work into a reusable personal operating system.

## Example

```text
/plan

My manager said: "Look into why the weekly report numbers are inconsistent."
Context: I am a new analyst. The report uses CRM exports and a spreadsheet.
Deadline: Friday.
```

WorkReady should return:

- a task interpretation
- assumptions and out-of-scope items
- an execution plan
- risks and dependencies
- questions to ask
- a manager confirmation message

