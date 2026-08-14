# 👥 Affected Users & Business Impact Analysis

## Purpose

Demonstrate how QA assesses the scope and business impact of a defect using reproducibility, application logs and monitoring evidence.

## Impact Dimensions

| Dimension | Questions |
|---|---|
| User segment | Which user flow or account type is affected? |
| Platform | Is the issue limited to web, iOS or Android? |
| App/browser version | Does a particular version reproduce the issue? |
| Region | Is the issue localized or broad? |
| Feature | Which business workflow is affected? |
| Frequency | How often does the issue occur? |
| Severity | What is the functional/business consequence? |

## Example Analysis

**Issue:** Checkout intermittently fails after payment submission.

**Evidence:**
- Reproduced in synthetic QA data.
- Sanitized logs show payment errors for the affected request pattern.
- Monitoring indicates an elevated checkout error rate during the test window.
- Traffic volume remains stable, suggesting the increase is not explained by a sudden traffic spike.

**Impact Assessment:**

The issue has potentially broad impact on users attempting checkout during the affected period. Exact production user counts should only be reported when supported by authorized telemetry; QA should not invent customer counts.

## Jira Impact Statement – Example

> High impact: checkout completion is intermittently affected for the tested payment flow. Log correlation and monitoring evidence indicate the issue may extend beyond a single user session. Engineering investigation is recommended before release.

## Important QA Practice

Do not expose or store real customer IDs, payment details, IP addresses, tokens or confidential production logs in a portfolio. Use synthetic evidence and describe the investigation method.
