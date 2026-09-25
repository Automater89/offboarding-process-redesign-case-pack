# User Stories and Acceptance Criteria: Offboarding Process Redesign

User stories are written from the perspective of each key stakeholder. Acceptance criteria define what "done" looks like for each story.

---

## Story 1: HR Initiates Offboarding

**As an** HR Business Partner,
**I want to** submit one offboarding intake form with the employee name, last day, and departure type,
**So that** all downstream stakeholders are automatically notified and assigned tasks without me sending individual emails.

**Acceptance Criteria:**
- [ ] Intake form captures employee name, ID, last day, departure type (resignation / termination / retirement), and manager
- [ ] Submission triggers Power Automate flow within 5 minutes
- [ ] All stakeholders (IT, Security, Payroll, Manager) receive task notifications automatically
- [ ] HR receives a confirmation that routing was successful
- [ ] Intake record is visible in the offboarding dashboard

---

## Story 2: IT Receives and Confirms Access Revocation

**As an** IT administrator,
**I want to** receive a structured task notification when an employee is offboarding,
**So that** I can revoke access and confirm completion within the defined SLA without relying on an email from HR.

**Acceptance Criteria:**
- [ ] IT receives notification with employee name, ID, last day, and systems list within 1 hour of intake submission
- [ ] Notification includes a confirm button or form to mark access revocation complete
- [ ] Completion timestamp is recorded in the offboarding record
- [ ] If not confirmed within 24 hours of last day, an escalation is sent to the IT lead

---

## Story 3: Manager Coordinates Knowledge Transfer

**As a** direct manager,
**I want to** receive a knowledge transfer checklist tailored to the departing employee's role,
**So that** I can ensure critical information is captured before their last day.

**Acceptance Criteria:**
- [ ] Manager receives a task notification with a knowledge transfer checklist within 1 hour of intake
- [ ] Checklist includes standard items plus role-specific items based on department (AI-assisted draft)
- [ ] Manager can mark checklist items complete individually
- [ ] Overall completion status is visible to HR in the dashboard

---

## Story 4: Security Deactivates Badge Access

**As a** security administrator,
**I want to** receive an automated alert with the employee's badge ID and last day,
**So that** I can deactivate physical access on time without waiting for an HR email.

**Acceptance Criteria:**
- [ ] Security receives notification with badge ID, employee name, last day, and site location
- [ ] Notification includes confirmation step to mark badge deactivation complete
- [ ] Deactivation is confirmed before end of business on last day
- [ ] SLA breach escalation triggers if not confirmed by noon on last day

---

## Story 5: HR Confirms Process Completion

**As an** HR Business Partner,
**I want to** see a single dashboard showing completion status for all offboarding tasks,
**So that** I can close the HR record confidently knowing all steps are done.

**Acceptance Criteria:**
- [ ] Dashboard shows each offboarding record with status by task owner (IT, Security, Payroll, Manager)
- [ ] HR can only mark the record closed when all tasks are confirmed complete
- [ ] Incomplete tasks are highlighted with owner name and days overdue
- [ ] Closed records are archived but searchable for 12 months

---

## Story 6: Employee Receives Clear Offboarding Guidance

**As a** departing employee,
**I want to** receive a clear checklist of what I need to do before my last day,
**So that** I can complete my obligations without chasing HR or IT for information.

**Acceptance Criteria:**
- [ ] Employee receives a personalized offboarding checklist via email within 24 hours of trigger
- [ ] Checklist includes equipment return instructions, exit interview scheduling, and final timesheet submission
- [ ] Checklist is plain-language and does not require HR follow-up to understand
