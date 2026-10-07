# OctoAcme Project Management Documentation

## Contents

- [Overview](#overview)
- [Core Principles](#core-principles)
- [Project Lifecycle Phases](#project-lifecycle-phases)
- [Cross-Cutting Guidance](#cross-cutting-guidance)
- [Key Artifacts](#key-artifacts)
- [Core Roles](#core-roles)
- [Getting Started](#getting-started)
- [Questions or Feedback?](#questions-or-feedback)

## Overview

OctoAcme follows a structured, lifecycle-based project management approach designed to deliver customer value through iterative increments with clear governance and accountability. Projects progress through **Initiation**, **Planning**, **Execution**, **Release**, and **Retrospective & Continuous Improvement**. Lightweight artifacts—including the Project One-pager, prioritized backlog, risk register, and release notes—create transparency and support data-informed decisions. Customer-first prioritization, iterative delivery, clear ownership, and psychological safety help teams balance speed with quality and learning.

Three primary roles guide delivery: **Product Managers (PdM)** define what should be built, own the product vision, prioritize the backlog, and measure outcomes; **Project Managers (PM)** coordinate how it is delivered, managing schedules, risks, dependencies, and communications; and **Developers** build features, write tests, and collaborate on design and risk mitigation. QA/testing and stakeholder input complement these responsibilities to maintain clarity and accountability.

Communication and risk management run throughout the lifecycle. The execution guide calls for 15-minute daily standups focused on progress and blockers, weekly delivery syncs, and demos at sprint or milestone boundaries; the overview also allows a team-agreed standup cadence and calls for monthly stakeholder updates. The escalation path is **Team → PM → Product Lead → Sponsor**. Risk registers track ID, description, impact, likelihood, owner, mitigation plan, and status, with weekly reviews. Teams use a GitHub Projects-style board (**Backlog → Ready → In Progress → In Review → QA → Done**), favor small PRs (≤400 lines when possible), run automated tests and linting in CI before review, and require at least one approval before merging (or the team-defined policy).

Quality assurance includes unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows, security scanning in CI, and manual QA when needed to validate acceptance criteria. Before release, acceptance criteria must be met, CI and security scans must pass, release notes must be drafted, and rollback or mitigation plans must be documented. Post-deploy verification and stakeholder announcements close the feedback loop. Retrospectives after sprints, releases, milestones, and incidents turn learning into backlog items or issues with owners and due dates.

## Core Principles

- **Customer-first delivery** — prioritize customer value and usability.
- **Iterative, incremental development** — deliver small, testable increments.
- **Clear ownership and accountability** — name a Project Manager and Product Lead for each project.
- **Data-informed decision making** — measure impact and iterate based on evidence.
- **Psychological safety and learning culture** — encourage feedback and continuous improvement.

## Project Lifecycle Phases

### 1. Initiation

Validate the business need, define measurable outcomes, align stakeholders, and establish a high-level timeline. Create the Project One-pager and initial risk list, then confirm the go/no-go decision for planning.

**Document:** [OctoAcme Project Initiation Guide](./octoacme-project-initiation.md)

### 2. Planning

Define scope, prioritize and estimate the backlog, identify dependencies, agree on the Definition of Done, and establish milestones, a release plan, and an initial QA approach.

**Document:** [OctoAcme Project Planning](./octoacme-project-planning.md)

### 3. Execution & Tracking

Build, test, review, and iterate. Use the project board to track progress, maintain the risk register, demonstrate working increments, and escalate blockers.

**Document:** [OctoAcme Execution & Tracking](./octoacme-execution-and-tracking.md)

### 4. Release & Deployment

Confirm release readiness, prepare release notes and rollback plans, validate in staging, deploy to production, verify the deployment, and announce the release.

**Document:** [OctoAcme Release & Deployment Guide](./octoacme-release-and-deployment.md)

### 5. Retrospective & Continuous Improvement

Capture what went well and what could improve. Prioritize actionable improvements with owners and due dates, track them in the backlog or issues, and review their impact.

**Document:** [OctoAcme Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)

## Cross-Cutting Guidance

Together with the five phase-specific guides above, these links form the complete directory of process documentation:

- **[OctoAcme Project Management Overview](./octoacme-project-management-overview.md)** — introduction to principles, roles, artifacts, lifecycle, and communication cadence.
- **[OctoAcme Risk Management & Communication](./octoacme-risks-and-communication.md)** — identifying, tracking, mitigating, and communicating risks and dependencies, including escalation and status templates.
- **[OctoAcme Roles and Personas](./octoacme-roles-and-personas.md)** — detailed responsibilities, goals, and communication practices for Developers, Product Managers, and Project Managers.

## Key Artifacts

| Artifact | Quick reference | Guide |
| --- | --- | --- |
| Project One-pager / Charter | Problem, goal, success metrics, stakeholders, timeline, risks, and proposed team | [Initiation](./octoacme-project-initiation.md) |
| Risk Register | ID, description, impact, likelihood, owner, mitigation plan, and status; review weekly | [Risk Management & Communication](./octoacme-risks-and-communication.md) |
| Project Board / Prioritized Backlog | Work items with acceptance criteria, priority, estimate, owner, and dependencies; track delivery status | [Planning](./octoacme-project-planning.md), [Execution & Tracking](./octoacme-execution-and-tracking.md) |
| Acceptance Criteria & Definition of Done | Shared expectations for completion and quality | [Planning](./octoacme-project-planning.md) |
| Roadmap / Release Plan | Planned increments, milestones, release timing, and responsibilities | [Planning](./octoacme-project-planning.md) |
| Release Notes / Rollback Plan | Changes, migration steps, known issues, and recovery or mitigation approach | [Release & Deployment](./octoacme-release-and-deployment.md) |
| Retrospective Notes & Action Items | Learnings and prioritized improvements with owners, due dates, and success criteria | [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) |

## Core Roles

| Role | Key responsibilities |
| --- | --- |
| **Project Manager (PM)** | Coordinate delivery, schedules, risks, dependencies, and communications; keep the team aligned and unblocked. |
| **Product Manager (PdM)** | Define product vision and outcomes, prioritize the roadmap and backlog, and measure success. |
| **Developers** | Design and implement features, maintain tests and documentation, review code, and mitigate technical risks. |
| **QA/Testing** | Validate acceptance criteria and quality. |
| **Stakeholders** | Provide input, feedback, and approvals. |

See [Roles and Personas](./octoacme-roles-and-personas.md) for detailed descriptions of the three primary roles and the [Project Management Overview](./octoacme-project-management-overview.md) for the full core role list.

## Getting Started

1. Start with [OctoAcme Project Management Overview](./octoacme-project-management-overview.md) for an introduction.
2. Follow the phase-specific guides in order as your project progresses.
3. Reference [OctoAcme Roles and Personas](./octoacme-roles-and-personas.md) for role clarity.
4. Use [OctoAcme Risk Management & Communication](./octoacme-risks-and-communication.md) throughout all phases.

## Questions or Feedback?

These docs are living artifacts. Contribute improvements, clarifications, or additional guidance through the [Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) issue template.
