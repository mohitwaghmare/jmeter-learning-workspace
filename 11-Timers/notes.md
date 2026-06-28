# Apache JMeter - Timers

## What is a Timer?

A Timer introduces a delay before a sampler is executed.

Timers help simulate realistic user behavior by preventing all requests from being sent instantly.

---

## Why Use Timers?

- Simulate real users
- Prevent unrealistic load
- Control request pacing
- Improve test realism

---

## Common Timers

### Constant Timer

Adds a fixed delay.

Example:

2000 milliseconds

= 2 seconds

---

### Uniform Random Timer

Adds a random delay within a defined range.

Useful for simulating different user think times.

---

### Gaussian Random Timer

Generates delays based on a normal (Gaussian) distribution.

---

### Synchronizing Timer

Makes multiple virtual users send requests simultaneously.

Useful for stress and spike testing.

---

## Units

1000 ms = 1 second

2000 ms = 2 seconds

5000 ms = 5 seconds

---

## Best Practices

- Use realistic think times.
- Avoid unnecessary delays.
- Choose timer types based on the testing objective.
- Combine timers with Thread Groups for realistic load.

---

## Interview Questions

### What is a Timer?

A Timer delays request execution to simulate user think time.

---

### Why are Timers used?

To make performance tests more realistic by controlling when requests are sent.

---

### Which Timer is most commonly used?

Constant Timer.

---

## Summary

Timers control the pacing of requests in JMeter. They are essential for creating realistic performance tests and avoiding unrealistic bursts of traffic.