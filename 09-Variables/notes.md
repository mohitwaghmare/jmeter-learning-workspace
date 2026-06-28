# Apache JMeter - User Defined Variables

## What are User Defined Variables?

User Defined Variables (UDVs) allow you to store reusable values in one place and reference them throughout a JMeter test plan.

Instead of hardcoding values such as URLs, server names, or endpoints, you define them once and reuse them.

---

## Why Use Variables?

- Reduce duplication
- Easy maintenance
- Improve readability
- Simplify environment changes
- Reuse values across multiple requests

---

## Variable Syntax

Variables are referenced using:

${variableName}

Example:

${server}

${endpoint}

---

## Example

Variable:

server = jsonplaceholder.typicode.com

Request:

Protocol: https

Server: ${server}

Path: /users

Actual Request:

https://jsonplaceholder.typicode.com/users

---

## Common Use Cases

- Base URL
- API Version
- Username
- Password
- Environment Name
- Endpoints

---

## User Defined Variables vs CSV Data Set Config

### User Defined Variables

- Static values
- Defined inside JMeter
- Same value for every request

### CSV Data Set Config

- Dynamic values
- Loaded from external CSV files
- Different value for each request

---

## Best Practices

- Use meaningful variable names.
- Avoid hardcoding URLs.
- Group related variables together.
- Use variables for reusable values.

---

## Interview Questions

### What are User Defined Variables?

Variables used to store reusable static values within a JMeter test plan.

---

### How do you reference a variable?

Using:

${variableName}

---

### When should you use User Defined Variables?

When multiple requests use the same value, such as a base URL or endpoint.

---

## Summary

User Defined Variables improve test maintainability by allowing reusable values to be stored in one place and referenced throughout the test plan.