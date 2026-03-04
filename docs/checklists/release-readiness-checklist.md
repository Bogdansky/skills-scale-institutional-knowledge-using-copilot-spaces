# Release Readiness Checklist

> **Owner:** Release Manager (with contributions from QA, Engineering, Product, and Technical Writer)
> **When to use:** Complete this checklist before authorising any production deployment. All items must be checked or explicitly waived with a documented reason before the go/no-go decision is made.

---

## 1. Release Branch & Code Freeze

- [ ] Release branch created from the correct base (e.g., `main` or agreed integration branch)
- [ ] Code freeze date communicated to and acknowledged by all contributing engineers
- [ ] No unapproved commits added to the release branch after code freeze
- [ ] All intended pull requests merged and release branch reflects the intended scope

---

## 2. CI / Build Green

- [ ] All automated CI checks (build, lint, unit tests) passing on the release branch
- [ ] No known build warnings that could indicate unreliable artefacts
- [ ] Release artefact (container image, package, binary) successfully built and tagged
- [ ] Artefact version/tag confirmed correct and matches release notes

---

## 3. Database & Migration Steps

- [ ] All database migration scripts reviewed and approved
- [ ] Migrations tested in a staging or pre-production environment
- [ ] Migration rollback scripts prepared and tested
- [ ] Estimated migration runtime documented; downtime window (if any) communicated to stakeholders

---

## 4. Release Notes

- [ ] Release notes drafted and reviewed by Technical Writer and Product Manager
- [ ] All user-facing changes (features, fixes, deprecations) captured
- [ ] Breaking changes clearly marked with upgrade/migration guidance
- [ ] Release notes ready to publish at deployment time

---

## 5. Rollback Plan

- [ ] Rollback procedure documented (steps to revert the deployment)
- [ ] Rollback tested in staging or confirmed viable via dry-run
- [ ] Rollback decision criteria defined (e.g., error rate threshold, on-call trigger)
- [ ] Rollback owner identified and available during the deployment window

---

## 6. QA Sign-Off

- [ ] QA Engineer confirms all acceptance criteria for in-scope stories are met
- [ ] No open P1 or P2 defects (or all known critical bugs waived with PM approval and documented)
- [ ] Regression test suite executed with results documented
- [ ] QA sign-off document shared with Release Manager

---

## 7. Accessibility & Usability Checks

- [ ] Accessibility tests run (e.g., automated WCAG 2.1 AA checks, screen reader smoke test)
- [ ] UX Designer confirmed design fidelity for any new or changed UI components
- [ ] Usability concerns raised during testing resolved or deferred with documented rationale
- [ ] Internationalisation / localisation (if applicable) validated

---

## 8. Documentation Updated

- [ ] User-facing documentation updated to reflect new or changed features
- [ ] Internal runbooks or operational guides updated (if deployment steps changed)
- [ ] API documentation updated (if APIs changed or new endpoints added)
- [ ] Docs changes reviewed and merged before or alongside the release

---

## 9. Communications Plan

- [ ] Internal stakeholders notified of release date, scope, and any expected impact
- [ ] Deployment window and expected downtime (if any) communicated at least 24 hours in advance
- [ ] On-call / support team briefed on changes and potential issues
- [ ] Escalation path confirmed and contacts available during deployment

---

## 10. Stakeholder Notification

- [ ] Product Manager sign-off on release scope confirmed
- [ ] Engineering lead confirms the build is stable and ready
- [ ] Customer-facing or external communication drafted (if applicable)
- [ ] Post-release monitoring plan in place (dashboards, alert thresholds, on-call rotation)

---

## Go / No-Go Decision

| Approver | Role | Sign-Off | Date |
|---|---|---|---|
| | QA Engineer | ☐ Approved / ☐ Blocked | |
| | Engineering Lead | ☐ Approved / ☐ Blocked | |
| | Product Manager | ☐ Approved / ☐ Blocked | |
| | Technical Writer | ☐ Approved / ☐ Blocked | |
| | Release Manager | ☐ **Final Go / No-Go** | |

**Decision:** ☐ GO — Proceed with deployment &nbsp;&nbsp; ☐ NO-GO — Reason: _____________________

---

*Last updated: [YYYY-MM-DD] — Template maintained by Release Manager*
