# Apache JMeter - Endurance (Soak) Testing

## What is Endurance Testing?

Endurance Testing, also known as Soak Testing, evaluates application performance under a constant load over an extended period.

The objective is to identify issues that appear only after long-running execution.

---

## Objectives

- Detect memory leaks
- Verify application stability
- Monitor CPU and memory usage
- Observe response time consistency
- Ensure sustained throughput

---

## Common Issues Found

- Memory leaks
- Increasing response times
- CPU spikes
- Resource exhaustion
- Connection pool exhaustion

---

## Important Metrics

- Response Time
- Throughput
- Error Percentage
- CPU Usage
- Memory Usage
- Network Utilization

---

## Best Practices

- Use realistic user loads.
- Monitor server resources throughout the test.
- Avoid using View Results Tree.
- Execute tests for several hours in production-like environments.
- Analyze trends instead of single measurements.

---

## Interview Questions

### What is Endurance Testing?

Endurance Testing verifies application stability under a constant workload over a long period.

---

### What problems can Endurance Testing identify?

- Memory leaks
- CPU spikes
- Resource exhaustion
- Performance degradation

---

### Why shouldn't View Results Tree be used?

Because it stores every request in memory, making it unsuitable for long-running performance tests.

---

## Summary

Endurance Testing ensures that applications remain stable, responsive, and reliable during prolonged periods of expected user activity.