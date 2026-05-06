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

## QA / Test Engineer

### Role Summary
QA / Test Engineers own the quality assurance strategy and execution across the delivery lifecycle. They design test plans, execute manual and automated tests, and act as the final quality gate before any release.

### Responsibilities
- Design and maintain test plans, test cases, and automated test suites
- Execute functional, regression, integration, and exploratory testing
- Track and triage defects; validate bug fixes before closure
- Define and uphold the Definition of Done and acceptance criteria validation
- Contribute to release readiness assessments and sign-off decisions
- Identify and document quality risks early in the planning cycle

### Goals
- Prevent defects from reaching production
- Enable fast, confident releases through reliable automation
- Provide objective quality signals to the team and stakeholders

### Typical Communication
- Daily standups and sprint reviews
- Bug reports and test result summaries
- Release readiness sign-off in the release checklist

### Interactions with Existing Roles
- **Developers**: Review acceptance criteria together; QA unblocks devs by clarifying test coverage gaps and validating fixes quickly.
- **Product Managers**: Align on acceptance criteria and edge cases; QA flags scope-impacting quality risks.
- **Project Managers**: Report test progress and defect trends in weekly status updates; flag blockers that affect release timelines.
- **Release Manager**: Provide formal sign-off or raise blockers in the release readiness checklist before any deployment.
- **Tech Lead**: Collaborate on test automation architecture and tooling decisions.

---

## UX Designer / Researcher

### Role Summary
UX Designers and Researchers champion the user perspective throughout the product lifecycle. They translate user needs and business goals into intuitive, accessible experiences, and validate designs through research.

### Responsibilities
- Conduct user research (interviews, usability studies, surveys) to inform design decisions
- Create wireframes, prototypes, and design specifications
- Maintain a consistent design system and accessibility standards
- Collaborate on acceptance criteria to include usability requirements
- Present research findings to stakeholders and the product team
- Iterate designs based on user feedback and analytics

### Goals
- Deliver experiences that are intuitive, accessible, and valued by users
- Reduce rework by validating design decisions before development begins
- Ensure user perspectives inform roadmap and prioritization decisions

### Typical Communication
- Design reviews and critiques with Product and Engineering
- Research readouts to stakeholders and Product Managers
- Annotated design specs shared with Developers
- Usability test reports during and after releases

### Interactions with Existing Roles
- **Product Managers**: Co-own the user problem statement; translate business requirements into user stories with usability acceptance criteria.
- **Developers**: Provide detailed design specs and answer implementation questions; review built UIs against design intent before QA.
- **QA / Test Engineers**: Collaborate on usability test cases; QA checks UI against design specs during testing.
- **Project Managers**: Flag design dependencies and research timelines that affect project scheduling.
- **Stakeholders**: Present research findings and design proposals to gain alignment and approval.

---

## Tech Lead / Engineering Lead

### Role Summary
The Tech Lead provides technical direction and architectural leadership for the delivery team. They bridge engineering concerns with product priorities, ensuring technical quality, scalability, and maintainability of delivered work.

### Responsibilities
- Own technical architecture decisions and document them in decision logs
- Set and enforce coding standards, review practices, and engineering best practices
- Break down complex technical work and support developer estimates
- Identify and mitigate technical risks and dependencies
- Facilitate technical design reviews and cross-team engineering alignment
- Partner with Security Lead on secure-by-design practices
- Mentor developers and grow technical capability on the team

### Goals
- Deliver technically sound, scalable, and maintainable systems
- Reduce technical debt and unplanned work through proactive design
- Align engineering velocity with product delivery goals

### Typical Communication
- Technical design docs and Architecture Decision Records (ADRs)
- Code review feedback and engineering sync meetings
- Risk and dependency entries in the RAID log
- Escalation to Project Manager when technical blockers affect timelines

### Interactions with Existing Roles
- **Developers**: Direct partner in daily technical decisions; provides guidance, unblocks, and reviews work.
- **Product Managers**: Translate technical constraints into terms the product team can use for prioritization.
- **Project Managers**: Surface technical risks, timeline impacts, and resource needs; co-own the RAID log.
- **Security Lead**: Collaborate on threat modelling and secure design before implementation begins.
- **QA / Test Engineers**: Define testability requirements and support automation architecture.
- **Release Manager**: Confirm technical readiness and deployment approach before releases.

---

## Security Lead

### Role Summary
The Security Lead owns the security posture of delivered products and systems. They embed security practices throughout the development lifecycle (DevSecOps), lead incident response for security events, and ensure the team meets regulatory and compliance requirements.

### Responsibilities
- Conduct threat modelling and security reviews during planning and design phases
- Define and champion secure coding standards and DevSecOps tooling (SAST, DAST, dependency scanning)
- Review and approve security-sensitive architecture decisions
- Own the security escalation path and incident response runbook
- Coordinate with external auditors, compliance teams, and legal as needed
- Track and prioritize security vulnerabilities in the risk register

### Goals
- Prevent security vulnerabilities from reaching production
- Enable fast response and containment when security incidents occur
- Build a culture of security awareness across the engineering team

### Typical Communication
- Security review sign-off in the release readiness checklist
- Security incident communications following the incident comms template
- Risk register entries for open vulnerabilities
- Periodic security briefings to stakeholders and leadership

### Interactions with Existing Roles
- **Tech Lead**: Co-lead threat modelling and architecture reviews; agree on security controls integrated into the development workflow.
- **Developers**: Provide secure coding guidance; review code for security issues and advise on remediations.
- **Project Managers**: Log security risks in the RAID log; surface timeline impacts when security issues must be resolved before release.
- **Release Manager**: Provide security sign-off in the release readiness checklist; raise blockers when vulnerabilities are unresolved.
- **QA / Test Engineers**: Coordinate security test cases (penetration tests, OWASP checks) as part of the test plan.
- **Site Reliability / Operations**: Collaborate on incident detection, response, and post-incident review for security events.

---

## Release Manager

### Role Summary
The Release Manager orchestrates the end-to-end release process, ensuring that all readiness criteria are met and that deployments occur safely, predictably, and with clear communication to all stakeholders.

### Responsibilities
- Own the release calendar and coordinate release windows with all involved teams
- Facilitate the release readiness checklist and go/no-go decision gate
- Coordinate deployment activities across Engineering, Ops, and QA
- Communicate release status, scope, and rollback plans to stakeholders
- Maintain the release notes and post-deployment verification process
- Lead post-release retrospectives for release process improvement

### Goals
- Achieve zero-surprise releases through clear preparation and communication
- Minimize production incidents caused by deployment issues
- Build a repeatable, low-friction release process

### Typical Communication
- Release readiness checklist and go/no-go meeting agenda
- Release notes and deployment announcements
- Post-deployment status updates to stakeholders
- Escalation to leadership if a release must be delayed or rolled back

### Interactions with Existing Roles
- **Project Managers**: Align release dates with project milestones; coordinate schedule changes and stakeholder communications.
- **Developers / Tech Lead**: Confirm code freeze, deployment steps, feature flags, and rollback procedures.
- **QA / Test Engineers**: Obtain test sign-off and verify that all acceptance criteria are met before go/no-go.
- **Security Lead**: Ensure security sign-off is included in the release readiness checklist.
- **Site Reliability / Operations**: Coordinate deployment execution and monitoring during and after release.
- **Product Managers**: Agree on release scope and ensure release notes accurately reflect delivered value.

---

## Site Reliability / Operations

### Role Summary
Site Reliability Engineers (SREs) and Operations staff ensure that systems are reliable, performant, and observable in production. They partner with engineering to build operational readiness into products from the start.

### Responsibilities
- Define and monitor Service Level Objectives (SLOs) and Service Level Indicators (SLIs)
- Manage infrastructure, deployment pipelines, and operational tooling
- Own incident response runbooks and lead incident management for operational events
- Conduct post-incident reviews (PIRs) and drive systemic improvements
- Review architectures for operational readiness, scalability, and observability
- Collaborate with Engineering on on-call rotation and escalation paths

### Goals
- Achieve and maintain agreed reliability and availability targets
- Reduce mean time to detect (MTTD) and mean time to recover (MTTR) for incidents
- Eliminate toil through automation and operational improvements

### Typical Communication
- Incident reports and post-incident review (PIR) documents
- SLO/SLI dashboards shared with stakeholders
- Operational readiness reviews before releases
- On-call handoffs and incident comms during active incidents

### Interactions with Existing Roles
- **Tech Lead**: Review infrastructure and architecture designs for operability, scalability, and observability requirements.
- **Release Manager**: Execute and monitor deployments; provide operational sign-off in the release readiness checklist.
- **Security Lead**: Collaborate on security incident detection and response; contribute to operational security controls.
- **Project Managers**: Surface operational risks and infrastructure dependencies in the RAID log.
- **Developers**: Partner on observability (logging, metrics, tracing) and on-call readiness standards.

---

## Customer Support / Success

### Role Summary
Customer Support and Customer Success roles act as the voice of the customer within the project team. They surface real-world feedback, help prioritize post-launch issues, and ensure customers derive value from delivered features.

### Responsibilities
- Collect and synthesize customer feedback, bug reports, and feature requests
- Triage and escalate critical customer-impacting issues to Engineering and Product
- Contribute customer impact assessments to the risk register and prioritization decisions
- Communicate product changes and known issues to customers proactively
- Partner with QA on user acceptance testing (UAT) and edge case identification
- Provide input to release notes and customer-facing documentation

### Goals
- Ensure customers are aware of changes that affect them
- Reduce customer churn and escalations through proactive communication and quality
- Close the feedback loop between customers and the product team

### Typical Communication
- Customer escalation reports and impact summaries
- Input to release notes and customer announcements
- Feedback sessions with Product Managers and UX Researchers
- Post-release customer satisfaction assessments

### Interactions with Existing Roles
- **Product Managers**: Share customer feedback and escalations to inform backlog prioritization and roadmap decisions.
- **QA / Test Engineers**: Provide customer-reported test scenarios and participate in UAT.
- **Release Manager**: Review customer-facing release notes before publication; flag customer-impacting rollback scenarios.
- **Project Managers**: Escalate critical customer issues that require schedule or scope adjustments.
- **UX Designer / Researcher**: Partner on user research and usability feedback collection.

---

## Stakeholder / Sponsor

### Role Summary
Stakeholders and Sponsors provide strategic direction, funding, and organizational authority for projects. They serve as the decision-makers for significant scope, budget, or strategic changes, and are accountable for project outcomes at the business level.

### Responsibilities
- Approve project charters, business cases, and major scope changes
- Provide timely input at decision gates (initiation, planning, release approval)
- Remove organizational blockers that are beyond the Project Manager's authority
- Maintain awareness of project health through regular status updates
- Champion the project within the wider organization

### Goals
- Ensure projects deliver measurable business value
- Maintain strategic alignment between projects and organizational priorities
- Enable fast decisions to unblock delivery

### Typical Communication
- Monthly stakeholder status briefings and milestone updates
- Decision gate approvals (charter sign-off, go/no-go for release)
- Escalation notifications when risks materialize or scope changes are required
- Post-project retrospective summary and outcomes review

### Interactions with Existing Roles
- **Project Managers**: Primary day-to-day point of contact; PMs escalate blockers and decisions to Sponsors.
- **Product Managers**: Align on strategic priorities; Sponsors provide business context for roadmap trade-offs.
- **Security Lead**: Receive briefings on high-severity security risks that require executive action or regulatory reporting.
- **Tech Lead**: Engage on significant architecture decisions that have strategic or financial implications.
- **Release Manager**: Provide final go/no-go approval authority for high-stakes or customer-impacting releases.

---

## Change Manager

### Role Summary
The Change Manager owns the organizational change management (OCM) process for projects that introduce significant process, technology, or behavioural changes. They ensure that people-side impacts are assessed, communicated, and managed so that changes are adopted successfully and sustainably.

### Responsibilities
- Assess the people-side impact of proposed changes and document a change impact analysis
- Develop and execute change management plans, including communications, training, and stakeholder engagement strategies
- Identify and manage resistance to change; surface adoption risks early
- Coordinate change rollouts with Release Managers and Project Managers to align technical and human timelines
- Collect and synthesize feedback from affected stakeholders during and after change rollouts
- Establish and track adoption metrics to measure change success

### Goals
- Achieve high adoption rates and minimize productivity disruption during transitions
- Ensure all affected stakeholders understand the change, its rationale, and their role in it
- Build organizational change capability and resilience over time

### Typical Communication
- Change impact assessments and stakeholder engagement plans
- Change communications distributed to affected teams before and during rollouts
- Adoption progress reports to Project Managers and Sponsors
- Post-rollout surveys and lessons-learned summaries

### Interactions with Existing Roles
- **Project Managers (PM)**: Co-own change timelines; PM handles delivery scheduling while Change Manager handles people readiness. Surface adoption risks in the RAID log.
- **Product Managers (PdM)**: Align on the user impact of product changes; provide change management input to feature release communications.
- **Tech Lead / Engineering Lead**: Understand technical changes deeply enough to translate them into plain-language impact summaries for affected users.
- **Release Manager**: Coordinate change communications to align with deployment windows; ensure user-facing announcements accompany technical deployments.
- **Customer Support / Success**: Brief Support on upcoming changes so they can prepare for customer questions; incorporate Support feedback into change readiness assessments.
- **Stakeholders / Sponsors**: Provide regular adoption metrics and escalate risks requiring executive sponsorship or resource decisions.
- **UX Designer / Researcher**: Leverage user research to inform change impact analysis and training material design.

---

## Data Analyst

### Role Summary
The Data Analyst provides actionable insights from project and product data to support evidence-based decision-making. They partner with product and engineering teams to define metrics, build reports, and surface trends that drive continuous improvement.

### Responsibilities
- Define, instrument, and maintain key performance indicators (KPIs) and success metrics for projects and products
- Build and maintain dashboards, reports, and ad-hoc analyses that are accessible to the wider team
- Conduct root-cause investigations for metric anomalies, quality issues, or unexpected outcomes
- Support A/B test design, execution, and interpretation
- Validate data quality and flag data integrity issues to engineering
- Translate data insights into clear recommendations for stakeholders and product teams

### Goals
- Enable data-driven prioritization and decision-making across all roles
- Reduce time-to-insight for project and product health monitoring
- Ensure decisions are grounded in reliable, well-understood data

### Typical Communication
- Dashboard links and automated metric reports shared with the team
- Analysis write-ups and insight summaries delivered to Product Managers and Stakeholders
- Data quality incident reports to Engineering and QA
- A/B test results and experiment readouts

### Interactions with Existing Roles
- **Product Managers (PdM)**: Collaborate on success metric definitions and roadmap prioritization; provide data to validate hypotheses and measure feature impact.
- **Project Managers (PM)**: Supply project health metrics and trend data for status reports and risk assessments.
- **Tech Lead / Engineering Lead**: Work together on instrumentation requirements, data pipeline reliability, and analytics architecture decisions.
- **QA / Test Engineers**: Share data anomaly findings that may indicate defects; collaborate on metrics for test coverage and quality trends.
- **Stakeholders / Sponsors**: Deliver executive-level reporting on business outcomes and project ROI.
- **Security Lead**: Ensure data handling practices comply with data privacy and security requirements; flag any analytics instrumentation that touches sensitive data.
- **UX Designer / Researcher**: Combine quantitative analytics with qualitative research to build a holistic picture of user behaviour.

---

## Legal / Compliance Advisor

### Role Summary
The Legal / Compliance Advisor ensures that all project deliverables, processes, and third-party relationships adhere to applicable legal, regulatory, and organizational compliance requirements. They are engaged proactively rather than reactively to reduce risk and accelerate delivery.

### Responsibilities
- Review contracts, vendor agreements, open-source licenses, and intellectual property (IP) considerations for project work
- Identify applicable regulatory frameworks (e.g., GDPR, HIPAA, SOC 2, accessibility standards) and translate requirements into actionable controls
- Participate in architecture and design reviews where data handling, privacy, or compliance controls are at stake
- Advise on acceptable use policies, terms of service, and content moderation requirements
- Maintain a compliance register and escalate unresolved compliance risks to Sponsors
- Provide guidance on incident disclosure obligations and coordinate with external regulators when required

### Goals
- Prevent legal and compliance issues from blocking releases or creating organizational liability
- Ensure the team has clear, actionable guidance on compliance requirements early in the project lifecycle
- Build a culture of proactive compliance rather than reactive remediation

### Typical Communication
- Compliance review sign-off in the release readiness checklist for regulated features or changes
- Legal risk entries in the RAID log
- Compliance briefings to Stakeholders and the Security Lead
- Guidance documents and FAQs shared with the wider team

### Interactions with Existing Roles
- **Security Lead**: Co-own compliance controls that overlap with security requirements (e.g., data encryption, access controls, audit logging). Coordinate on security incident disclosure obligations.
- **Product Managers (PdM)**: Advise on compliance constraints that affect roadmap decisions and feature design (e.g., data retention, consent flows).
- **Tech Lead / Engineering Lead**: Review technical architectures for privacy-by-design and compliance-by-design requirements; advise on permissible open-source license usage.
- **Release Manager**: Provide compliance sign-off in the release readiness checklist for changes that affect regulated data or user-facing legal terms.
- **Project Managers (PM)**: Log compliance risks in the RAID log; flag when regulatory timelines create project constraints.
- **Stakeholders / Sponsors**: Escalate unresolved legal risks or regulatory actions requiring executive decisions or external engagement.
- **Data Analyst**: Review analytics instrumentation for data privacy compliance (e.g., PII handling, consent requirements).

---

## Community Manager

### Role Summary
The Community Manager builds and nurtures relationships with the external user and developer community surrounding OctoAcme products. They act as the two-way bridge between the community and the internal team, surfacing external insights while ensuring the community has a positive, informed experience.

### Responsibilities
- Manage and moderate public communication channels (forums, social media, community platforms, developer portals)
- Gather, synthesize, and prioritize community feedback and feature requests for the product team
- Create and publish community-facing content including announcements, release highlights, tutorials, and FAQs
- Identify and respond to emerging community sentiment, including risks or reputational concerns
- Build relationships with power users, advocates, and community contributors
- Coordinate beta programmes and early-access feedback loops with Product Managers

### Goals
- Build a healthy, engaged community that advocates for and contributes to the product
- Ensure the community is informed and prepared for product changes before they occur
- Surface external insights and risks that the internal team would otherwise miss

### Typical Communication
- Community announcements and release notes published on public channels
- Feedback digests and sentiment reports shared with Product Managers and Project Managers
- Community risk escalations to Stakeholders when public issues emerge
- Coordination with Release Manager on the timing and messaging of public release communications

### Interactions with Existing Roles
- **Product Managers (PdM)**: Deliver regular community feedback digests to inform backlog prioritization; co-own beta programmes and early-access initiatives.
- **Customer Support / Success**: Coordinate on customer-impacting issues that surface in community channels; share escalation paths and ensure consistent messaging.
- **Release Manager**: Align public-facing community announcements with deployment timing; review community-facing release notes before publication.
- **UX Designer / Researcher**: Partner on community-based user research and usability feedback collection.
- **Project Managers (PM)**: Flag community-sourced risks (e.g., reputational issues, breaking change concerns) for inclusion in the RAID log.
- **Security Lead**: Escalate security-related community disclosures (e.g., public vulnerability reports) through proper channels immediately.
- **Stakeholders / Sponsors**: Escalate community escalations that carry reputational or strategic implications requiring executive response.

---

## AI / ML Lead

### Role Summary
The AI / ML Lead provides technical and ethical leadership for projects that design, build, or integrate artificial intelligence and machine learning capabilities. They ensure AI/ML solutions are technically sound, responsibly designed, operationally maintainable, and aligned with organizational values and regulatory requirements.

### Responsibilities
- Lead AI/ML solution design, model selection, and architecture decisions; document these in Architecture Decision Records (ADRs)
- Define model evaluation frameworks, performance benchmarks, and acceptance criteria for AI features
- Ensure responsible and ethical AI practices including bias assessment, explainability, and fairness reviews
- Own the model lifecycle (training, validation, deployment, monitoring, retraining, and retirement)
- Identify and manage AI-specific technical risks including model drift, data quality issues, and adversarial inputs
- Collaborate with the Security Lead on AI-specific security considerations (e.g., prompt injection, data poisoning, model exfiltration)
- Track AI-related technical debt and advocate for investment in model quality and infrastructure

### Goals
- Deliver AI/ML capabilities that are accurate, reliable, fair, and maintainable in production
- Ensure the organization's use of AI is ethical, transparent, and compliant with emerging regulations
- Build team capability in AI/ML practices and foster a culture of responsible innovation

### Typical Communication
- AI Architecture Decision Records (ADRs) and model cards documenting model behaviour and limitations
- Model evaluation reports and performance dashboards
- Responsible AI review summaries shared with Stakeholders and Legal / Compliance Advisor
- Technical risk entries in the RAID log for AI-specific risks

### Interactions with Existing Roles
- **Tech Lead / Engineering Lead**: Co-own technical architecture decisions when AI/ML components are involved; align on engineering standards for model code, testing, and deployment.
- **Developers**: Provide guidance on AI/ML implementation, tooling, and best practices; review AI-related code for correctness, security, and maintainability.
- **Product Managers (PdM)**: Translate AI capabilities and limitations into product decisions; advise on what is technically feasible and set realistic expectations for AI-powered features.
- **Security Lead**: Collaborate on AI-specific threat modelling (e.g., adversarial attacks, data privacy in training sets, model access controls).
- **Legal / Compliance Advisor**: Coordinate on AI regulatory requirements, model transparency obligations, and responsible AI policies.
- **Data Analyst**: Align on data quality standards, feature engineering, and metric frameworks that feed AI/ML models and measure their impact.
- **QA / Test Engineers**: Define AI-specific testing strategies including model validation, regression testing for model updates, and fairness/bias test suites.
- **Site Reliability / Operations**: Design observability and monitoring for AI/ML systems in production; establish model drift detection and retraining triggers.
- **Stakeholders / Sponsors**: Communicate AI risks, ethical considerations, and strategic opportunities at executive level; obtain approval for high-impact AI decisions.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [Templates & Checklists](octoacme-templates-and-checklists.md) for RACI, decision log, and other artifacts that reference these personas.
- Use the [Role Engagement Checklist](templates/role-engagement-checklist.md) at the start of any project to confirm which roles are needed and when, including the newer cross-functional roles (Change Manager, Data Analyst, Legal / Compliance Advisor, Community Manager, AI / ML Lead).

