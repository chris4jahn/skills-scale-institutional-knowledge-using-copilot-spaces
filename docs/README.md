# OctoAcme Project Management Docs

Welcome to the OctoAcme Project Management documentation! This guide provides a comprehensive overview of our project management processes, roles, and best practices.

## Overview

OctoAcme runs projects with an iterative, outcome-oriented lifecycle that emphasizes customer value, clear ownership, and data-informed decisions. Our approach moves work through distinct phases:

- **Initiation**: Validate the problem using a Project One-pager, align stakeholders, define success metrics, and make go/no-go decisions
- **Planning**: Break work into shippable increments, create prioritized backlogs, identify dependencies and risks, and map releases
- **Execution & Tracking**: Deliver small increments on a project board using short feedback cycles and continuous quality practices
- **Risk & Communication**: Manage risks proactively with a risk register and maintain clear stakeholder communication
- **Release & Deployment**: Follow standardized deployment checklists with rollback plans and post-deploy verification
- **Retrospective**: Capture learnings and convert them into actionable improvements for continuous growth

Our workflow emphasizes rapid visibility, predictable handoffs, small PRs linked to issues, automated CI checks, and formalized quality practices. Metrics like velocity and burndown, combined with regular retrospectives, drive continuous improvement.

## Core Roles

### Project Manager (PM)

Project Managers coordinate delivery activities, manage schedules, risks, and communications to enable efficient team delivery.

**Key Responsibilities:**
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

**Goals:** Deliver projects on time and within scope, minimize unplanned work, maintain transparency and alignment.

### Product Manager (PdM)

Product Managers define what should be built to deliver customer and business value, own the product vision, and measure outcomes.

**Key Responsibilities:**
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

**Goals:** Maximize customer value and impact, make clear data-driven prioritization decisions, ensure product-market fit.

### Developer

Developers design, build, test, and deliver software components while collaborating with product and project leads.

**Key Responsibilities:**
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

**Goals:** Deliver reliable, maintainable code, reduce cycle time, maintain high test coverage and observability.

## Documentation

Explore our complete project management guides:

1. [**Project Management Overview**](./octoacme-project-management-overview.md) — Core principles, roles, artifacts, lifecycle, and communication cadence
2. [**Project Initiation**](./octoacme-project-initiation.md) — Validate and authorize work, align stakeholders, create project one-pagers
3. [**Project Planning**](./octoacme-project-planning.md) — Turn initiatives into actionable plans, create backlogs, and define Definition of Done
4. [**Execution & Tracking**](./octoacme-execution-and-tracking.md) — Day-to-day execution, team rhythm, workflows, quality practices, and metrics
5. [**Risk Management & Communication**](./octoacme-risks-and-communication.md) — Identify, manage, and communicate risks; stakeholder communication templates
6. [**Release & Deployment**](./octoacme-release-and-deployment.md) — Standardize releases, deployment checklists, rollback plans, and incident playbooks
7. [**Retrospective & Continuous Improvement**](./octoacme-retrospective-and-continuous-improvement.md) — Capture learnings and create actionable improvements
8. [**Roles & Personas**](./octoacme-roles-and-personas.md) — Detailed role definitions for Developers, Product Managers, and Project Managers

## How to Use These Docs

**For New Team Members:**
- Start with the [Project Management Overview](./octoacme-project-management-overview.md) to understand our approach
- Review [Roles & Personas](./octoacme-roles-and-personas.md) to understand your responsibilities and how you collaborate with others
- Reference specific guides as needed during each project phase

**For Project Execution:**
- Keep the Project Charter/One-pager updated in your project repository
- Follow the relevant process guides for your current project phase
- Use the checklists in each guide to ensure you don't miss critical steps

**For GitHub Copilot Spaces:**
- Add relevant process docs to your `.copilot/` directory so Copilot Spaces can use them as context for project-specific guidance
- Reference these docs in your Copilot Space prompts when you need process-related assistance

## Updating These Docs

These process docs should evolve based on team feedback and learnings:

- **Small Updates**: Submit a PR with your proposed changes and context for the update
- **Major Changes**: Open an issue first to discuss the change with stakeholders before implementing
- **After Retrospectives**: If a retrospective identifies a process improvement, update the relevant doc and link the action item

Keep documentation concise, actionable, and grounded in actual team practices.

---

*This README addresses issue #2 and provides a central entry point for all OctoAcme project management documentation.*
