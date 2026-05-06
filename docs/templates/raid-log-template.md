# RAID Log: [Project / Initiative Name]

> **Usage:** Maintain this log throughout the project lifecycle. Review it at every weekly sync and sprint planning session. Escalate items whose status changes to **Escalated** to the Project Manager immediately.

---

## Risks

| ID | Description | Likelihood (H/M/L) | Impact (H/M/L) | Owner | Mitigation / Response | Status | Date Raised | Last Updated |
|---|---|---|---|---|---|---|---|---|
| R-001 | [Risk description] | M | H | [Name] | [Mitigation action] | Open | YYYY-MM-DD | YYYY-MM-DD |
| R-002 | [Security vulnerability in dependency] | L | H | Security Lead | Monitor CVE feeds; schedule patching sprint | Open | YYYY-MM-DD | YYYY-MM-DD |

**Status values:** Open · Mitigated · Escalated · Closed

---

## Assumptions

| ID | Assumption | Owner | Validation Method | Validated? | Date Raised |
|---|---|---|---|---|---|
| A-001 | [Assumption description] | [Name] | [How will this be confirmed?] | No | YYYY-MM-DD |
| A-002 | [API availability from third-party system] | Tech Lead | Spike / proof of concept | No | YYYY-MM-DD |

---

## Issues

| ID | Description | Severity (H/M/L) | Owner | Resolution / Action | Status | Date Raised | Target Resolution |
|---|---|---|---|---|---|---|---|
| I-001 | [Issue description] | M | [Name] | [Action being taken] | In Progress | YYYY-MM-DD | YYYY-MM-DD |
| I-002 | [Production incident — see incident report IR-001] | H | SRE | Post-incident review completed; fix deployed | Closed | YYYY-MM-DD | YYYY-MM-DD |

**Severity / Status values:** H/M/L · Open · In Progress · Escalated · Closed

### Escalation Paths
- **Technical issues:** Developer → Tech Lead → Project Manager
- **Security incidents:** Developer/Security Lead → Security Lead → Project Manager → Sponsor (for P1 incidents, notify within 1 hour)
- **Operational incidents:** On-call SRE → SRE Lead → Release Manager → Project Manager (for Sev-1, notify within 30 minutes)
- **Business/scope issues:** Project Manager → Product Manager → Sponsor

---

## Dependencies

| ID | Description | Type (Internal/External) | Owner | Dependent Team/System | Due Date | Status |
|---|---|---|---|---|---|---|
| D-001 | [Dependency description] | Internal | [Name] | [Team/System] | YYYY-MM-DD | On Track |
| D-002 | [Third-party API contract finalised] | External | Product Manager | [Vendor name] | YYYY-MM-DD | At Risk |

**Status values:** On Track · At Risk · Blocked · Resolved

---

## Review Log

| Date | Reviewer | Changes Made |
|---|---|---|
| YYYY-MM-DD | [Name] | Initial log created |
| YYYY-MM-DD | [Name] | [Description of update] |

---

_See [Templates & Checklists Index](../octoacme-templates-and-checklists.md) for related templates._
_See [Risk Management & Communication](../octoacme-risks-and-communication.md) for the full escalation and communication policy._
