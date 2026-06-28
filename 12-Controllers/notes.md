# Apache JMeter - Logic Controllers

## What is a Logic Controller?

Logic Controllers determine the order and conditions under which requests execute.

They help organize and control test execution.

---

## Common Logic Controllers

### Simple Controller

Groups related requests.

Useful for improving readability.

---

### Loop Controller

Repeats child requests a specified number of times.

---

### Once Only Controller

Executes child requests only once, regardless of the Thread Group loop count.

---

### If Controller

Executes requests only when a specified condition evaluates to true.

---

## Why Use Logic Controllers?

- Organize requests
- Repeat requests
- Execute conditional logic
- Improve maintainability
- Simulate real user workflows

---

## Best Practices

- Use meaningful controller names.
- Group related requests together.
- Keep nesting levels simple.
- Avoid unnecessary complexity.

---

## Interview Questions

### What is a Logic Controller?

A Logic Controller controls how requests execute within a JMeter test plan.

---

### What is the difference between a Thread Group and a Loop Controller?

A Thread Group controls virtual users and overall execution.

A Loop Controller repeats only the requests placed inside it.

---

### Which controller executes only once?

Once Only Controller.

---

## Summary

Logic Controllers organize and control request execution. They help create realistic user flows and improve test plan readability.