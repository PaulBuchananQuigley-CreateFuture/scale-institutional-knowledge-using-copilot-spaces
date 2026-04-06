# OctoAcme — Ways of Working

> A concise guide to how we work together day-to-day. Keep it as a living document and update it when the team agrees to change a practice.

---

## 1. Principles

| Principle | What it means in practice |
|---|---|
| **Customer-first** | Every piece of work traces back to a customer outcome or measurable metric. |
| **Iterative delivery** | Ship small, testable increments rather than big-bang releases. |
| **Clear ownership** | Every issue, PR, and decision has a named owner. |
| **Documented decisions** | Non-trivial decisions are captured in a decision record so future team members understand the *why*. |
| **Psychological safety** | Feedback is welcomed, mistakes are learning opportunities, and all voices are heard. |

---

## 2. Workflow at a Glance

```
Idea / Request
     │
     ▼
Issue created & triaged (Definition of Ready checked)
     │
     ▼
Sprint/iteration planning — item pulled into "In Progress"
     │
     ▼
Development → PR raised (PR Checklist completed)
     │
     ▼
Code Review → CI passes → Approved
     │
     ▼
Merged → QA / Acceptance testing
     │
     ▼
Definition of Done checked ✓
     │
     ▼
Released (Deployment Checklist completed)
     │
     ▼
Retrospective — learnings captured and actioned
```

---

## 3. Issue Lifecycle

- **Creating an issue**: Use the [issue template](.github/ISSUE_TEMPLATE/) and ensure it meets the [Definition of Ready](templates/definition-of-ready.md) before it is pulled into a sprint.
- **Ownership**: Every issue must have a single assignee once work begins.
- **Status**: Keep the project board up to date — move cards when status changes, not at the end of the sprint.
- **Closing**: An issue is closed only when the [Definition of Done](templates/definition-of-done.md) is satisfied.

---

## 4. Pull Request Conventions

- Keep PRs small (≤ 400 lines where possible). If a PR grows large, split it.
- Link the issue in the PR description (e.g., `Closes #123`).
- Complete the [PR Checklist](templates/pr-checklist.md) before requesting review.
- At least **one approval** is required before merging.
- CI must be green before merge (tests, linting, security scans).
- Delete the source branch after merging.

---

## 5. Meetings & Communication

| Meeting | Cadence | Owner | Purpose |
|---|---|---|---|
| Standup | Twice-weekly (or daily) | Scrum Master / PM | Progress, blockers, dependencies |
| Sprint Planning | Start of each sprint | Scrum Master / PdM | Pull and commit to sprint backlog |
| Sprint Review / Demo | End of each sprint | PM | Showcase completed work |
| Retrospective | End of each sprint or milestone | Scrum Master / PM | Learnings and improvements |
| PM + PdM Sync | Weekly | PM | Risk, priorities, dependencies |
| Stakeholder Update | Monthly | PM | Progress, outcomes, asks |

- Use the [Meeting Notes Template](templates/meeting-notes.md) to capture outcomes and action items.
- Action items must have an **owner** and a **due date**.

---

## 6. Decision Making

- Decisions with broad impact or architectural implications are recorded as [Decision Records](templates/decision-record.md).
- All decisions are logged in the [Decision Log](decision-log.md) with a link to the full record.
- The decision owner is responsible for socialising the decision with affected parties before recording it.

---

## 7. Definition of Ready & Definition of Done

- **Definition of Ready** (DoR): An issue meets DoR before it can be pulled into a sprint. See [Definition of Ready checklist](templates/definition-of-ready.md).
- **Definition of Done** (DoD): Work is only "done" when it meets DoD. See [Definition of Done checklist](templates/definition-of-done.md).

---

## 8. Documentation

- All process docs live in the `docs/` folder.
- Update docs when practices change — stale documentation is worse than no documentation.
- Reference documents in issues and PRs where relevant.

---

*Last updated: see git history. To suggest a change, open an issue or raise a PR.*
