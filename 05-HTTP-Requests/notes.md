# Apache JMeter - HTTP Request Sampler

## What is an HTTP Request?

An HTTP Request Sampler sends requests from JMeter to a server using HTTP or HTTPS protocols.

It is one of the most commonly used samplers in JMeter.

---

## Supported HTTP Methods

- GET
- POST
- PUT
- PATCH
- DELETE
- HEAD
- OPTIONS

---

## Main Fields

### Protocol

Specifies the protocol.

Examples:

- http
- https

---

### Server Name or IP

Target server.

Example:

reqres.in

---

### Method

Specifies the HTTP method.

Example:

GET

---

### Path

API endpoint.

Example:

/api/users?page=2

---

## Listener

The View Results Tree listener displays:

- Request
- Response
- Headers
- Response Code
- Response Message
- Response Time

---

## Best Practices

- Use meaningful sampler names.
- Keep URLs configurable where possible.
- Remove heavy listeners before large load tests.
- Test functionality first, then increase load.

---

## Summary

The HTTP Request Sampler is used to send requests to web servers and APIs. Combined with Thread Groups and Listeners, it forms the foundation of most JMeter performance tests.