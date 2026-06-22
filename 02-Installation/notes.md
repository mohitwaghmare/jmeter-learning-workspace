# Apache JMeter - Installation & Setup

## Prerequisites

Before installing Apache JMeter, ensure Java is installed on your system.

Check Java version:

```bash
java -version
```

Example output:

```
java version "23.0.2"
```

---

## Download Apache JMeter

Download the latest stable release from the official Apache JMeter website.

After downloading:

- Extract the ZIP file.
- Open the extracted folder.
- Navigate to:

```
bin/
```

Run:

Windows

```
jmeter.bat
```

Linux/macOS

```
jmeter
```

---

## JMeter Folder Structure

```
apache-jmeter/
│
├── bin/
├── docs/
├── extras/
├── lib/
├── licenses/
├── printable_docs/
```

### Important folders

**bin**
- Contains executable files.
- Stores JMX test plans.
- Contains report generation utilities.

**lib**
- Third-party libraries.
- JDBC drivers.
- Plugins.

**docs**
- Documentation.

---

## Verify Installation

Launch JMeter.

You should see:

- Menu Bar
- Toolbar
- Test Plan
- Workbench (older versions)
- Left navigation tree
- Right configuration panel

If JMeter opens successfully, the installation is complete.

---

## Recommended Settings

- Keep JMeter updated.
- Avoid running heavy load tests in GUI mode.
- Save test plans regularly.
- Close unnecessary applications before performance testing.

---

## GUI Mode vs Non-GUI Mode

### GUI Mode

Used for:

- Creating test plans
- Debugging
- Learning
- Small tests

### Non-GUI Mode

Used for:

- Large load tests
- CI/CD execution
- Better performance
- HTML report generation

Command example:

```bash
jmeter -n -t TestPlan.jmx -l results.jtl
```

---

## Best Practices

- Design tests in GUI mode.
- Execute large tests in Non-GUI mode.
- Organize test plans in folders.
- Keep test data separate.
- Use version control.

---

## Summary

Apache JMeter requires Java and runs without installation after extracting the ZIP archive. GUI mode is ideal for creating test plans, while Non-GUI mode is recommended for executing performance tests.