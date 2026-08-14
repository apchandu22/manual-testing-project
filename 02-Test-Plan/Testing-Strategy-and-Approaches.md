# Testing Strategy & Testing Approaches

## 1. Testing Strategy

The project follows a structured, requirement-driven and risk-based manual testing strategy. Testing is planned according to business requirements, application risk, feature complexity and impact of changes.

### Overall Strategy

```text
Requirement Analysis
        ↓
Test Planning
        ↓
Risk & Scope Assessment
        ↓
Test Scenario Design
        ↓
Test Case Design
        ↓
Test Data Preparation
        ↓
Build / Environment Validation
        ↓
Smoke Testing
        ↓
Functional & Integration Testing
        ↓
System / End-to-End Testing
        ↓
Defect Reporting & Tracking
        ↓
Retesting
        ↓
Regression Testing
        ↓
Release Validation
        ↓
Test Closure
```

## 2. Testing Approaches

### 2.1 Requirement-Based Testing

Test cases are designed from approved business and functional requirements. Requirements are mapped to scenarios and test cases through the RTM.

### 2.2 Risk-Based Testing

Testing effort is prioritized according to business impact, probability of failure, complexity and dependencies.

**High-risk areas:** Login, Cart, Checkout, Payment and Order Placement.

### 2.3 Positive Testing

Verify expected application behavior using valid inputs and valid user actions.

**Example:** Login using valid credentials.

### 2.4 Negative Testing

Verify that invalid, incomplete or unexpected inputs are handled correctly.

**Example:** Login with an invalid password and verify the validation message.

### 2.5 Boundary Value Analysis

Test values at, below and above defined limits.

**Examples:** Password length, quantity limits, PIN/ZIP length and maximum input length.

### 2.6 Equivalence Partitioning

Divide input data into valid and invalid groups and test representative values from each group.

### 2.7 Exploratory Testing

Explore application behavior beyond scripted test cases to identify unexpected defects, usability issues and workflow gaps.

### 2.8 End-to-End Testing

Validate complete business workflows from the initial user action through the final expected outcome.

```text
Login
  ↓
Search Product
  ↓
View Product
  ↓
Add to Cart
  ↓
Checkout
  ↓
Place Order
  ↓
Verify Order History
```

### 2.9 Data-Driven Testing

Execute the same functionality with multiple data sets including valid, invalid, boundary, duplicate and empty values.

### 2.10 Compatibility Testing

Validate critical functionality across supported browsers and supported environments.

### 2.11 Retesting

Execute the failed test case again after a defect fix to confirm that the reported issue has been resolved.

### 2.12 Regression Testing

Execute impacted and business-critical existing functionality after changes or defect fixes to ensure that no new defects were introduced.

## 3. Test Execution Approach

Testing is executed in stages:

1. Build verification
2. Smoke testing
3. Functional testing
4. Integration testing
5. System / E2E testing
6. Defect reporting
7. Retesting
8. Regression testing
9. Release validation

## 4. Defect Management Approach

Defects are recorded in Jira with clear reproduction steps, expected and actual results, severity, priority, environment, evidence and related test case information.

After a fix is delivered, QA performs retesting followed by appropriate regression testing.

## 5. Release Validation Approach

Release readiness is assessed using:

- Test execution status
- Critical business workflow results
- Open defect status
- Severity and priority of remaining defects
- Regression results
- Known risks and dependencies

## 6. Test Closure Approach

Testing is closed after planned execution is completed, required retesting and regression are finished, critical risks are communicated, and the final Test Summary Report is prepared.

> This document describes the QA methodology used in the portfolio project. It does not represent confidential production processes or data.
