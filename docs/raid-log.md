# RAID Log: Offboarding Process Redesign

RAID stands for Risks, Assumptions, Issues, and Dependencies. This log is a living document updated throughout the project.

---

## Risks

| # | Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|---|
| R1 | HRIS does not support API trigger for Power Automate | Medium | High | Use a manual SharePoint form as trigger fallback; plan HRIS integration as phase 2 |
| R2 | IT team capacity to adopt new notification-based workflow | Medium | Medium | Include IT in design review; keep task format simple and familiar |
| R3 | Termination scenarios require faster SLA than resignation | High | High | Add departure type logic to flow; set 4-hour SLA for terminations vs 48-hour for resignations |
| R4 | Employee data in automation layer creates privacy exposure | Low | High | Limit data fields in automation to role, last day, and department; no personal reasons stored |
| R5 | Dashboard not adopted by HR if too complex | Medium | Medium | Keep dashboard to 5 key fields; validate design with HR lead before build |

---

## Assumptions

| # | Assumption | Owner | Validation Needed? |
|---|---|---|---|
| A1 | HR will use a SharePoint form to initiate offboarding if HRIS integration is not available | HR Lead | Yes — confirm in stakeholder session |
| A2 | IT has a ticketing system that can receive structured input from Power Automate | IT Lead | Yes — confirm system and API access |
| A3 | All offboarding steps can be completed within a 3-business-day SLA | HR / IT / Security leads | Yes — validate with each owner |
| A4 | Manager receives notification at same time as IT and Security | Design decision | No — confirm in flow design |

---

## Issues

| # | Issue | Status | Owner | Resolution |
|---|---|---|---|
| I1 | Current offboarding for one business unit uses a separate manual process not yet mapped | Open | HR Lead | Schedule discovery session to map current-state variant |
| I2 | Knowledge transfer checklist format not yet agreed upon across departments | Open | HR / Dept Leads | Facilitate short workshop to align on core vs department-specific items |

---

## Dependencies

| # | Dependency | Depends On | Risk If Not Met |
|---|---|---|---|
| D1 | Power Automate flow design | SharePoint list structure finalized | Flow cannot be built until intake fields are locked |
| D2 | IT task notification | IT confirms receipt format (email vs Teams vs ticket) | Notification may not integrate cleanly with IT workflow |
| D3 | Dashboard build | All task confirmation steps defined | Dashboard cannot show accurate completion status without defined confirmation logic |
| D4 | SLA enforcement | Escalation recipients defined by HR and IT | Escalation flow cannot be configured without named owners |
