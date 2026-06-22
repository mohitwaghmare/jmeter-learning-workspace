# Apache JMeter - Listeners

## What is a Listener?

A Listener displays, stores, and analyzes the results generated during test execution.

---

## Common Listeners

### View Results Tree

Used for debugging.

Displays:

- Request
- Response
- Headers
- JSON/XML
- Response Code

---

### Summary Report

Displays:

- Samples
- Average Response Time
- Minimum
- Maximum
- Throughput
- Error %

---

### Aggregate Report

Displays:

- Average
- Median
- 90th Percentile
- 95th Percentile
- 99th Percentile
- Throughput
- Error %

---

## Best Practices

Use View Results Tree only while creating or debugging tests.

Remove heavy listeners before running large load tests because they consume significant memory.

For performance analysis, Summary Report and Aggregate Report are preferred.

---

## Real-World Usage

Development:
- View Results Tree

QA:
- Summary Report

Performance Testing:
- Aggregate Report
- HTML Dashboard Report

---

## Summary

Listeners help analyze test execution. During test creation, View Results Tree is the most useful. During performance analysis, Summary Report and Aggregate Report provide key metrics such as response time, throughput, and percentiles.