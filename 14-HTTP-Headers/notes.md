# Apache JMeter - HTTP Header Manager

## What is HTTP Header Manager?

HTTP Header Manager allows JMeter to send HTTP headers along with requests.

Headers provide additional information to the server about the request.

---

## Common Headers

### Accept

Specifies the expected response format.

Example:

Accept: application/json

---

### Content-Type

Specifies the format of the request body.

Example:

Content-Type: application/json

---

### User-Agent

Identifies the client sending the request.

Example:

User-Agent: Apache JMeter

---

### Authorization

Used to send authentication credentials.

Example:

Authorization: Bearer <token>

(We'll implement this in Lesson 15.)

---

## Why Use Header Manager?

- Send API headers
- Configure content types
- Specify accepted response formats
- Pass authentication information
- Avoid repeating headers in multiple requests

---

## Best Practices

- Add Header Manager at the Thread Group level when multiple requests share the same headers.
- Use meaningful header names.
- Avoid duplicate headers.
- Store dynamic header values in variables when appropriate.

---

## Interview Questions

### What is HTTP Header Manager?

It is a Config Element used to add HTTP headers to requests.

---

### Why do we use Content-Type?

It tells the server the format of the request body.

Example:

application/json

---

### Why do we use Accept?

It tells the server the response format expected by the client.

---

### Can Header Manager be shared?

Yes.

If added at the Thread Group level, all child requests inherit the headers.

---

## Summary

HTTP Header Manager simplifies API testing by allowing common headers to be configured once and reused across multiple HTTP Requests.