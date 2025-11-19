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

## QA / Test Engineering

### Role Summary
QA Engineers ensure quality through test planning, execution, and automation advocacy. They validate acceptance criteria and gate releases when quality standards are not met.

### Responsibilities
- Develop and maintain test plans and test cases
- Execute manual and automated tests
- Report and track defects through resolution
- Participate in acceptance criteria definition
- Advocate for test automation and quality metrics

### Goals
- Prevent defects from reaching production
- Increase test coverage and automation
- Reduce manual testing overhead over time

### Typical Communication
- Test plans and test results shared in sprint reviews
- Defect reports and quality metrics in dashboards
- QA sign-off before release

### Interactions with other roles
- **Developers**: Collaborate on testability, review PRs for test coverage
- **Product Managers**: Validate acceptance criteria and provide quality feedback
- **Project Managers**: Report on quality gates and testing progress
- **Quality Champion**: Partner on test strategy and automation goals

---

## Release Manager

### Role Summary
Release Managers own the end-to-end release process, coordinating deployment activities, verifying release readiness, and ensuring rollback plans are in place.

### Responsibilities
- Coordinate release schedules and deployment windows
- Validate pre-release requirements (tests passed, approvals secured)
- Execute deployment steps and post-release verification
- Manage release notes and communication to stakeholders
- Coordinate with Security Lead for security-sensitive releases

### Goals
- Deliver reliable, low-risk releases
- Minimize production incidents and rollbacks
- Maintain consistent release quality and communication

### Typical Communication
- Release schedules and deployment notifications
- Release notes and change summaries
- Post-release reports and metrics

### Interactions with other roles
- **Project Managers**: Align on release timelines and dependencies
- **Developers**: Coordinate merge deadlines and deployment verification
- **QA**: Confirm testing completion and sign-off
- **Technical Writer**: Collaborate on release notes and user-facing documentation
- **Security Lead**: Review security considerations for each release

---

## Quality Champion

### Role Summary
Quality Champions drive quality culture and practices across the team, owning test strategy, quality gates, and automation advocacy at a program level.

### Responsibilities
- Define test strategy and quality standards for the project
- Establish quality gates and criteria for release blocking
- Champion test automation and CI/CD quality practices
- Track quality metrics (test coverage, defect trends, flakiness)
- Coordinate security scan remediation tracking

### Goals
- Embed quality throughout the development lifecycle
- Increase confidence in releases through robust testing
- Reduce technical debt related to quality

### Typical Communication
- Quality strategy documents and gate definitions
- Quality metrics dashboards and trend analysis
- Recommendations in planning and retrospectives

### Interactions with other roles
- **QA Engineers**: Set strategy and standards, mentor on best practices
- **Developers**: Advocate for testability and automation in design reviews
- **Project Managers**: Define quality gates and communicate quality risks
- **Security Lead**: Ensure security testing is integrated into quality processes

---

## Security Lead

### Role Summary
Security Leads ensure security best practices are followed throughout the project lifecycle, from design to deployment.

### Responsibilities
- Review designs and architectures for security concerns
- Coordinate security scanning and vulnerability remediation
- Define security requirements and acceptance criteria
- Advise on secure coding practices and threat modeling
- Approve security-sensitive releases

### Goals
- Prevent security vulnerabilities in production
- Ensure compliance with security policies and standards
- Build security awareness across the team

### Typical Communication
- Security review findings and recommendations
- Vulnerability scan results and remediation plans
- Security incident post-mortems and lessons learned

### Interactions with other roles
- **Developers**: Provide security guidance and review code for vulnerabilities
- **Release Manager**: Review and approve security-sensitive releases
- **Quality Champion**: Ensure security testing is part of quality strategy
- **Project Managers**: Communicate security risks and timelines for remediation

---

## Technical Writer

### Role Summary
Technical Writers create and maintain user-facing documentation, release notes, and knowledge base articles to support product adoption and usability.

### Responsibilities
- Write and maintain product documentation and user guides
- Collaborate on release notes with Release Manager and PM
- Create tutorials, FAQs, and troubleshooting guides
- Ensure documentation accuracy and consistency
- Participate in early design reviews to scope documentation needs

### Goals
- Make products easy to understand and use
- Reduce support burden through clear documentation
- Maintain up-to-date, accurate documentation

### Typical Communication
- Documentation drafts for review by subject matter experts
- Release note content and user-facing announcements
- Documentation plan and scope during project planning

### Interactions with other roles
- **Product Managers**: Understand product vision and user needs
- **Developers**: Clarify technical details and implementation specifics
- **Release Manager**: Co-author release notes and deployment communications
- **UX Designer**: Align documentation with user experience and workflows

---

## UX Designer

### Role Summary
UX Designers ensure products are intuitive, accessible, and delightful by conducting user research and creating design solutions that meet user needs.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, mockups, and prototypes
- Define design systems and interaction patterns
- Collaborate on acceptance criteria for UX requirements
- Provide design handoff artifacts (specs, assets, prototypes)

### Goals
- Deliver user-centered design solutions
- Improve product usability and accessibility
- Maintain design consistency across features

### Typical Communication
- Design reviews and critique sessions
- Research findings and usability reports
- Design handoff documentation for developers

### Interactions with other roles
- **Product Managers**: Validate problem statements and user needs through research
- **Developers**: Provide design specs and collaborate on implementation feasibility
- **Technical Writer**: Ensure documentation aligns with designed user workflows
- **Project Managers**: Communicate design timeline and dependencies

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

