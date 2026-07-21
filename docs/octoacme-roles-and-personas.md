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

## Engineering Manager

### Role Summary
Engineering Managers own team health, technical delivery capacity, and execution reliability. They bridge engineering teams and product/project leadership to ensure staffing, quality, and pace align with roadmap commitments.

### Responsibilities
- Align staffing and capacity to roadmap commitments
- Remove execution blockers escalated by Project Managers and Developers
- Coach engineers on quality, delivery practices, and career growth
- Partner with Product Managers and Project Managers on scope and sequencing trade-offs
- Manage headcount, onboarding, and cross-team dependencies

### Goals
- Maintain a healthy, high-performing delivery team
- Ensure sustainable pace and reduce unplanned interruptions
- Build engineering capability that scales with product ambition

### Typical Communication
- Weekly capacity and risk alignment with Project Manager
- Feasibility and sequencing discussions with Product Manager
- 1:1s and team retros with Developers
- Escalation paths for blockers that cross team boundaries

### Interactions with Existing Roles
- **Project Manager:** Weekly syncs on capacity, risks, and milestone commitments; joint escalation decisions.
- **Product Manager:** Trade-off conversations on scope, schedule, and technical feasibility.
- **Developers:** Mentorship, workload oversight, and delivery support; shields team from unplanned context-switching.

---

## UX Designer / Researcher

### Role Summary
UX Designers and Researchers ensure solutions are usable, accessible, and validated with real users before and after build. They translate customer insights into clear interaction specifications that guide development.

### Responsibilities
- Produce user flows, wireframes, and interaction specifications
- Run lightweight user validation sessions and synthesize findings
- Define usability acceptance inputs before development begins
- Collaborate on post-release behavior analysis to inform iteration
- Maintain a shared design system and accessibility standards

### Goals
- Deliver experiences that are intuitive and meet user needs
- Reduce rework caused by late-stage usability discoveries
- Ensure accessibility and inclusive design across features

### Typical Communication
- Problem-framing sessions and design reviews with Product Manager
- Edge-case and interaction detail discussions with Developers
- Usability scenario handoffs to QA/Testing
- Design critiques and research readouts with cross-functional team

### Interactions with Existing Roles
- **Product Manager:** Refine problem framing, validate success criteria, and align on user research findings.
- **Developers:** Clarify edge cases, interaction details, and responsive/accessibility requirements during build.
- **Project Manager:** Flag design dependency timelines and flag scope changes affecting UX milestones.

---

## DevOps / SRE

### Role Summary
DevOps Engineers and Site Reliability Engineers own release reliability, observability, and operational readiness. They ensure deployments are safe, reversible, and supported by monitoring and runbooks.

### Responsibilities
- Maintain CI/CD pipelines and deployment safeguards
- Define monitoring, alerting, and runbook expectations for each release
- Validate rollback readiness and incident response paths before go-live
- Track reliability indicators (error rates, latency, uptime) after releases
- Manage environment provisioning and infrastructure-as-code practices

### Goals
- Achieve high deployment frequency with low change-failure rate
- Reduce mean time to recovery (MTTR) for production incidents
- Build observability that gives teams fast, accurate production signals

### Typical Communication
- Release planning and risk review with Project Manager
- Production-readiness and instrumentation discussions with Developers
- Environment and smoke-test coordination with QA/Testing
- Post-incident reviews and action-item tracking

### Interactions with Existing Roles
- **Project Manager:** Participate in release planning gates; flag infrastructure risks and deployment window constraints.
- **Developers:** Review production-readiness checklists, logging/tracing requirements, and feature-flag configurations.
- **Product Manager:** Communicate operational constraints that affect release scope or timing.

---

## Security Champion

### Role Summary
Security Champions embed security practices into planning and delivery. They advise on threat and risk considerations, enforce secure coding checkpoints, and support incident response for security-related events.

### Responsibilities
- Advise on threat modeling and risk considerations for new features
- Ensure secure coding practices and dependency hygiene checkpoints throughout the sprint
- Support incident communication and remediation for security-related events
- Partner with Project Manager and Product Manager on remediation prioritization
- Stay current on vulnerability disclosures affecting the product's dependencies

### Goals
- Prevent security vulnerabilities from reaching production
- Shorten the time to detect and remediate identified risks
- Build a security-aware culture across the delivery team

### Typical Communication
- Security requirements reviews during sprint planning with Product Manager
- Secure implementation pattern guidance with Developers
- Escalation and compliance communication with Project Manager
- Periodic threat model updates and security retrospective notes

### Interactions with Existing Roles
- **Product Manager:** Define security requirements as part of acceptance criteria; prioritize remediation items on the backlog.
- **Developers:** Provide secure implementation patterns, review code for vulnerabilities, and advise on dependency choices.
- **Project Manager:** Escalate security risks that affect timeline or compliance; coordinate external disclosure communications.

---

## Customer Support / Success Liaison

### Role Summary
Customer Support and Success Liaisons connect customer-facing feedback to delivery priorities. They aggregate recurring pain points, prepare support teams for releases, and feed post-release sentiment back into the backlog.

### Responsibilities
- Aggregate and synthesize recurring customer pain points and feature requests
- Provide release readiness input—known issues, FAQ updates, and support playbooks—for support teams
- Validate support documentation and known-issue notes before go-live
- Feed post-release customer sentiment and ticket trends back into the product backlog
- Reproduce and document customer-reported defects for engineering triage

### Goals
- Reduce customer-facing incidents caused by unaddressed feedback loops
- Ensure support teams are prepared and informed before every release
- Build a tight feedback cycle between customer experience and product decisions

### Typical Communication
- Prioritization syncs with Product Manager on high-impact customer issues
- Rollout risk and readiness briefings with Project Manager
- Defect reproduction and triage sessions with Developers and QA/Testing
- Post-release sentiment reports and ticket trend summaries

### Interactions with Existing Roles
- **Product Manager:** Surface and prioritize high-impact customer issues; validate that release notes address key pain points.
- **Project Manager:** Communicate support readiness risks and confirm go-live checklist items affecting customer-facing teams.
- **Developers / QA:** Assist in reproducing customer-reported defects and validating fixes against real-world scenarios.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

