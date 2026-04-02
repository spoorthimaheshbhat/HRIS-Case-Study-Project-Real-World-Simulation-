# AS-IS Process – Leave Management (Functional View)

### HRIS Case Study Project (Phase 1)

---

## Process Objective

To manage employee leave requests through an approval mechanism ensuring:

* Manager visibility into team availability
* HR tracking of leave balances
* Proper documentation of leave records

---

## Process Actors & Responsibilities

| Actor    | Responsibility                             |
| -------- | ------------------------------------------ |
| Employee | Initiate leave request and follow up       |
| Manager  | Review, approve/reject leave request       |
| HR Team  | Maintain leave records and update balances |

---

## Current Workflow (AS-IS Process)

### Trigger:

Employee intends to take leave

---

### Step 1: Leave Request Initiation

* Employee drafts an email to the reporting manager
* Includes:

  * Leave type (Sick/Casual/Earned)
  * Start and end date
  * Reason for leave

---

### Step 2: Manager Review

* Manager checks:

  * Team availability
  * Business impact
  * No system support for validation (manual judgment)

---

### Step 3: Approval / Rejection

* Manager responds via email:

  * Approve → confirmation email
  * Reject → reason shared (optional)

---

### Step 4: Follow-Up (If Required)

* If no response:

  * Employee sends reminder emails
* No automated escalation mechanism

---

### Step 5: HR Record Update

* HR receives approval email (sometimes manually forwarded)
* Updates leave details in Excel:

  * Employee name
  * Leave dates
  * Leave type
  * Updated balance

---

### Step 6: Leave Balance Tracking

* Employee must:

  * Ask HR for updated leave balance
  * Or refer to outdated records

---

### Step 7: Record Maintenance

* HR maintains:

  * Multiple Excel sheets
  * Monthly or team-wise records
* No centralized repository

---

## Business Rules (Current State)

* Leave approval is **mandatory before leave is taken**
* Leave balance is tracked manually by HR
* No system validation for:

  * Overlapping leaves
  * Insufficient leave balance
* Approval hierarchy is **single-level (Manager only)**

---

## Process Characteristics

| Aspect        | Current State         |
| ------------- | --------------------- |
| Workflow Type | Manual (Email-driven) |
| Validation    | Manual                |
| Tracking      | Excel-based           |
| Visibility    | Limited               |
| Notifications | Manual (emails only)  |
| Audit Trail   | Not maintained        |

---

## Functional Gaps Identified

### Workflow Gaps

* No structured workflow or system enforcement
* No defined SLA for approvals

---

### Validation Gaps

* No leave balance validation
* No restriction on invalid requests

---

### Tracking Gaps

* No real-time status tracking
* No centralized leave history

---

### Communication Gaps

* No automated notifications or reminders
* High dependency on manual follow-ups

---

### Data & Control Gaps

* No single source of truth
* High risk of data inconsistency
* No audit trail or reporting

---

## Business Impact

* Delayed leave approvals
* Increased manual effort for HR
* Higher chances of errors in leave records
* Reduced employee satisfaction due to lack of transparency

---

## Summary

The current leave management process operates through **manual, unstructured workflows with limited validation and tracking capabilities**, resulting in inefficiencies, lack of transparency, and increased operational overhead.

This highlights the need for a **system-driven, automated workflow in the TO-BE state**.

---
