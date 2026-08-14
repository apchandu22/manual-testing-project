# 🟣 Jira Defect Management

## Purpose

Demonstrate how defects are documented and managed through the Jira lifecycle during Agile testing.

## Sample Jira Ticket

**Issue Key:** ECOM-101  
**Summary:** Order record created after payment failure  
**Issue Type:** Bug  
**Priority:** High  
**Severity:** High  
**Environment:** QA  
**Component:** Payment / Order

### Description

A synthetic declined payment response displays a payment failure, but an order record is created unexpectedly.

### Acceptance for Fix

- Failed payment must not create a completed order.
- User must receive a clear failure message.
- Retry must not create duplicate orders.
- Order history must remain consistent.

## Jira Workflow

```text
Open
 ↓
Assigned
 ↓
In Progress
 ↓
Fixed
 ↓
Ready for QA
 ↓
Retest
 ├── Pass → Closed
 └── Fail → Reopened
```

## QA Evidence

Jira defects should reference the related test case, build/version, environment, screenshots, timestamps, API evidence and relevant sanitized logs where applicable.

## Agile Usage

- Defects are discussed during daily Scrum when they affect sprint scope.
- QA updates test execution and defect status.
- High-impact defects are reviewed before release sign-off.
- Fixed defects are retested before closure.
