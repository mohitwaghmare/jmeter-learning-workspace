# Apache JMeter - Test Plan

## What is a Test Plan?

A Test Plan is the root element in Apache JMeter. It contains all the components required to execute a performance test.

Everything in JMeter starts with a Test Plan.

---

## What can a Test Plan contain?

- Thread Groups
- HTTP Requests
- Assertions
- Timers
- Controllers
- Listeners
- Configuration Elements
- Variables

---

## Why is a Test Plan important?

A Test Plan defines:

- What to test
- How many users to simulate
- What requests to send
- How to validate responses
- How to display results

---

## File Extension

JMeter Test Plans are saved as:

```
.jmx
```

These files are XML-based and can be shared, version-controlled, and reused.

---

## Best Practices

- Use meaningful names.
- Organize test plans into folders.
- Save frequently.
- Keep test data separate from test plans.
- Store test plans in Git.

---

## Summary

The Test Plan is the foundation of every JMeter project. It acts as the container for all performance testing components and is stored as a `.jmx` file.