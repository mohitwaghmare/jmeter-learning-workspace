# GitHub Actions Integration

## Sample Workflow

```yaml
name: JMeter Test

on:
  push:
    branches:
      - main

jobs:
  performance-test:
    runs-on: windows-latest

    steps:
      - uses: actions/checkout@v4

      - name: Run JMeter Test
        run: |
          jmeter -n -t LoadTest.jmx -l results.jtl
```

---

## Workflow

Developer Push

↓

GitHub Repository

↓

GitHub Actions

↓

Run JMeter

↓

Generate Results

↓

Publish Reports

---

## Benefits

* Automated performance testing
* Version-controlled workflows
* Faster feedback
* Easy collaboration
* Continuous quality assurance
