# Apache JMeter - Assertions

## What is an Assertion?

An Assertion is used to validate the response returned by the server after a request is executed.

It helps verify that the application is returning the expected data and not just a successful HTTP status code.

---

## Why Use Assertions?

Assertions help to:

- Validate API responses
- Verify response content
- Detect failures automatically
- Improve test reliability
- Prevent false positives

Example:

A request may return **200 OK**, but the response body could contain incorrect data. Assertions ensure the response is both successful and correct.

---

## Types of Assertions in JMeter

- Response Assertion
- Duration Assertion
- Size Assertion
- XML Assertion
- JSON JMESPath Assertion
- MD5Hex Assertion

Among these, **Response Assertion** is the most commonly used.

---

## Response Assertion

A Response Assertion validates one or more parts of the server response.

It can verify:

- Response Text
- Response Code
- Response Message
- Response Headers
- Request Headers
- URL

---

## Pattern Matching Rules

JMeter supports different matching options:

- Contains
- Matches (Regular Expression)
- Equals
- Substring
- Not

Example:

Response contains:

```
Leanne Graham
```

If the response includes this value, the assertion passes.

---

## Assertion Results

### Passed Assertion

- Request is marked as successful.
- Green indicator in View Results Tree.

### Failed Assertion

- Request is marked as failed.
- Red indicator in View Results Tree.
- Displays an assertion failure message.

---

## Best Practices

- Validate only important response data.
- Keep assertions simple and meaningful.
- Avoid unnecessary assertions in high-load tests.
- Use descriptive names for assertions.
- Test both positive and negative scenarios.

---

## Real-World Example

Suppose a User API returns:

```json
{
  "id": 1,
  "name": "Leanne Graham"
}
```

A Response Assertion checks whether the response contains:

```
Leanne Graham
```

If the name changes unexpectedly or is missing, the assertion fails, indicating a potential issue with the application.

---

## Interview Questions

### What is an Assertion?

An Assertion validates that the server response matches the expected result.

---

### Why are Assertions important?

They ensure that requests return the correct data, not just a successful HTTP status code.

---

### What is the most commonly used Assertion?

Response Assertion.

---

### Can a request return HTTP 200 and still fail?

Yes.

If the response content is incorrect, the Response Assertion will fail even though the HTTP status code is 200.

---

## Summary

Assertions are essential for validating server responses in JMeter. They help ensure that APIs and applications return the expected results and make performance tests more reliable and meaningful.