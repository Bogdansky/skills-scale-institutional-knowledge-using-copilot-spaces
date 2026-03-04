# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

> **Note:** This document was expanded to include additional specialist personas (QA Engineer, UX Designer / Researcher, Business Analyst, Technical Writer, Release Manager) to close gaps identified in [issue #4](https://github.com/Bogdansky/skills-scale-institutional-knowledge-using-copilot-spaces/issues/4). The added roles clarify ownership, handoffs, and collaboration across the full delivery team.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

### Interactions with Other Roles
- **PdM:** Receive feature specs and acceptance criteria; surface technical constraints early.
- **PM:** Report progress, blockers, and estimates; flag risks that affect timelines.
- **QA Engineer:** Hand off completed features for test sign-off; fix reported defects promptly.
- **UX Designer:** Implement designs and raise feasibility concerns during handoff.
- **Technical Writer:** Provide API or feature details to support accurate documentation.

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

### Interactions with Other Roles
- **Developers:** Provide requirements and acceptance criteria; review demos and give sign-off.
- **PM:** Align on timeline, scope, and trade-offs; escalate blockers together.
- **Business Analyst:** Co-own requirements refinement and traceability.
- **UX Designer:** Collaborate on user research, journey maps, and usability goals.
- **Stakeholders:** Present roadmap priorities and gather input; communicate changes proactively.

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

### Interactions with Other Roles
- **Developers:** Remove blockers, track velocity, escalate resource or scope issues.
- **PdM:** Align scope and timeline; facilitate trade-off discussions.
- **Release Manager:** Coordinate release windows and deployment readiness.
- **Stakeholders:** Provide regular status reports and surface risks early.

---

## QA Engineer

### Role Summary
QA Engineers own end-to-end test planning, define quality gates, and ensure release readiness. They act as the quality checkpoint between development and production.

### Responsibilities
- Develop and maintain test plans (unit, integration, e2e, acceptance)
- Define and enforce quality gates and definition of done
- Execute manual and automated tests; report and track defects
- Review acceptance criteria and flag ambiguities before development starts
- Sign off on features prior to release
- Contribute to the [QA Checklist](qa-checklist.md)

### Goals
- Prevent defects from reaching production
- Increase test coverage and automate repetitive test cases
- Provide clear, timely quality signals to the team

### Typical Communication / Interactions
- **Developers:** Receive feature handoffs; file bugs with reproduction steps; collaborate on fix verification.
- **PdM:** Validate acceptance criteria; flag gaps in requirements that affect testability.
- **PM:** Report test status and quality risks on release readiness; flag blockers early.
- **Release Manager:** Provide test sign-off and quality gate status before each release.
- **Stakeholders:** Share high-level quality metrics and release readiness summaries when requested.

### Example Handoffs & RACI Notes
- **R** (Responsible): Test plan creation, defect triage, test sign-off
- **A** (Accountable): Quality gate approval before release
- **C** (Consulted): Requirements review, acceptance criteria definition
- **I** (Informed): Sprint planning outcomes, release dates

---

## UX Designer / Researcher

### Role Summary
UX Designers and Researchers define user journeys, usability goals, and feedback cycles. They ensure that product decisions are grounded in user needs and improve customer experience.

### Responsibilities
- Conduct user research and synthesize findings into actionable insights
- Create wireframes, prototypes, and high-fidelity designs
- Define user journeys and usability success criteria
- Facilitate usability testing and share results with the team
- Collaborate with PdM and Developers to validate design feasibility

### Goals
- Deliver intuitive, accessible experiences that meet user needs
- Reduce usability-related defects and rework
- Enable fast, informed design decisions grounded in evidence

### Typical Communication / Interactions
- **Developers:** Hand off finalized designs with annotations; address implementation questions; review built UI for fidelity.
- **PdM:** Align on user personas and research priorities; co-own usability metrics.
- **PM:** Surface research timelines and design dependencies; flag risks from unresolved usability questions.
- **Business Analyst:** Share user journey findings to refine requirements and acceptance criteria.
- **Stakeholders:** Present research findings and design rationale in review sessions.

### Example Handoffs & RACI Notes
- **R** (Responsible): User research, wireframes, prototype delivery
- **A** (Accountable): Design sign-off before development begins
- **C** (Consulted): Acceptance criteria review, technical feasibility checks
- **I** (Informed): Sprint schedules, release timelines

---

## Business Analyst

### Role Summary
Business Analysts clarify requirements, maintain traceability, and bridge the gap between business stakeholders and the technical team. They support backlog refinement and acceptance criteria definition.

### Responsibilities
- Elicit, document, and validate business and functional requirements
- Maintain requirements traceability from business need to delivered feature
- Facilitate backlog refinement sessions with PdM and Developers
- Write or review acceptance criteria and user stories
- Identify and document process gaps or dependencies
- Support change management and impact analysis

### Goals
- Ensure requirements are complete, testable, and unambiguous before development starts
- Reduce rework caused by misunderstood or missing requirements
- Improve stakeholder alignment on scope and priorities

### Typical Communication / Interactions
- **Developers:** Clarify requirements and acceptance criteria during sprint planning and daily work.
- **PdM:** Co-own backlog refinement; align on business priorities and value metrics.
- **PM:** Raise scope changes, ambiguities, or dependency risks; support impact assessments.
- **QA Engineer:** Share requirements documentation to support test plan creation.
- **Stakeholders:** Gather requirements, validate solutions, and communicate scope changes.

### Example Handoffs & RACI Notes
- **R** (Responsible): Requirements documentation, acceptance criteria authoring
- **A** (Accountable): Requirements sign-off before sprint commitment
- **C** (Consulted): Design reviews, test plan validation
- **I** (Informed): Release schedules, retrospective outcomes

---

## Technical Writer

### Role Summary
Technical Writers maintain user-facing and internal documentation, support onboarding, and enable knowledge sharing between roles.

### Responsibilities
- Author and maintain product, API, and process documentation
- Support onboarding by creating guides and runbooks
- Collaborate with Developers and PdM to document new features accurately
- Review documentation for clarity, accuracy, and consistency
- Maintain the docs/ folder and documentation standards
- Facilitate knowledge transfer across teams

### Goals
- Ensure documentation is accurate, discoverable, and up to date
- Reduce onboarding time for new team members
- Support knowledge retention and reduce dependency on individual people

### Typical Communication / Interactions
- **Developers:** Request technical details (APIs, configs, behaviors) to write accurate docs; review drafts for accuracy.
- **PdM:** Align on feature scope and documentation priorities; ensure docs match product intent.
- **PM:** Coordinate documentation timelines within the release plan.
- **QA Engineer:** Coordinate on test documentation and runbooks.
- **Stakeholders:** Deliver user-facing docs and release notes on schedule.

### Example Handoffs & RACI Notes
- **R** (Responsible): Documentation authoring, review, and publication
- **A** (Accountable): Final docs sign-off before release
- **C** (Consulted): Feature specifications, acceptance criteria
- **I** (Informed): Sprint outcomes, release dates

---

## Release Manager

### Role Summary
Release Managers oversee the release process, ensure checklists and rollback plans are followed, coordinate deployment timing, and communicate release status to stakeholders.

### Responsibilities
- Plan and schedule release windows with PM and Developers
- Ensure all pre-release requirements are met before deployment (see [Release Checklist](release-checklist.md))
- Coordinate go/no-go decisions with PM, QA, and technical leads
- Manage rollback plans and communicate incident status if deployments fail
- Announce releases to stakeholders and support teams
- Track post-deployment health and capture learnings

### Goals
- Deliver releases predictably, safely, and with full team alignment
- Minimize production incidents caused by incomplete release preparation
- Maintain a clear audit trail for every release

### Typical Communication / Interactions
- **Developers:** Confirm code freeze, deployment readiness, and rollback procedures.
- **PM:** Align on release windows, scope, and stakeholder communications.
- **QA Engineer:** Obtain test sign-off and quality gate status before go/no-go.
- **Technical Writer:** Coordinate release notes and user-facing communications.
- **Stakeholders:** Provide release status updates, announce deployments, and report post-deploy health.

### Example Handoffs & RACI Notes
- **R** (Responsible): Release checklist execution, go/no-go coordination, deployment announcement
- **A** (Accountable): Final go/no-go decision (with PM and QA sign-off)
- **C** (Consulted): Rollback plan review, post-deploy monitoring setup
- **I** (Informed): Sprint outcomes, acceptance criteria sign-off

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

