# Problem Statement: Employee Offboarding Process

## Process Scope

The employee offboarding process covers all activities from the point a resignation or termination is confirmed through the employee's last day and final administrative closure. It spans HR, IT, Security, Payroll, and the departing employee's direct manager.

## Stakeholders

| Stakeholder | Role in Process |
|---|---|
| HR Business Partner | Initiates offboarding, manages documentation and compliance |
| Direct Manager | Coordinates knowledge transfer, approves final time, returns equipment |
| IT | Revokes access, retrieves equipment, archives accounts |
| Security | Deactivates badge and physical access |
| Payroll | Processes final pay, PTO payout |
| Departing Employee | Completes checklist, returns equipment, attends exit interview |

## Current State Pain Points

1. **No single trigger point.** Offboarding starts differently for resignations vs. terminations, and the process is not consistently initiated. Some steps are missed entirely when handoffs are verbal.
2. **Manual email coordination.** HR emails IT, Security, and Payroll separately. There is no structured handoff, no confirmation, and no tracking.
3. **Access revocation delays.** IT revocation is dependent on receiving an email from HR, which sometimes arrives after the employee's last day. This creates security exposure.
4. **Equipment recovery gaps.** No centralized tracking of what equipment needs to be returned, by when, or who is responsible for follow-up.
5. **Inconsistent exit documentation.** Exit interviews, final performance notes, and knowledge transfer completion are tracked in different places or not tracked at all.
6. **No SLA or accountability.** There is no defined timeline for completing offboarding steps, and no one is accountable for the overall process completion.

## Why This Matters

Incomplete offboarding creates real risk: security exposure from unrevoked access, compliance gaps in HR records, equipment loss, and a poor departing employee experience that affects employer brand. It is also a source of significant manual work for HR and IT teams.

## Design Goal

Redesign the offboarding process so that it is:
- Triggered consistently from a single source of truth
- Routed automatically to all owners with clear tasks and deadlines
- Tracked end-to-end with full visibility
- Completed within a defined SLA with accountability
- Supported by AI and automation where it reduces manual work without introducing new risk
