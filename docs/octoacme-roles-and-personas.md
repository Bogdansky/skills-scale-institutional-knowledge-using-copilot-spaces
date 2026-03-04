# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

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

---

---

## QA Engineer

### Role Summary
QA Engineers own the quality assurance process from test planning through release sign-off. They define quality gates, manage test coverage, and act as the last line of defense before code reaches production.

### Responsibilities
- Develop and maintain test plans, test cases, and automated test suites
- Define and enforce quality gates for feature acceptance and releases
- Execute regression, integration, and exploratory testing
- Identify, document, and track defects through to resolution
- Support release readiness reviews and sign off on deployment criteria
- Communicate testing status and risks to the team and stakeholders

### Typical Interactions / Handoffs
- **Developers:** Review acceptance criteria together before development starts; triage defects and verify fixes; collaborate on test automation strategies
- **Product Managers:** Align on definition of done and acceptance criteria; escalate quality risks that may affect release timelines
- **Project Managers:** Provide test status updates; flag blocking issues; participate in release go/no-go decisions
- **Release Manager:** Supply QA sign-off confirmation and test summary reports before each release
- **UX Designer:** Validate usability requirements and accessibility acceptance criteria during testing

### Artifacts Owned
- Test plans and test case libraries
- QA status reports and defect logs
- Regression test suites (manual and automated)
- Release sign-off and QA handoff documents

### Acceptance Criteria / Signals of Done
- All acceptance criteria for in-scope stories have corresponding test cases
- Test coverage meets or exceeds agreed thresholds
- No open P1/P2 defects at the time of release sign-off
- QA sign-off document completed and shared with Release Manager
- Regression suite executed with results documented

---

## UX Designer / Researcher

### Role Summary
UX Designers and Researchers define user journeys, usability goals, and feedback cycles to ensure the product meets real user needs. They bridge the gap between customer insights and engineering implementation.

### Responsibilities
- Conduct user research, interviews, and usability testing
- Create wireframes, prototypes, and design specifications
- Define and document user journeys and interaction patterns
- Establish usability and accessibility standards for the product
- Facilitate design reviews and iterate based on feedback
- Maintain a design system or component library where applicable

### Typical Interactions / Handoffs
- **Developers:** Hand off design specs and assets; review implemented UI for fidelity; clarify interaction details during development
- **Product Managers:** Co-define user stories and acceptance criteria; share research findings to inform prioritization
- **Project Managers:** Communicate design timelines and dependencies; flag risks when design is blocked or under-resourced
- **QA Engineer:** Define accessibility and usability acceptance criteria; participate in usability testing sessions
- **Business Analyst:** Collaborate on requirements that affect user-facing workflows and data presentation

### Artifacts Owned
- User research reports and usability study summaries
- Wireframes, mockups, and interactive prototypes
- Design specifications and asset libraries
- Accessibility and usability guidelines

### Acceptance Criteria / Signals of Done
- Designs reviewed and approved by Product Manager and key stakeholders before development starts
- Developer handoff package (specs, assets, annotations) delivered
- Usability testing completed with documented findings and resolutions
- Accessibility requirements met (e.g., WCAG 2.1 AA) and verified
- Design system components updated to reflect new patterns

---

## Business Analyst

### Role Summary
Business Analysts clarify requirements, maintain traceability, and bridge the gap between business stakeholders and the technical team. They ensure delivery work maps back to agreed business objectives.

### Responsibilities
- Elicit, document, and refine business and functional requirements
- Maintain requirements traceability from business goals to delivery artifacts
- Facilitate backlog refinement and acceptance criteria definition
- Analyse business processes and identify improvement opportunities
- Produce process models, data flow diagrams, and specification documents
- Support UAT (User Acceptance Testing) coordination and sign-off

### Typical Interactions / Handoffs
- **Developers:** Clarify ambiguous requirements; validate that implementations meet the intent of the specification
- **Product Managers:** Translate strategic goals into actionable requirements; surface conflicts or gaps in the backlog
- **Project Managers:** Provide requirements status and flag scope changes; support change-control documentation
- **QA Engineer:** Co-define acceptance criteria; support test scenario creation from requirements
- **UX Designer:** Align on user-facing requirements and workflows; ensure research insights are captured in specs

### Artifacts Owned
- Business requirements documents (BRDs) and functional specifications
- Traceability matrices
- Process flow diagrams and data models
- UAT plans and sign-off records

### Acceptance Criteria / Signals of Done
- All in-scope requirements documented, reviewed, and baselined before sprint start
- Traceability matrix up to date linking requirements to stories and test cases
- UAT completed with documented stakeholder sign-off
- Change requests assessed and documented before implementation begins
- Requirements reviewed in sprint planning with no unresolved ambiguities

---

## Technical Writer

### Role Summary
Technical Writers maintain user-facing and internal documentation, supporting onboarding, knowledge sharing, and operational transparency across teams. They ensure documentation remains accurate, accessible, and up to date.

### Responsibilities
- Author, edit, and maintain product documentation, API references, and user guides
- Create and update internal process documents and runbooks
- Support onboarding materials for new team members and users
- Review and improve documentation contributed by engineers and other roles
- Coordinate documentation releases to align with product releases
- Establish and maintain documentation standards and style guides

### Typical Interactions / Handoffs
- **Developers:** Review technical accuracy of content; receive updates on API or behaviour changes that require doc updates
- **Product Managers:** Align docs with feature announcements and release notes; incorporate PM feedback on user-facing content
- **Project Managers:** Track documentation tasks in the project plan; ensure doc work is included in release checklists
- **QA Engineer:** Verify that documented procedures match tested behaviour
- **Release Manager:** Confirm release notes are drafted, reviewed, and ready before deployment

### Artifacts Owned
- User guides, API documentation, and product help content
- Internal runbooks, how-to guides, and process documents
- Release notes and changelog entries
- Documentation style guide and content standards

### Acceptance Criteria / Signals of Done
- Documentation reviewed and approved before the associated feature ships
- Release notes drafted and ready at least 48 hours before release
- All new public-facing features have corresponding docs coverage
- Style guide compliance verified for all new or updated content
- Docs repository updated and changes reflected in the published site

---

## Release Manager

### Role Summary
Release Managers oversee the end-to-end release process, ensuring checklists and rollback plans are followed, deployments are coordinated, and stakeholders are kept informed at every stage.

### Responsibilities
- Plan and schedule releases in coordination with engineering and product teams
- Maintain and enforce release readiness checklists and go/no-go criteria
- Coordinate deployment activities and communicate timelines to stakeholders
- Ensure rollback plans are documented and validated before each release
- Track and resolve pre-release blockers; escalate when needed
- Conduct post-release reviews and capture lessons learned

### Typical Interactions / Handoffs
- **Developers:** Confirm code freeze dates; verify build and deployment artefacts; review migration and rollback steps
- **Product Managers:** Align on release scope and timelines; manage scope change requests close to release
- **Project Managers:** Report release status and risks; coordinate cross-team dependencies
- **QA Engineer:** Receive QA sign-off before authorising deployment; review test summary reports
- **Technical Writer:** Confirm release notes and documentation updates are ready before go-live

### Artifacts Owned
- Release plan and deployment schedule
- Release readiness checklist and go/no-go decision record
- Rollback plan documentation
- Post-release review and lessons-learned report

### Acceptance Criteria / Signals of Done
- Release readiness checklist completed and approved by all required parties
- Go/no-go decision documented with sign-off from QA, PM, and engineering leads
- Rollback plan tested and confirmed viable
- Stakeholder communication sent before and after release
- Post-release review completed within 5 business days of deployment

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- When reviewing role ownership during **sprint planning**, confirm that each key deliverable has a clearly identified persona responsible for it.
- During **retrospectives**, use this document to assess whether handoffs between personas went smoothly and identify process improvements.

