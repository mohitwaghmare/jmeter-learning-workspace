# Apache JMeter - Introduction

## What is Apache JMeter?

Apache JMeter is an open-source performance testing tool developed by the Apache Software Foundation. It is primarily used to measure the performance of web applications, REST APIs, SOAP services, databases, FTP servers, and many other protocols.

Originally designed for web application testing, JMeter has evolved into a powerful load testing and functional testing tool.

---

## Why Use JMeter?

- Free and Open Source
- Easy-to-use Graphical User Interface (GUI)
- Supports Load, Stress, Spike, and Endurance Testing
- Supports multiple protocols
- Generates detailed HTML reports
- Supports distributed testing
- Integrates with Jenkins and CI/CD pipelines
- Highly extensible through plugins

---

## Features

- Multi-threaded load generation
- HTTP/HTTPS testing
- REST API testing
- SOAP API testing
- JDBC Database testing
- FTP testing
- Assertions
- Timers
- CSV Data Driven Testing
- Correlation
- Parameterization
- Command Line Execution
- HTML Dashboard Reports

---

## Types of Performance Testing

### 1. Load Testing
Checks application behavior under expected user load.

Example:
500 users accessing an e-commerce website simultaneously.

---

### 2. Stress Testing
Determines the application's breaking point.

Example:
Increase users until the server crashes.

---

### 3. Spike Testing
Suddenly increases or decreases user load.

Example:
100 users suddenly become 5,000 users.

---

### 4. Endurance (Soak) Testing
Runs the application under load for an extended period.

Example:
500 users continuously for 24 hours.

---

## Common Terminology

Thread
Represents one virtual user.

Thread Group
A collection of virtual users.

Sampler
A request sent to the server.

Listener
Displays test results.

Assertion
Validates server responses.

Timer
Adds delay between requests.

Controller
Controls execution flow.

---

## Advantages

- Open Source
- Platform Independent
- Supports GUI and CLI
- Easy Reporting
- Plugin Support
- Distributed Load Testing

---

## Limitations

- High resource usage on the load generator
- GUI mode is not recommended for large load tests
- Limited browser rendering capabilities
- Not suitable for browser-based UI automation

---

## Real-World Use Cases

- API Performance Testing
- Website Load Testing
- Database Performance Testing
- Microservices Testing
- Capacity Planning
- Regression Performance Testing

---

## Summary

Apache JMeter is one of the most widely used performance testing tools. It enables QA engineers to simulate thousands of virtual users, analyze application performance, identify bottlenecks, and generate detailed reports for performance analysis.