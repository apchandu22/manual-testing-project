# 🔎 Kibana Investigation

## Purpose

Demonstrate a QA workflow for investigating application errors using a Kibana-style log search with sanitized sample data.

## Investigation Steps

1. Reproduce the defect.
2. Record timestamp, environment and correlation/request ID.
3. Search the relevant service logs.
4. Filter by error level, service and request ID.
5. Compare successful and failed requests.
6. Identify the error pattern and frequency.
7. Capture only non-sensitive evidence in the Jira defect.

## Example Search Concept

```text
service:checkout AND level:ERROR AND request_id:req-1001
```

## Sample Findings

| Observation | Finding |
|---|---|
| Service | Payment |
| Error | PAYMENT_DECLINED |
| Correlation ID | req-1001 |
| Related Event | Unexpected order creation |
| Pattern | Reproduced 3/3 in synthetic QA data |
| QA Action | Linked evidence to Jira defect |

## QA Value

Kibana-style log investigation helps QA move beyond UI symptoms by correlating a failed workflow with backend service events and timestamps.

> This is a portfolio simulation using synthetic logs; it does not represent access to confidential production dashboards or customer data.
