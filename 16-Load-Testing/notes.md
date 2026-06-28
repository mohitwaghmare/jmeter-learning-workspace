# Apache JMeter - Load Testing

## What is Load Testing?

Load Testing measures an application's performance under expected user traffic.

The goal is to ensure the application remains stable and responsive during normal business operations.

---

## Objectives

- Measure response time
- Verify throughput
- Identify bottlenecks
- Ensure stability
- Detect performance degradation

---

## Important Metrics

### Response Time

Time required to complete a request.

---

### Throughput

Number of requests processed per second.

---

### Latency

Time until the first byte of the response is received.

---

### Error Percentage

Percentage of failed requests.

Target:

0%

---

### Concurrent Users

Number of users executing requests simultaneously.

---

## Best Practices

- Start with small user loads.
- Increase users gradually.
- Remove View Results Tree during large tests.
- Monitor CPU, Memory, and Network utilization.
- Analyze reports after execution.

---

## Real-World Example

Suppose an e-commerce website expects 500 concurrent users during a sale.

A Load Test simulates those 500 users and measures:

- Response Time
- Throughput
- Error Rate
- Server Stability

If the application performs well, it is considered capable of handling the expected production load.

---

## Interview Questions

### What is Load Testing?

Load Testing evaluates application performance under expected user load.

---

### Why is Load Testing performed?

To ensure the application can handle expected traffic without performance degradation.

---

### Which metrics are most important?

- Response Time
- Throughput
- Latency
- Error Percentage

---

### Is View Results Tree recommended for large Load Tests?

No.

It consumes significant memory and is intended for debugging.

---

## Summary

Load Testing validates that an application performs efficiently under expected traffic levels. It helps identify bottlenecks before production deployment.