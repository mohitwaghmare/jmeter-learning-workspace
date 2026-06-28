# Jenkins Integration

## Steps

1. Install Jenkins.
2. Install Java.
3. Install Apache JMeter.
4. Create a Jenkins Job or Pipeline.
5. Execute JMeter in Non-GUI mode.
6. Archive the HTML Dashboard Report.

---

## Sample Pipeline

```groovy
pipeline {
    agent any

    stages {
        stage('Run JMeter Tests') {
            steps {
                bat 'jmeter -n -t LoadTest.jmx -l results.jtl'
            }
        }
    }
}
```

---

## Benefits

* Automated execution
* Scheduled performance tests
* Historical build records
* HTML report publishing
* Easy integration with CI/CD
