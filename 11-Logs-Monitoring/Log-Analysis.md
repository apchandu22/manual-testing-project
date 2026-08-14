# 📋 Application Log Analysis

## Purpose

Demonstrate how QA uses sanitized application logs to investigate failures and support defect validation.

## Investigation Workflow

```text
Defect Reproduction
      ↓
Record Timestamp / Correlation ID
      ↓
Search Application Logs
      ↓
Identify Error / Warning Pattern
      ↓
Compare Request and Response
      ↓
Document Evidence in Jira
      ↓
Retest After Fix
```

## Sample Sanitized Log

```text
2026-08-14T10:21:33Z INFO  request_id=req-1001 action=checkout status=started
2026-08-14T10:21:35Z ERROR request_id=req-1001 service=payment error=PAYMENT_DECLINED
2026-08-14T10:21:35Z WARN  request_id=req-1001 order_creation=unexpected
```

## What QA Validates

- Timestamp matches the reproduced issue.
- Correlation/request ID is consistent across related events.
- HTTP/service error is consistent with the UI behavior.
- Unexpected downstream actions are identified.
- Error frequency is considered before assessing impact.

## Defect Evidence

Log findings should be summarized in Jira rather than copying sensitive production data. Example:

> Correlation ID `req-1001` shows a payment-declined event followed by an unexpected order-creation event. This supports the reported behavior and was attached as sanitized evidence.

> Examples are synthetic and contain no production logs.
