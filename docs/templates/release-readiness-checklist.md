# Release Readiness Checklist: [Project Name] — [Version / Release Tag]

> **Usage:** Complete this checklist before every production deployment. All **Required** items must be checked before the Release Manager calls a go/no-go. Any unchecked required item is an automatic **NO-GO** unless an approved exception is documented.

---

## Release Details

| Field | Details |
|---|---|
| **Project / Service** | [Name] |
| **Release Version / Tag** | [v1.2.3 / YYYY-MM-DD-release] |
| **Target Deployment Date** | YYYY-MM-DD HH:MM UTC |
| **Release Manager** | [Name] |
| **Go/No-Go Decision** | ⬜ GO / ⬜ NO-GO |
| **Decision Made By** | [Name, Role] |
| **Decision Date** | YYYY-MM-DD |

---

## 1. Scope & Requirements

| # | Check | Required | Owner | Status |
|---|---|---|---|---|
| 1.1 | All committed features / stories are merged and closed | ✅ Required | Product Manager | ⬜ |
| 1.2 | Acceptance criteria verified for each story | ✅ Required | QA / Test Engineer | ⬜ |
| 1.3 | Out-of-scope items documented and deferred to next release | ✅ Required | Project Manager | ⬜ |
| 1.4 | Feature flags configured correctly for this release | ✅ Required | Tech Lead | ⬜ |

---

## 2. Quality & Testing

| # | Check | Required | Owner | Status |
|---|---|---|---|---|
| 2.1 | All automated test suites pass (unit, integration, e2e) | ✅ Required | QA / Test Engineer | ⬜ |
| 2.2 | Regression test suite executed and passed | ✅ Required | QA / Test Engineer | ⬜ |
| 2.3 | No open P1 / Critical bugs | ✅ Required | QA / Test Engineer | ⬜ |
| 2.4 | All open P2 bugs assessed and accepted/deferred with owner | ✅ Required | Product Manager | ⬜ |
| 2.5 | Performance / load testing completed (if applicable) | ⚠️ If applicable | Tech Lead | ⬜ |
| 2.6 | Accessibility / usability review completed | ⚠️ If applicable | UX Designer | ⬜ |
| 2.7 | Test summary report linked below | ✅ Required | QA / Test Engineer | ⬜ |

**Test summary report:** [link]

---

## 3. Security

| # | Check | Required | Owner | Status |
|---|---|---|---|---|
| 3.1 | Security review completed (SAST/DAST scans passed) | ✅ Required | Security Lead | ⬜ |
| 3.2 | No open High/Critical CVEs in dependencies | ✅ Required | Security Lead | ⬜ |
| 3.3 | Secrets / credentials not hardcoded; secrets rotated if exposed | ✅ Required | Security Lead | ⬜ |
| 3.4 | Threat model reviewed and risks accepted or mitigated | ✅ Required | Security Lead | ⬜ |
| 3.5 | Penetration test / security assessment completed (if required) | ⚠️ If applicable | Security Lead | ⬜ |

**Security sign-off by:** [Name] **Date:** YYYY-MM-DD

---

## 4. Operational Readiness

| # | Check | Required | Owner | Status |
|---|---|---|---|---|
| 4.1 | Deployment runbook is current and reviewed | ✅ Required | SRE / Ops | ⬜ |
| 4.2 | Rollback plan documented and tested | ✅ Required | SRE / Ops | ⬜ |
| 4.3 | Monitoring, alerting, and dashboards updated for new changes | ✅ Required | SRE / Ops | ⬜ |
| 4.4 | SLOs / SLIs reviewed and baselines updated | ✅ Required | SRE / Ops | ⬜ |
| 4.5 | On-call rotation confirmed and briefed on release | ✅ Required | SRE / Ops | ⬜ |
| 4.6 | Maintenance window communicated to affected teams | ✅ Required | Release Manager | ⬜ |
| 4.7 | Data migration / schema changes reviewed and tested | ⚠️ If applicable | Tech Lead | ⬜ |

---

## 5. Communication & Documentation

| # | Check | Required | Owner | Status |
|---|---|---|---|---|
| 5.1 | Release notes drafted and reviewed | ✅ Required | Product Manager | ⬜ |
| 5.2 | Customer-facing announcements prepared (if needed) | ⚠️ If applicable | Customer Support | ⬜ |
| 5.3 | Internal stakeholder notification prepared | ✅ Required | Project Manager | ⬜ |
| 5.4 | User / API documentation updated | ⚠️ If applicable | Tech Lead / UX | ⬜ |
| 5.5 | Support team briefed on new features and known issues | ✅ Required | Customer Support | ⬜ |

---

## 6. Go/No-Go Sign-offs

| Role | Name | Sign-off | Date |
|---|---|---|---|
| QA / Test Engineer | [Name] | ⬜ Approved / ⬜ Blocked | YYYY-MM-DD |
| Tech Lead | [Name] | ⬜ Approved / ⬜ Blocked | YYYY-MM-DD |
| Security Lead | [Name] | ⬜ Approved / ⬜ Blocked | YYYY-MM-DD |
| SRE / Operations | [Name] | ⬜ Approved / ⬜ Blocked | YYYY-MM-DD |
| Product Manager | [Name] | ⬜ Approved / ⬜ Blocked | YYYY-MM-DD |
| **Release Manager** | **[Name]** | **⬜ GO / ⬜ NO-GO** | YYYY-MM-DD |

---

## 7. Exceptions / Deferred Items

> List any required checks that were not completed and the approved exception reason.

| # | Check Skipped | Reason | Approved By | Date |
|---|---|---|---|---|
| [e.g. 3.5] | [Check description] | [Reason] | [Name] | YYYY-MM-DD |

---

## 8. Post-Deployment Verification

| # | Check | Owner | Status |
|---|---|---|---|
| 8.1 | Smoke tests passed in production | SRE / QA | ⬜ |
| 8.2 | Key metrics and error rates within baseline thresholds | SRE | ⬜ |
| 8.3 | Release notes published | Product Manager | ⬜ |
| 8.4 | Stakeholders notified of successful deployment | Project Manager | ⬜ |
| 8.5 | No rollback triggered within 30 minutes of deployment | SRE | ⬜ |

---

_See [Templates & Checklists Index](../octoacme-templates-and-checklists.md) for related templates._
_See [Release & Deployment](../octoacme-release-and-deployment.md) for the full release process._
