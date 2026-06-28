# Apache JMeter - Authentication

## What is Authentication?

Authentication is the process of verifying the identity of a client before allowing access to an application or API.

Most enterprise APIs require authentication to protect sensitive data.

Without valid authentication, the server typically returns:

- 401 Unauthorized
- 403 Forbidden

---

## Why is Authentication Important?

Authentication helps:

- Protect APIs from unauthorized access
- Secure sensitive data
- Verify user identity
- Control access to resources

---

## Common Authentication Types

### API Key Authentication

The client sends a unique API key with each request.

Example:

x-api-key: YOUR_API_KEY

API keys are commonly used by public APIs.

---

### Bearer Token Authentication

The client sends a JWT or access token in the Authorization header.

Example:

Authorization: Bearer eyJhbGciOiJIUzI1NiIs...

This is one of the most common authentication methods for REST APIs.

---

### Basic Authentication

Credentials are sent using Base64 encoding.

Example:

Authorization: Basic dXNlcjpwYXNzd29yZA==

Although simple, it should always be used over HTTPS.

---

### OAuth 2.0

OAuth 2.0 is an authorization framework widely used by enterprise applications.

Typical flow:

- Login
- Receive Access Token
- Send Access Token with subsequent requests

---

## Authentication in JMeter

Authentication is commonly implemented using:

- HTTP Header Manager
- HTTP Authorization Manager
- Variables
- Correlation (for dynamic tokens)

---

## HTTP Header Manager

Common authentication headers:

Authorization: Bearer <token>

x-api-key: YOUR_API_KEY

Content-Type: application/json

Accept: application/json

---

## Common Response Codes

200 OK

Authentication successful.

401 Unauthorized

Authentication failed or missing credentials.

403 Forbidden

Authenticated but access is denied.

---

## Best Practices

- Never hardcode production API keys.
- Store tokens in variables whenever possible.
- Use HTTPS for authenticated requests.
- Remove expired tokens before testing.
- Avoid committing sensitive credentials to Git repositories.

---

## Real-World Example

Login Request

↓

Receive JWT Token

↓

Extract Token

↓

Store in Variable

↓

Authorization: Bearer ${token}

↓

Access Protected APIs

---

## Interview Questions

### What is Authentication?

Authentication verifies the identity of a client before allowing access to an application or API.

---

### Name common authentication methods.

- API Key
- Bearer Token (JWT)
- Basic Authentication
- OAuth 2.0

---

### How is Bearer Token passed?

Using the Authorization header.

Example:

Authorization: Bearer <token>

---

### What is the difference between Authentication and Authorization?

Authentication verifies who the user is.

Authorization determines what the authenticated user is allowed to access.

---

## Summary

Authentication is an essential part of API testing. JMeter supports multiple authentication mechanisms through Header Managers, Authorization Managers, variables, and extractors, enabling secure and realistic API performance testing.