# CI/CD with Apache JMeter

## Workflow

Developer

↓

Source Control (GitHub)

↓

CI/CD Tool (Jenkins / GitHub Actions / Azure DevOps)

↓

Run JMeter Test

↓

Generate HTML Dashboard

↓

Publish Results

---

## Benefits

* Automated execution
* Faster feedback
* Consistent testing
* Easier collaboration
* Early detection of performance issues

---

## Common Commands

Run Test

```cmd
jmeter -n -t LoadTest.jmx -l results.jtl
```

Generate Dashboard

```cmd
jmeter -g results.jtl -o Dashboard
```
