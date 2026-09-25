# Process Notes: As-Is and To-Be Design

## As-Is Summary

The current offboarding process is primarily email-driven and manually coordinated. There is no centralized trigger, no automated routing, and no SLA.

**Key handoff failures in the current state:**

- HR notifies IT and Security by email, often after the fact
- IT has no visibility into pending offboardings until they receive an email
- Equipment return has no formal tracking or deadline
- Exit documentation is inconsistent and stored in multiple places
- No one owns the overall process end-to-end

**Typical cycle time today:** 5 to 14 days for full closure, often incomplete

---

## To-Be Design

The redesigned process uses a single intake trigger in SharePoint or an HRIS integration, which then fans out automatically to all owners with task assignments, deadlines, and confirmations tracked in one place.

**To-be design principles:**

1. One trigger, consistent for all departure types
2. Automated routing to IT, Security, Payroll, and Manager within 1 hour of trigger
3. Each owner receives a structured task with a deadline and a confirmation step
4. A central dashboard shows completion status per offboarding record
5. SLA breach triggers an escalation notification to HR lead

**Where AI and automation realistically help:**

| Process Step | AI / Automation Opportunity | Notes |
|---|---|---|
| Step 1: Trigger | Power Automate triggered by HRIS record change or form submission | Removes manual initiation |
| Step 2: Notify stakeholders | Automated routing via Power Automate with task cards | Replaces manual email chain |
| Step 3: Access revocation | Auto-generated IT ticket via ServiceNow or IT system API | Removes email dependency |
| Step 4: Badge deactivation | Automated alert to Security with badge ID and last day | Removes manual Security email |
| Step 5: Knowledge transfer | AI-assisted checklist generation based on role and tenure | Copilot can draft a starter checklist |
| Step 6: Final pay | Automated Payroll notification with hours and PTO data | Reduces manual timesheet coordination |
| Step 7: Record closure | Automated checklist completion check before HR record is closed | Prevents premature closure |

**Target cycle time to-be:** Full closure within 3 business days of last day

---

## Key Design Decisions

- **Human in the loop at IT and Security.** Access revocation creates a ticket and sends a confirmation; a human confirms completion. Automation initiates; humans verify.
- **No AI making employment decisions.** Copilot assists with drafting only. All approvals remain with HR and manager.
- **Privacy-first.** The offboarding record in SharePoint includes role and departure date only. Personal departure reasons are not stored in the automation layer.
