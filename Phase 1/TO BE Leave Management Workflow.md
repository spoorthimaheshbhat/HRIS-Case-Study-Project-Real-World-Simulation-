# TO-BE Workflow Explanation – Leave Management

---

## Overview

The TO-BE Leave Management workflow is a **system-driven, automated process** designed to replace manual, email-based leave handling.

It introduces:

* Structured e-forms
* Real-time validation
* Role-based approval workflows
* Automated notifications
* Centralized data management

---

## Actors Involved

* **Employee** → Applies for leave
* **System (HRIS)** → Validates, routes, and updates data
* **Manager** → Reviews and approves/rejects requests
* **HR** → Monitors and validates records

---

## Workflow Description

### 1. Leave Application Initiation (Employee)

* Employee logs into HRIS
* Navigates to **Apply Leave**
* Fills e-form:

  * Leave type
  * Leave dates
  * Reason

---

### 2. System Validation

The system performs real-time checks:

#### A. Leave Balance Validation

* Ensures sufficient leave balance
* If invalid → error message displayed
* Employee modifies input
* Process ends if employee has no leave balance.

#### B. Date Conflict Check

* Verifies overlapping leave requests
* If conflict → error message displayed

---

### 3. Request Submission

Once validated:

* Leave request is submitted
* System updates:
  * **Status = Pending**
  * Approval ticket is created
* Notification sent to Manager

---

### 4. Manager Review

* Manager logs into HRIS
* Opens approval ticket
* Reviews:

  * Leave details
  * Team availability

---

### 5. Approval Decision

#### If Approved:

* System:

  * Deducts leave balance
  * Updates leave history
  * Maintains audit log
* Notification sent to Employee (CC: HR)
* Ticket status updated to **Closed**

---

#### If Rejected:

* Manager provides comments
* Notification sent to Employee
* Ticket status updated to **Closed**

---

### 6. HR Visibility

* HR can:

  * View leave records
  * Validate updates
  * Access reports and audit logs

---

## Key System Features

* Real-time validation engine
* Automated approval workflow
* Role-based access control
* Notification triggers at each stage
* Centralized database updates
* Audit trail for compliance

---

## Status Flow

```id="flow123"
Draft → Pending → Approved / Rejected → Closed
```

---

## Business Benefits

* Eliminates manual email-based process
* Reduces approval delays
* Improves data accuracy
* Provides real-time visibility
* Enhances employee experience
* Enables audit and compliance tracking

## Out of Scope (Phase 1 Limitations)

The following features has been identified as a potential enhancement but is currently **out of scope for Phase 1** due to development feasibility and budget constraints:

### 1. Reminder Notification Triggers for Pending Approvals

* Automated reminder notifications to managers for **unapproved leave requests after a defined SLA (e.g., 24/48 hours)**
* Escalation mechanisms to higher authorities (e.g., skip-level manager or HR) for prolonged delays

---

## Rationale

* Requires additional development effort for:

  * Scheduler/cron-based trigger mechanisms
  * SLA configuration and tracking
  * Escalation logic design
* Increases system complexity in initial rollout phase
* Prioritized lower compared to core workflow automation (submission, validation, approval)

---

## Future Consideration

This feature can be included in **Phase 2 or Phase 3** to:

* Improve approval turnaround time
* Reduce dependency on manual follow-ups
* Enhance overall workflow efficiency


---

### 2. Unpaid Leave Handling (When Leave Balance is Insufficient)

#### Description:

Currently, the system restricts leave application if the employee does not have sufficient leave balance.

#### Constraint:

* No provision to apply for **unpaid leave (Loss of Pay / LOP)**
* System validation blocks submission when balance is insufficient

#### Rationale:

* Requires additional business rules:

  * Policy-based approval for unpaid leave
  * Payroll integration for salary deductions
* Increases complexity in validation and approval logic
* Needs alignment with HR/payroll policies

#### Future Enhancement:

* Allow employees to apply for unpaid leave - include LOP Leave e-form
* Add approval rules specific to LOP
* Integrate with payroll system for deduction handling

---

### 3. Manager-Initiated Leave Application (On Behalf of Employee)

#### Description:

Currently, leave requests can only be initiated by the employee.

#### Constraint:

* Managers cannot apply leave on behalf of employees
* No proxy or delegated access mechanism available

#### Rationale:

* Requires role-based override permissions
* Needs audit tracking for proxy actions
* Introduces risk of misuse without proper controls

#### Future Enhancement:

* Enable **“Apply on Behalf”** feature for managers/HR - e-form modification
* Maintain audit trail (who applied, for whom)
* Add notification to employee for transparency

---

## Summary

These constraints highlight scenarios that require:

* Additional business rules
* Cross-system integration (e.g., payroll)
* Enhanced role-based access controls

They are deferred to future phases to ensure **focused delivery of core functionalities in Phase 1**.

---

## Conclusion

The TO-BE workflow transforms leave management into a **structured, automated, and transparent process**, significantly improving operational efficiency and user experience compared to the AS-IS state.

---
