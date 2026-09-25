# KPI Framework: Offboarding Process Redesign

## Design Principle

KPIs should measure whether the redesigned process actually improves outcomes — not just whether the automation runs. A flow that fires every time is not a success if access is still revoked late or HR records are still left open.

---

## Core KPIs

| KPI | Definition | Baseline (Current) | Target (To-Be) | Measurement Source |
|---|---|---|---|---|
| End-to-end cycle time | Days from trigger to full record closure | 5–14 days | ≤ 3 business days | Offboarding dashboard |
| On-time access revocation | % of offboardings where IT confirms revocation before last day EOB | Unknown (manual) | > 95% | Power Automate log |
| On-time badge deactivation | % of offboardings where Security confirms deactivation by last day EOB | Unknown (manual) | > 95% | Power Automate log |
| Knowledge transfer completion | % of offboardings with manager checklist fully completed | Unknown | > 80% | Dashboard |
| SLA breach rate | % of offboardings with at least one step past SLA | Unknown | < 10% | Dashboard escalation log |
| HR record closure rate | % of offboardings with fully closed HR record within 5 days | Unknown | > 90% | HR system |
| Automation trigger reliability | % of offboardings correctly initiated via new process vs manual workaround | 0% (no automation) | > 95% | Power Automate run history |

---

## Measurement Cadence

| Frequency | Review |
|---|---|
| Weekly | SLA breach log and any open escalations |
| Monthly | All KPIs vs targets; top 3 process gaps |
| Quarterly | Full process review; user feedback from HR, IT, Security leads; consider scope changes |

---

## Baselining Plan

Before the new process goes live, capture baseline data by:
1. Reviewing the last 20 completed offboarding records for cycle time and common failure points
2. Surveying HR, IT, and Security leads on current pain level (1–5 scale)
3. Documenting the current manual steps and estimated time per step

This baseline gives a before/after comparison to demonstrate real impact, not just technical deployment.
