# 🧪 Manual Testing Project

## 📌 Project Overview

This repository demonstrates an end-to-end Manual QA approach for a web-based e-commerce application. It covers the Software Testing Life Cycle (STLC), Agile/Scrum testing, test design, execution, defect management, API validation and production-style investigation using sanitized logs and monitoring examples.

> **Portfolio note:** All data, defects, logs, metrics and identifiers are synthetic examples created for demonstration. No production/customer information is included.

## 🎯 Testing Objectives

- Validate functionality against business requirements
- Design positive, negative and boundary test coverage
- Validate critical end-to-end e-commerce workflows
- Execute smoke, sanity, functional, integration and regression testing
- Validate APIs using Postman
- Track defects through Jira workflow
- Investigate application failures using logs and Kibana-style searches
- Review Grafana-style service metrics for supporting evidence
- Assess potential affected-user/business impact without exposing real user data
- Verify fixes through retesting and regression testing
- Support release validation and QA sign-off decisions

## 🧪 Testing Types

- Functional Testing
- Regression Testing
- Smoke Testing
- Sanity Testing
- Integration Testing
- System Testing
- End-to-End Testing
- Exploratory Testing
- Usability Testing
- Compatibility / Cross-Browser Testing
- Negative Testing
- Boundary Value Analysis
- Equivalence Partitioning
- API Testing

## 🌐 Application Modules

### 🔐 User Management
- User Registration
- Login / Logout
- Password Validation
- Invalid Login
- Session Validation

### 🔎 Product Management
- Product Search
- Product Listing
- Product Details
- Filtering
- Sorting

### 🛒 Shopping Cart
- Add Product
- Remove Product
- Update Quantity
- Cart Total
- Cart Persistence

### 💳 Checkout & Payment
- Address Management
- Order Summary
- Payment Validation
- Successful / Failed Payment
- Order Placement

### 📦 Order Management
- Order Confirmation
- Order History
- Order Details
- Order Status

## 🔄 QA Testing Workflow

```text
Requirement Analysis
        ↓
Test Planning & Risk Assessment
        ↓
Test Scenario Design
        ↓
Test Case Design
        ↓
Test Data Preparation
        ↓
Environment / Build Validation
        ↓
Smoke Testing
        ↓
Functional Testing
        ↓
API / Backend Validation
        ↓
Defect Reporting in Jira
        ↓
Log Investigation
        ↓
Kibana Error Analysis
        ↓
Grafana Metrics Review
        ↓
Affected User / Business Impact Assessment
        ↓
Developer Fix
        ↓
Retesting
        ↓
Risk-Based Regression Testing
        ↓
Release Validation
```

## 📂 Repository Contents

| Folder | Purpose |
|---|---|
| `01-Requirements` | Business and functional requirements |
| `02-Test-Plan` | Scope, strategy, risks and entry/exit criteria |
| `03-Test-Scenarios` | High-level test scenarios |
| `04-Test-Cases` | Detailed manual test cases |
| `05-RTM` | Requirement-to-test-case traceability |
| `06-Test-Data` | Synthetic reusable test data |
| `07-Test-Execution` | Execution results and metrics |
| `08-Defect-Reports` | Structured sample defects |
| `09-Jira` | Jira defect lifecycle and QA workflow |
| `10-API-Testing` | Postman API validation |
| `11-Logs-Monitoring` | Application log analysis |
| `12-Kibana` | Kibana-style error investigation |
| `13-Grafana` | Monitoring and service metrics |
| `14-Impact-Analysis` | Affected-user and business impact assessment |
| `15-Agile` | Agile/Scrum QA activities |
| `16-Regression` | Risk-based regression suite |
| `17-Smoke-Sanity` | Smoke and sanity suites |
| `18-Test-Summary` | Final QA test summary and release validation |

## 🔌 API Testing – Postman

API coverage includes login, product search, cart, checkout and order workflows. Validation includes status codes, response body/schema, headers, authentication, negative scenarios, response time and UI/API data consistency.

## 🐞 Jira Defect Management

Sample defects demonstrate:

- Summary and module
- Environment/build
- Preconditions
- Steps to reproduce
- Expected vs actual result
- Severity and priority
- Evidence
- Related test case
- Retest and closure status

## 📋 Logs, Kibana & Grafana Investigation

The project demonstrates an investigation workflow where QA:

1. Reproduces the issue.
2. Records timestamp and correlation/request ID.
3. Reviews sanitized application logs.
4. Searches for related errors using Kibana-style filters.
5. Reviews Grafana-style error rate, latency and availability metrics.
6. Compares successful and failed requests.
7. Assesses whether the issue appears isolated or potentially broader.
8. Documents evidence and impact in Jira.
9. Retests the fix and executes impacted regression tests.

## 👥 Affected User / Business Impact

Impact is assessed using supported evidence such as affected workflow, platform/version, region, reproducibility, error frequency and service metrics. Exact production user counts are never invented or exposed in this portfolio.

## 📊 Example Test Metrics

- Total Test Cases: 25
- Executed: 25
- Passed: 21
- Failed: 3
- Blocked: 1
- Pass Rate: 84%
- Critical Defects: 0
- High Defects: 2
- Medium Defects: 1

> Metrics above are synthetic portfolio examples.

## 🧰 Tools & Skills

**Manual QA:** Functional, Regression, Smoke, Sanity, Integration, System, E2E, Exploratory, Compatibility Testing

**API:** Postman, REST API validation

**Defect / Test Management:** Jira, test case management concepts, RTM

**Database:** SQL validation concepts

**Investigation / Monitoring:** Application Logs, Kibana, Grafana

**Methodology:** Agile / Scrum, STLC, SDLC

**Documentation:** Markdown, test evidence and execution reporting

## 🎯 QA Skills Demonstrated

- Requirement Analysis
- Risk-Based Testing
- Test Scenario Design
- Test Case Design
- Test Data Preparation
- API Testing
- Defect Reporting
- Defect Lifecycle Management
- Log Analysis
- Monitoring Analysis
- Impact Assessment
- Retesting
- Regression Testing
- Release Validation

---

### 👨‍💻 Author

**A P Chandan**  
Software Test Engineer | Manual Testing | API Testing | Automation Testing

urlGitHub Profilehttps://github.com/apchandu22
