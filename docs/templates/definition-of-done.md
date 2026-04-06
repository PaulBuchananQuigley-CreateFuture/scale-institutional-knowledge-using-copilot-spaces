# Definition of Done Checklist

Work is **done** only when **all** applicable criteria below are satisfied. Apply this checklist before closing an issue or marking a story complete.

---

## Checklist

### Code Quality
- [ ] Code is reviewed and approved by at least one peer.
- [ ] No known linting errors or code-style violations.
- [ ] No commented-out code left in the PR (unless explicitly documented).

### Testing
- [ ] Unit tests are written or updated for new/changed logic.
- [ ] Integration tests updated where applicable.
- [ ] All automated tests pass in CI.
- [ ] Manual QA / acceptance testing completed (if required for this item).

### Acceptance Criteria
- [ ] All acceptance criteria defined in the issue are met.
- [ ] Edge cases and error scenarios from the issue have been verified.
- [ ] Stakeholder / Product Manager sign-off obtained (for user-facing changes).

### Documentation
- [ ] Code-level documentation (comments, docstrings) updated.
- [ ] Relevant process or user-facing docs updated (if behaviour changed).
- [ ] Release notes entry drafted (for user-visible changes).

### Security & Compliance
- [ ] Security scanning in CI has passed.
- [ ] No new vulnerabilities introduced (or existing ones are tracked and accepted).
- [ ] Data handling changes reviewed against privacy/compliance requirements (if applicable).

### Deployment Readiness
- [ ] Feature flag or configuration documented (if applicable).
- [ ] Rollback plan noted (for significant changes).
- [ ] Monitoring / alerting updated for new components (if applicable).

---

## When to use this checklist
- Before closing an issue or moving a card to "Done" on the project board.
- During sprint review to validate completed items.
- As part of the PR description for significant features.

---

## Tips
- Not every criterion applies to every piece of work — use judgement and mark N/A where genuinely not applicable.
- Update this checklist in retrospectives if criteria are consistently skipped or missing.

---

*Part of the [OctoAcme Ways of Working](../ways-of-working.md). See also: [Definition of Ready](definition-of-ready.md).*
