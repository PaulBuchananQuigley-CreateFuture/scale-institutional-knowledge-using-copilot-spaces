# Pull Request Checklist & Review Guide

Use this guide when **raising** a PR and when **reviewing** one.

---

## For the Author — Before Requesting Review

### Completeness
- [ ] The PR description clearly explains *what* changed and *why*.
- [ ] The linked issue number is included (e.g., `Closes #123`).
- [ ] Acceptance criteria from the issue are summarised or linked.

### Code Quality
- [ ] The PR is focused — unrelated changes are in a separate PR.
- [ ] PR size is reasonable (aim for ≤ 400 lines of meaningful change; split if larger).
- [ ] No debug code, TODOs, or temporary hacks are left in without a tracking issue.

### Tests & CI
- [ ] New or changed logic has unit tests.
- [ ] All CI checks pass (tests, linting, security scans).

### Documentation
- [ ] Inline code comments are added for complex logic.
- [ ] Any user-facing or process docs affected by this change are updated.

### Review Readiness
- [ ] Self-review completed — read your own diff before requesting review.
- [ ] At least one reviewer has been assigned.

---

## For the Reviewer — Review Guide

### What to look for
1. **Correctness** — Does the code do what the issue/acceptance criteria require?
2. **Edge cases** — Are error states and boundary conditions handled?
3. **Readability** — Is the code clear and maintainable?
4. **Tests** — Are tests meaningful and sufficient?
5. **Security** — Are there any obvious vulnerabilities (injection, secrets in code, insecure defaults)?
6. **Performance** — Are there obvious performance concerns for the scale we operate at?
7. **Documentation** — Is the change documented adequately?

### How to give feedback
- Be specific and constructive — reference the line and explain the concern.
- Distinguish between blocking issues and suggestions:
  - **[blocking]** — must be resolved before merge.
  - **[nit]** — minor style or preference; author can decide.
  - **[question]** — seeking clarification, not necessarily requesting a change.
- Approve only when you are confident the change is ready to ship.

### Review SLA
- Aim to complete reviews within **1 business day** of being assigned.
- If you cannot review within that window, say so and suggest an alternative reviewer.

---

## Merge Criteria

A PR can be merged when:
- [ ] At least **one approval** from a team member (or more, per team policy).
- [ ] All **blocking** review comments are resolved.
- [ ] CI is **green** (tests, lint, security).
- [ ] The author has **not** force-pushed after approval without re-requesting review.

---

*Part of the [OctoAcme Ways of Working](../ways-of-working.md). See also: [Definition of Done](definition-of-done.md).*
