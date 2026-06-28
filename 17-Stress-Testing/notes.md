# Apache JMeter - Stress Testing

## What is Stress Testing?

Stress Testing evaluates an application's behavior under traffic levels that exceed expected production load.

The objective is to identify the application's breaking point and evaluate its stability under extreme conditions.

---

## Objectives

- Find maximum supported load
- Identify performance bottlenecks
- Observe system failures
- Verify recovery after overload

---

## Key Metrics

### Response Time

Time taken to complete requests.

---

### Throughput

Number of requests processed per second.

---

### Error Percentage

Percentage of failed requests.

---

### Breaking Point

The point where the application can no longer handle additional load.

---

## Best Practices

- Increase users gradually.
- Monitor server resources.
- Record response times.
- Analyze errors.
- Remove View Results Tree for large tests.

---

## Real-World Example

Suppose an application normally supports 500 users.

Stress Test:

500

↓

1000

↓

1500

↓

2000

Eventually:

- Response time increases
- Errors appear
- Server crashes or becomes unresponsive

The highest stable load before failure is used to estimate system capacity.

---

## Interview Questions

### What is Stress Testing?

Stress Testing evaluates an application's behavior under load beyond its expected capacity.

---

### Why perform Stress Testing?

To determine the application's breaking point and identify performance bottlenecks.

---

### What is the difference between Load Testing and Stress Testing?

Load Testing validates expected traffic.

Stress Testing exceeds expected traffic to identify failure limits.

---

## Summary

Stress Testing helps organizations understand system limits, identify bottlenecks, and improve application reliability before production.