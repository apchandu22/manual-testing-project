# 📈 Grafana Monitoring

## Purpose

Demonstrate how QA can use service metrics to understand whether a defect is isolated or associated with a wider service degradation.

## Metrics Reviewed

- Request volume
- Error rate
- HTTP 4xx/5xx rate
- Response latency
- Service availability
- Dependency failures

## Example Synthetic Observation

| Metric | Baseline | During Issue | Interpretation |
|---|---:|---:|---|
| Checkout error rate | 0.8% | 7.2% | Significant increase |
| Payment latency | 420 ms | 1,250 ms | Degradation observed |
| HTTP 5xx | 0.2% | 2.1% | Elevated server errors |
| Request volume | 10,000/hr | 10,400/hr | Traffic remained stable |

## QA Analysis

A defect reproduced by a single user may still require broader validation if monitoring indicates elevated error rates. QA should correlate the application behavior, timestamps and logs with service metrics before making an impact assessment.

## Release Decision Support

Metrics are supporting evidence, not a substitute for functional testing. QA combines monitoring evidence with reproduction results, test execution and business impact to communicate release risk.

> Metrics shown here are synthetic portfolio examples.
