# Release Manager Checklist

This checklist provides a lightweight, reusable process for Release Managers to coordinate Patch, Minor, and Major releases.

---

## Pre-Release Phase

### Requirements Validation
- [ ] All acceptance criteria met for features included in this release
- [ ] All PRs merged and code freeze initiated (if applicable)
- [ ] CI/CD pipeline passing (all tests green, security scans clean)
- [ ] Release notes drafted and reviewed

### Stakeholder Alignment
- [ ] Release scope and timeline communicated to stakeholders
- [ ] Deployment window scheduled (if required)
- [ ] On-call and support teams notified of release schedule

### Risk & Readiness Review
- [ ] Rollback plan documented and tested
- [ ] Smoke test plan prepared and reviewed
- [ ] For security-sensitive releases: Security Lead has reviewed and approved
- [ ] Dependencies on external teams or systems confirmed ready

---

## Deployment Phase

### Pre-Deployment
- [ ] Create backup or snapshot of production environment (if applicable)
- [ ] Verify staging environment is up-to-date and healthy
- [ ] Deploy to staging environment

### Staging Verification
- [ ] Run smoke tests on staging
- [ ] Verify key user flows and integrations
- [ ] Confirm monitoring and alerts are functional in staging

### Production Deployment
- [ ] Execute deployment to production (via automated pipeline or manual process)
- [ ] Monitor deployment progress and watch for errors/warnings
- [ ] Confirm services are starting and healthy

---

## Post-Release Phase

### Verification
- [ ] Run post-deploy smoke tests on production
- [ ] Verify key user flows and critical functionality
- [ ] Check monitoring dashboards for anomalies (latency, errors, usage)
- [ ] Confirm no critical alerts or incidents triggered

### Communication & Documentation
- [ ] Announce release completion to stakeholders and support teams
- [ ] Publish release notes to users and internal teams
- [ ] Update project status and close related issues/tickets

### Incident Response (if needed)
- [ ] If deployment fails or causes critical issues:
  - Trigger incident response and notify on-call team
  - Execute rollback plan if necessary
  - Triage root cause and document lessons learned

---

## Release Type Guidance

### Patch Releases
- Focus on hotfixes and critical bug fixes
- Minimize scope and risk
- Fast-track approvals and testing if needed for urgent issues

### Minor Releases
- Include incremental features and improvements
- Follow standard release process
- Coordinate with product and support for feature announcements

### Major Releases
- Significant functionality or breaking changes
- Require extended stakeholder review and communication
- Consider phased rollout or feature flags to reduce risk
- Schedule additional post-release monitoring and support coverage

---

## Tips for Success
- Keep stakeholders informed early and often
- Don't skip smoke tests, even for "small" changes
- Always have a rollback plan ready before deploying
- Document any deviations from the plan for retrospective review
