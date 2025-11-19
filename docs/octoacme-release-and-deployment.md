# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Manager Ownership
The **Release Manager** coordinates all release activities, ensuring readiness, executing deployments, and verifying post-release health. They work closely with developers, QA, and stakeholders to maintain release quality and communication.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

For a detailed, reusable checklist covering pre-release, deployment, and post-release activities, see [Release Manager Checklist](templates/release-manager-checklist.md).

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:

### Release Notes Ownership
Release notes are collaboratively authored by:
- **Technical Writer**: Drafts user-facing content and formatting
- **Release Manager**: Ensures completeness and coordinates review
- **Product Manager**: Approves messaging and highlights customer value

## Security Considerations
For security-sensitive releases (e.g., vulnerability fixes, authentication changes):
- **Security Lead** reviews release plan and approves deployment timing
- Consider staggered rollout or feature flags to limit blast radius
- Coordinate with security team on disclosure timing if applicable
- Include security-specific verification steps in post-deploy checks
