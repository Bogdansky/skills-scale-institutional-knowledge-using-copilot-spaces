# OctoAcme — QA & Testing Checklist

**Owners:** QA Engineer, Developers
**Reference:** [Roles & Personas](octoacme-roles-and-personas.md) | [Release Checklist](release-checklist.md)

Use this checklist to track testing completeness before a feature or release is signed off. All items in the applicable sections must be checked before QA sign-off is granted.

---

## Test Coverage

- [ ] Unit tests written and passing for all new/changed business logic
- [ ] Integration tests cover service boundaries and key API contracts
- [ ] End-to-end (e2e) tests cover the primary happy-path user flows
- [ ] Edge cases and known failure modes have test coverage
- [ ] Regression tests run to confirm no existing functionality is broken
- [ ] Accessibility checks performed for any UI changes (WCAG AA minimum)

---

## Quality Gates

- [ ] Code coverage meets or exceeds the agreed threshold (e.g., ≥80%)
- [ ] No open critical or high-severity defects for the features in scope
- [ ] All defects found during this cycle are triaged (fixed, deferred with owner, or accepted)
- [ ] Performance benchmarks within acceptable range (if applicable)
- [ ] Security testing completed (SAST/DAST or manual review) — no critical findings

---

## Acceptance Testing

- [ ] Acceptance criteria from the feature spec reviewed and tested
- [ ] Product Manager / Business Analyst sign-off obtained on acceptance tests
- [ ] User-facing flows validated against UX designs (if applicable)
- [ ] Test results documented and shared with PM and Release Manager

---

## Test Sign-Off

| Role | Sign-off | Date |
|------|----------|------|
| QA Engineer | ☐ | |
| Developer (feature owner) | ☐ | |
| Product Manager | ☐ | |

> **Next step:** Once all items are checked and sign-offs collected, update the [Release Checklist](release-checklist.md) with QA sign-off status.
