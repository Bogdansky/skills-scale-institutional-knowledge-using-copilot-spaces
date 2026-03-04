# OctoAcme — Release Checklist

**Owners:** Release Manager, Project Manager
**Reference:** [Release & Deployment Guide](octoacme-release-and-deployment.md) | [Roles & Personas](octoacme-roles-and-personas.md)

A pragmatic checklist to follow for every release. Complete each phase in order and obtain sign-offs before proceeding. Track this checklist in the release ticket or project board.

---

## Pre-Release

- [ ] All acceptance criteria met and verified by QA Engineer (see [QA Checklist](qa-checklist.md))
- [ ] All feature PRs merged; code freeze confirmed with Developers
- [ ] CI pipeline passing (build, lint, unit tests, integration tests)
- [ ] Security scan completed with no critical/high findings unresolved
- [ ] Release notes drafted and reviewed by Technical Writer
- [ ] Rollback plan documented and shared with on-call team
- [ ] Deployment window scheduled and communicated to stakeholders
- [ ] Database migrations reviewed and tested (if applicable)
- [ ] Feature flags and configuration changes reviewed
- [ ] Go/no-go sign-off obtained from: PM ☐ QA ☐ Tech Lead ☐

---

## Deploy

- [ ] Backup or snapshot taken (if applicable)
- [ ] Deploy to staging environment
- [ ] Smoke tests run on staging — all critical paths passing
- [ ] Deploy to production via automated pipeline (preferred)
- [ ] Monitor error rates, latency, and health metrics during rollout
- [ ] Confirm deployment successful with on-call/Developers

---

## Post-Deploy Verifications

- [ ] Post-deploy smoke tests passing in production
- [ ] Key user flows verified (happy path + critical edge cases)
- [ ] No spike in error rates or alerts triggered
- [ ] Release announced to stakeholders and support team
- [ ] Release notes published (changelog, docs, or comms channel)
- [ ] Monitoring dashboards reviewed for at least 30 minutes post-deploy

---

## Rollback Criteria

Trigger a rollback if any of the following are observed:

- [ ] Critical user-facing feature is broken or unavailable
- [ ] Error rate exceeds the agreed threshold (e.g., >1% 5xx errors)
- [ ] Data loss or corruption risk identified
- [ ] On-call team cannot mitigate the issue within the agreed SLA window

**Rollback steps:** Follow the [Rollback & Incident Playbook](octoacme-release-and-deployment.md#rollback--incident-playbook).
