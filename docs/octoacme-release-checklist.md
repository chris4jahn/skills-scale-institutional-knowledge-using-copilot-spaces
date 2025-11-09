# OctoAcme — Release Checklist

## Purpose
Provide a practical, step-by-step checklist for executing releases consistently and safely. This checklist complements the [Release & Deployment Guide](octoacme-release-and-deployment.md) with actionable steps and clear ownership.

---

## Pre-Release

### Code Readiness
- [ ] All planned features and fixes merged to release branch — **Owner: Developers**
- [ ] All acceptance criteria validated — **Owner: PM, QA**
- [ ] CI/CD pipeline passing (tests, linting, security scans) — **Owner: Developers**
- [ ] Code freeze announced to team — **Owner: Release Manager**

### Documentation & Communication
- [ ] Release notes drafted and reviewed — **Owner: Technical Writer, PM**
- [ ] User-facing documentation updated — **Owner: Technical Writer**
- [ ] API documentation updated (if applicable) — **Owner: Developers, Technical Writer**
- [ ] Known issues documented — **Owner: QA, PM**

### Quality Assurance
- [ ] Smoke tests executed in staging environment — **Owner: QA**
- [ ] Performance and security testing completed — **Owner: QA, Security Champion**
- [ ] Regression testing completed for critical flows — **Owner: QA**
- [ ] Accessibility review completed (if UI changes) — **Owner: UX Designer, QA**

### Release Planning
- [ ] Deployment window scheduled and communicated — **Owner: Release Manager**
- [ ] Rollback plan documented and reviewed — **Owner: Release Manager, Developers**
- [ ] On-call engineer identified and briefed — **Owner: Release Manager**
- [ ] Support team briefed on changes and known issues — **Owner: Customer Support Lead**

---

## Deployment

### Pre-Deployment
- [ ] Backup or snapshot created (if applicable) — **Owner: Release Manager, Developers**
- [ ] Deployment checklist reviewed in go/no-go meeting — **Owner: Release Manager, PM**
- [ ] Final smoke test in staging passed — **Owner: QA**
- [ ] Stakeholders notified of deployment start — **Owner: Release Manager**

### Execute Deployment
- [ ] Deploy to production (automated pipeline preferred) — **Owner: Release Manager, Developers**
- [ ] Monitor deployment logs for errors — **Owner: Release Manager, Developers**
- [ ] Verify deployment completed successfully — **Owner: Release Manager**

### Immediate Verification
- [ ] Run post-deployment smoke tests — **Owner: QA, Release Manager**
- [ ] Check key metrics and dashboards (errors, latency, traffic) — **Owner: Developers**
- [ ] Verify database migrations completed (if applicable) — **Owner: Developers**
- [ ] Confirm critical user flows functional — **Owner: QA**

---

## Post-Release

### Validation & Monitoring
- [ ] Monitor production metrics for anomalies (first 24 hours) — **Owner: Developers, Release Manager**
- [ ] Review error logs and alerts — **Owner: Developers**
- [ ] Confirm no unexpected support escalations — **Owner: Customer Support Lead**
- [ ] Validate success metrics defined in project plan — **Owner: PM**

### Communication
- [ ] Release notes published to users — **Owner: Technical Writer**
- [ ] Release announcement sent to stakeholders — **Owner: Release Manager, PM**
- [ ] Support team notified release is complete — **Owner: Customer Support Lead**
- [ ] Post-release summary shared with team — **Owner: Release Manager**

### Wrap-Up
- [ ] Tag release in version control — **Owner: Release Manager, Developers**
- [ ] Close related issues and update project board — **Owner: PM**
- [ ] Archive release artifacts and logs — **Owner: Release Manager**
- [ ] Schedule post-release retrospective (if needed) — **Owner: PM**

---

## Rollback Decision Guideline

### When to Consider Rollback
- Critical functionality is broken or unavailable
- Significant performance degradation impacting user experience
- Data integrity or security issue detected
- Error rates exceed acceptable thresholds defined in SLOs

### Rollback Decision Process
1. **Assess Impact**: Determine severity and number of users affected
2. **Evaluate Mitigations**: Can the issue be hotfixed quickly without rollback?
3. **Consult Stakeholders**: Brief PM, Release Manager, and on-call engineer
4. **Make Decision**: Go/no-go decision on rollback (Release Manager with PM input)
5. **Execute Rollback**: Follow rollback playbook in [Release & Deployment Guide](octoacme-release-and-deployment.md)
6. **Post-Incident**: Conduct incident review and capture action items

### Rollback Authority
- **Release Manager** has authority to initiate rollback for critical issues
- **PM** should be consulted when feasible, but may be bypassed in time-critical scenarios
- **On-call engineer** can escalate for immediate rollback if Release Manager unavailable

---

## Notes
- Adapt this checklist to your specific release cadence and tooling
- Use project management tools to track checklist completion
- Review and update this checklist during retrospectives to improve the process
