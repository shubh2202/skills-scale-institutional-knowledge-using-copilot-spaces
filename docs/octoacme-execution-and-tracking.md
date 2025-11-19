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

### Quality Champion Responsibilities
The **Quality Champion** owns the test strategy and quality standards for the project:
- Defines test-plan ownership and ensures coverage across unit, integration, and E2E tests
- Establishes quality gates: criteria that must be met before a release proceeds
- Advocates for test automation and monitors quality metrics (coverage, flakiness, defect trends)
- Coordinates with **Security Lead** to track security scan remediation and integrate security testing into CI/CD

### QA Gating Guidance
Quality gates should block a release when:
- Critical or high-severity defects remain unresolved
- Test coverage falls below agreed thresholds
- Automated tests are failing or flaky without investigation
- Security vulnerabilities are unaddressed

If a release is blocked, the Quality Champion escalates to the Project Manager and stakeholders with a clear remediation plan and timeline.

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
