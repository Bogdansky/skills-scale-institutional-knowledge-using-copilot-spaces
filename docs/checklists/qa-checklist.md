# QA Handoff & Release Checklist

> **Owner:** QA Engineer
> **When to use:** Complete this checklist before handing off to the Release Manager for go/no-go approval. Share the completed checklist with the Release Manager, Engineering Lead, and Product Manager.

---

## 1. Test Coverage Summary

- [ ] Test plan created and reviewed for the current release scope
- [ ] All in-scope user stories and acceptance criteria have corresponding test cases
- [ ] Test coverage report generated and coverage meets or exceeds the agreed threshold (e.g., ≥80% for critical paths)
- [ ] Coverage gaps identified, documented, and accepted by the Engineering Lead or PM

---

## 2. End-to-End (E2E) Test Results

- [ ] E2E test suite executed against the release candidate build
- [ ] E2E results documented (total tests, passed, failed, skipped)
- [ ] All E2E failures investigated — root cause identified as either a known issue (waived) or a defect requiring resolution
- [ ] E2E suite run in an environment that mirrors production configuration

---

## 3. Regression Test Results

- [ ] Full regression suite executed on the release branch
- [ ] Regression results documented (pass rate, any new failures compared to previous run)
- [ ] Any regressions triaged — confirmed as either pre-existing (known) or newly introduced
- [ ] Newly introduced regressions resolved or formally accepted/waived with PM sign-off

---

## 4. Flaky Test Mitigation

- [ ] Known flaky tests identified and listed
- [ ] Flaky tests quarantined or re-run strategy applied (e.g., retry logic) so they do not block the release
- [ ] Flaky test backlog updated with newly identified tests
- [ ] Flakiness rate for the release run documented and within acceptable limits

---

## 5. Environment Readiness

- [ ] Test environment mirrors production configuration (versions, infra, data sets)
- [ ] Test data refreshed or seeded appropriately for the release scope
- [ ] Any environment-specific issues (e.g., connectivity, service mocks) resolved before final test run
- [ ] Environment configuration changes required for production documented and handed off to Engineering

---

## 6. Deployment Smoke Test Steps

*These steps are to be executed immediately after deployment to production or staging to confirm the deployment succeeded.*

- [ ] Smoke test script or runbook documented and shared with the on-call team
- [ ] Critical user journeys identified for smoke testing (e.g., login, core workflow, key API endpoints)
- [ ] Smoke test expected results documented (what "passing" looks like for each step)
- [ ] Smoke test pass/fail criteria defined — including what triggers an immediate rollback
- [ ] Person responsible for running the smoke test post-deployment identified

---

## 7. Defect Status Summary

| Severity | Open | Resolved | Waived |
|---|---|---|---|
| P1 (Critical) | | | |
| P2 (High) | | | |
| P3 (Medium) | | | |
| P4 (Low) | | | |

- [ ] All P1 defects resolved or the release has been explicitly delayed/blocked
- [ ] All P2 defects resolved or formally waived with documented rationale and PM approval
- [ ] P3/P4 defects logged in the backlog for future sprints

---

## 8. Sign-Offs

| Approver | Role | Decision | Date |
|---|---|---|---|
| | QA Engineer | ☐ Ready for Release / ☐ Blocked | |
| | Engineering Lead | ☐ Acknowledged / ☐ Concerns raised | |
| | Product Manager | ☐ Approved / ☐ Blocked | |

**QA Recommendation:** ☐ Proceed to Release &nbsp;&nbsp; ☐ Do NOT release — Reason: _____________________

---

## Handoff Notes

*Use this space to communicate any context the Release Manager, Engineering, or Support team should be aware of after the QA sign-off:*

> _[e.g., Known issues deferred to next sprint, unusual test conditions, manual tests that were waived with approval, environment differences noted]_

---

*Last updated: [YYYY-MM-DD] — Owner: QA Engineer*
