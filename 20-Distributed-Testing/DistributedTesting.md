# Apache JMeter - Distributed Testing

## Overview

Distributed Testing allows multiple Apache JMeter machines to work together and generate load against the same target application.

Instead of using a single machine, JMeter distributes the workload across multiple systems, allowing large-scale performance testing.

---

## Architecture

```
                 MASTER

            Apache JMeter

                  │

     ┌────────────┼────────────┐

     │            │            │

 WORKER 1     WORKER 2     WORKER 3

 Apache       Apache       Apache

 JMeter       JMeter       JMeter

     │            │            │

     └────────────┼────────────┘

             Target Application
```

---

## Components

### Master

* Controls test execution.
* Sends the test plan to Worker machines.
* Starts and stops the test.
* Collects test results.

### Worker (Slave)

* Receives the test plan.
* Executes requests.
* Generates virtual users.
* Sends results back to the Master.

---

## Requirements

* Same JMeter version on all machines.
* Same Java version.
* Same plugins.
* Same test data (CSV files, JMX files).
* Network connectivity.
* Open RMI ports.
* Time synchronization between machines.

---

## Configuration Steps

1. Install Apache JMeter on every machine.
2. Copy the test plan (.jmx) and required files.
3. Configure `remote_hosts` in `jmeter.properties`.
4. Start `jmeter-server` on every Worker machine.
5. Start the test from the Master machine using:

   * **Run → Remote Start All**
   * or the JMeter CLI.

---

## Advantages

* Supports thousands of virtual users.
* Better CPU and memory utilization.
* Scalable performance testing.
* Suitable for enterprise applications.

---

## Limitations

* Requires multiple machines.
* More setup and maintenance.
* Network configuration is required.
* Workers must remain synchronized.

---

## Best Practices

* Use identical JMeter and Java versions.
* Execute tests in Non-GUI mode.
* Monitor CPU, Memory, and Network utilization.
* Keep all Worker machines on a stable network.
* Store test plans and data consistently across machines.

---

## Real-World Example

A banking application expects 15,000 concurrent users during salary credit day.

Instead of running all users from one laptop:

* Master Machine
* 5 Worker Machines
* 3,000 Users per Worker

Total:

15,000 Virtual Users

This approach distributes the workload efficiently and prevents a single machine from becoming a bottleneck.

---

## Conclusion

Distributed Testing is an advanced JMeter feature used for large-scale performance testing. It enables multiple systems to work together, making it possible to simulate thousands of concurrent users while maintaining stable resource utilization.
