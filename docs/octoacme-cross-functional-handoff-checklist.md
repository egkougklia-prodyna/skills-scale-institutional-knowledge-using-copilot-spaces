# OctoAcme Cross-Functional Handoff Checklist

This document provides lightweight RACI guidance and checklists for the key handoff moments where multiple roles collaborate. Use these to reduce gaps, prevent missed dependencies, and keep accountability visible.

---

## RACI Key

| Symbol | Meaning |
|--------|---------|
| **R** | Responsible — does the work |
| **A** | Accountable — owns the outcome |
| **C** | Consulted — provides input |
| **I** | Informed — kept up to date |

---

## 1. Feature Scoping & Acceptance Criteria

| Activity | Project Manager | Product Manager | Engineering Manager | Developers | UX Designer | Security Champion | DevOps / SRE | Support Liaison |
|---|---|---|---|---|---|---|---|---|
| Define problem statement | I | A/R | C | C | C | C | I | C |
| Set success metrics | I | A/R | C | I | C | I | I | C |
| Produce UX flows / wireframes | I | C | I | C | A/R | I | I | I |
| Write acceptance criteria | C | A/R | C | C | C | C | I | C |
| Security threat review | I | C | C | C | I | A/R | C | I |
| Capacity / feasibility sign-off | A | C | A/R | C | I | I | C | I |

---

## 2. Sprint / Iteration Start

**Checklist before work begins:**

- [ ] Acceptance criteria are written and approved (Product Manager)
- [ ] UX specs and edge-case flows are finalized and shared (UX Designer)
- [ ] Security requirements are captured in acceptance criteria (Security Champion)
- [ ] Infrastructure and environment dependencies are confirmed ready (DevOps / SRE)
- [ ] Capacity confirmed; team is not over-committed (Engineering Manager)
- [ ] Known support or customer constraints are flagged (Support Liaison)
- [ ] Sprint backlog is prioritized and visible on the project board (Project Manager)

---

## 3. Development → QA / Testing Handoff

**Checklist before moving a story to QA:**

- [ ] All acceptance criteria are implemented and verified by the Developer
- [ ] PR is linked to the relevant issue and acceptance criteria
- [ ] Automated tests are passing in CI
- [ ] Logging, feature flags, and observability instrumentation are in place (Developers + DevOps / SRE)
- [ ] Security-sensitive changes have been reviewed by the Security Champion
- [ ] UX Designer has confirmed interaction spec is met (for UI/UX stories)
- [ ] Known edge cases and out-of-scope items are documented in the PR

---

## 4. QA / Testing → Release Readiness

**Checklist before marking a release candidate ready:**

- [ ] All acceptance criteria verified and sign-off recorded (QA/Testing)
- [ ] Regression suite passed; no open P0/P1 defects (QA/Testing)
- [ ] Rollback plan and runbook confirmed (DevOps / SRE)
- [ ] Monitoring and alerting validated in staging (DevOps / SRE)
- [ ] Security scan completed; critical/high findings resolved (Security Champion)
- [ ] Support documentation and known-issues notes finalized (Support Liaison)
- [ ] Release notes reviewed and approved (Product Manager + Project Manager)
- [ ] Go/no-go decision recorded with rationale (Project Manager)

---

## 5. Release → Post-Release Monitoring

**Checklist within 24–48 hours after deployment:**

- [ ] Production monitors and alerts confirmed active (DevOps / SRE)
- [ ] Initial error-rate and latency baselines reviewed (DevOps / SRE)
- [ ] Customer support channels monitored for spike in related tickets (Support Liaison)
- [ ] Feature flag or rollout percentage reviewed if incremental rollout (DevOps / SRE + Product Manager)
- [ ] Any post-release issues triaged and severity assessed (Project Manager)
- [ ] Quick retro note or "ship log" entry added (Project Manager)

---

## 6. Retrospective → Backlog Loop

| Activity | Project Manager | Product Manager | Engineering Manager | Support Liaison |
|---|---|---|---|---|
| Facilitate retrospective | A/R | C | C | I |
| Summarize action items | A/R | C | C | I |
| Prioritize process improvements | C | A | C | C |
| Add customer-feedback items to backlog | I | A/R | I | R |
| Track action-item follow-through | A/R | C | C | I |

---

## How to use this checklist

- Teams should adapt these checklists to their own project context; remove irrelevant items rather than leaving them unchecked.
- Embed checklist items as GitHub issue templates or PR templates for automated reminders.
- Review and update checklists during retrospectives as processes evolve.
