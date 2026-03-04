# OctoAcme — Handoff & Communication Checklist

**Owners:** All roles (see RACI in [Roles & Personas](octoacme-roles-and-personas.md))
**Reference:** [Project Planning](octoacme-project-planning.md) | [Execution & Tracking](octoacme-execution-and-tracking.md)

Use this checklist at each major cross-role handoff to reduce missed steps and improve clarity. Complete all applicable items before passing work to the next role.

---

## Requirements → Development Handoff

*Owner: Business Analyst / Product Manager → Developers*

- [ ] Problem statement and user stories are written and reviewed
- [ ] Acceptance criteria are specific, testable, and agreed upon
- [ ] Designs or wireframes attached and annotated (UX Designer sign-off)
- [ ] Dependencies and blockers identified and documented
- [ ] Definition of Done reviewed and confirmed with the team
- [ ] Any open questions resolved or formally deferred with an owner

---

## Development → QA Handoff

*Owner: Developers → QA Engineer*

- [ ] Feature branch merged; code review completed and approved
- [ ] Unit and integration tests passing in CI
- [ ] Test environment updated and stable
- [ ] Known limitations or deferred items documented
- [ ] QA test plan reviewed and any gaps flagged to PM
- [ ] Deployment notes (env vars, migrations, flags) communicated to QA and Release Manager

---

## QA → Release Handoff

*Owner: QA Engineer → Release Manager*

- [ ] [QA Checklist](qa-checklist.md) completed and sign-offs collected
- [ ] No open critical/high defects in scope for this release
- [ ] Test summary report shared with PM and Release Manager
- [ ] Go/no-go recommendation provided by QA Engineer

---

## Release → Stakeholders Handoff

*Owner: Release Manager / PM → Stakeholders*

- [ ] Release notes finalized by Technical Writer
- [ ] Deployment completed and post-deploy verifications passed (see [Release Checklist](release-checklist.md))
- [ ] Release announcement sent to stakeholders and support team
- [ ] Documentation updated to reflect shipped changes
- [ ] Feedback channel or escalation path communicated to stakeholders
