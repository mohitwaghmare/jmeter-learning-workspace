# Apache JMeter - Correlation

## What is Correlation?

Correlation is the process of extracting dynamic values from one server response and using them in subsequent requests.

Dynamic values include:

- Session IDs
- Authentication Tokens
- User IDs
- Order IDs
- CSRF Tokens

Without correlation, many automated performance tests fail because dynamic values change for every request.

---

## JSON JMESPath Extractor

The JSON JMESPath Extractor extracts values from JSON responses.

Example:

Response

```json
[
  {
    "id": 1,
    "name": "Leanne Graham"
  }
]
```

JMESPath Expression

```
[0].id
```

Extracted Value

```
1
```

Variable

```
${userId}
```

---

## Why is Correlation Important?

- Eliminates hardcoded values.
- Handles dynamic application data.
- Makes tests reusable.
- Simulates real user behavior.

---

## Common Dynamic Values

- Session IDs
- JWT Tokens
- OAuth Tokens
- User IDs
- Order IDs
- Cart IDs

---

## Best Practices

- Use meaningful variable names.
- Verify extracted values using View Results Tree.
- Extract only the required fields.
- Prefer JSON Extractors for JSON APIs.

---

## Interview Questions

### What is Correlation?

Correlation is the process of capturing dynamic values from one request and using them in subsequent requests.

---

### Why is Correlation required?

Modern applications generate dynamic values that change for every user or request. Correlation allows automated tests to continue working by extracting and reusing those values.

---

### Which extractor is used for JSON responses?

JSON JMESPath Extractor.

---

## Summary

Correlation is one of the most important concepts in JMeter. It enables dynamic, reusable, and realistic performance tests by extracting data from responses and passing it to future requests.