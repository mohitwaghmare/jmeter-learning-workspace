# Apache JMeter - Functions

## What are Functions?

Functions are built-in utilities that generate dynamic values during test execution.

They help avoid hardcoded values and make test plans more flexible.

---

## Common Functions

### __Random()

Generates a random number.

Example:

${__Random(100,999,)}

---

### __UUID()

Generates a unique identifier.

Example:

${__UUID()}

Useful for creating unique usernames or transaction IDs.

---

### __time()

Returns the current date and time.

Example:

${__time(yyyy-MM-dd HH:mm:ss,)}

---

### __counter()

Generates an incrementing counter.

Example:

${__counter(FALSE,)}

---

## Why Use Functions?

- Generate dynamic data
- Avoid duplicate values
- Create unique test data
- Improve automation flexibility

---

## Best Practices

- Use UUIDs for unique identifiers.
- Use Random for test data variation.
- Use Time for logging and timestamps.
- Use Counter for sequential values.

---

## Interview Questions

### What are Functions in JMeter?

Functions generate dynamic values during test execution.

---

### Name some commonly used Functions.

- __Random()
- __UUID()
- __time()
- __counter()

---

### Why use UUID?

To generate unique values for every request.

---

## Summary

Functions help create realistic and reusable JMeter test plans by generating dynamic values such as random numbers, timestamps, counters, and UUIDs.