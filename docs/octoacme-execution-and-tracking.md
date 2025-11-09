# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Role Interactions During Execution

This section maps personas to key execution activities to clarify expectations and improve coordination.

### Daily Standups
- **Developers**: Share progress, blockers, and dependencies
- **PM**: Prioritize blockers and adjust scope if needed
- **Project Manager**: Track progress against plan and identify risks
- **QA/Customer Support Lead**: Escalate critical bugs or user-impacting issues
- **UX Designer**: Update on design progress and coordinate with Developers on implementation

### Pull Request Reviews
- **Developers**: Author PRs with clear descriptions, review peers' code for quality and correctness
- **Security Champion**: Review PRs for security vulnerabilities and best practices
- **Technical Writer**: Review PRs that affect user-facing features or APIs for documentation needs
- **Project Manager**: Monitor PR velocity and flag bottlenecks

### QA Handoffs
- **Developers**: Mark features ready for QA with acceptance criteria and test guidance
- **QA**: Execute test plans, document bugs, and validate fixes
- **PM**: Validate feature meets acceptance criteria and user needs
- **UX Designer**: Validate design implementation and user flows
- **Customer Support Lead**: Review features from support perspective and prepare support materials

### Incident Response
- **Developers**: Triage and fix production issues, coordinate with on-call
- **Release Manager**: Coordinate rollback decisions and communicate with stakeholders
- **Customer Support Lead**: Communicate with affected users and gather impact details
- **Security Champion**: Lead response for security incidents, coordinate remediation
- **PM**: Make prioritization decisions on incident fixes vs. planned work

### Retrospectives
- **All team members**: Reflect on what went well, what didn't, and action items
- **Project Manager**: Facilitate retrospective and track action items
- **PM**: Share outcomes data and prioritize process improvements
- **Release Manager**: Review release process effectiveness
- **Technical Writer**: Share documentation feedback and improvement ideas

---

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
