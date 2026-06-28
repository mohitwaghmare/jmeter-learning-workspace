# Generate HTML Dashboard Report

## Step 1

Open Command Prompt.

Navigate to the Apache JMeter `bin` directory.

Example:

```cmd
cd C:\Users\ASUS\OneDrive\Desktop\apache-jmeter-5.6.3\bin
```

---

## Step 2

Run the JMeter test in Non-GUI mode:

```cmd
jmeter -n -t "C:\Users\ASUS\OneDrive\Documents\GitHub\jmeter-learning-workspace\21-HTML-Dashboard-Reports\Dashboard Report Demo.jmx" -l "C:\Users\ASUS\OneDrive\Documents\GitHub\jmeter-learning-workspace\21-HTML-Dashboard-Reports\results.jtl"
```

---

## Step 3

Generate the HTML Dashboard Report:

```cmd
jmeter -g "C:\Users\ASUS\OneDrive\Documents\GitHub\jmeter-learning-workspace\21-HTML-Dashboard-Reports\results.jtl" -o "C:\Users\ASUS\OneDrive\Documents\GitHub\jmeter-learning-workspace\21-HTML-Dashboard-Reports\Dashboard"
```

---

## Step 4

Open:

```
Dashboard/index.html
```

in your preferred web browser.

---

## Output

The generated Dashboard folder contains:

* index.html
* content/
* images/
* statistics.json

---

## Advantages

* Interactive graphs
* Response Time Analysis
* Throughput Charts
* Error Percentage
* Active Threads
* Performance Summary

This is the recommended reporting approach for Apache JMeter performance tests.

# Commands Used

## Check JMeter Version

```cmd
jmeter -v
```

Purpose:
Verifies that Apache JMeter is installed correctly and displays the current version.

---

## Execute Test in Non-GUI Mode

```cmd
jmeter -n -t "C:\Users\ASUS\OneDrive\Documents\GitHub\jmeter-learning-workspace\21-HTML-Dashboard-Reports\Dashboard Report Demo.jmx" -l "C:\Users\ASUS\OneDrive\Documents\GitHub\jmeter-learning-workspace\21-HTML-Dashboard-Reports\results.jtl"
```

Options:

* `-n` → Run in Non-GUI mode.
* `-t` → Specifies the JMeter test plan (`.jmx`).
* `-l` → Specifies the output results file (`.jtl`).

Output:

* `results.jtl`

---

## Generate HTML Dashboard Report

```cmd
jmeter -g "C:\Users\ASUS\OneDrive\Documents\GitHub\jmeter-learning-workspace\21-HTML-Dashboard-Reports\results.jtl" -o "C:\Users\ASUS\OneDrive\Documents\GitHub\jmeter-learning-workspace\21-HTML-Dashboard-Reports\Dashboard"
```

Options:

* `-g` → Reads the JTL results file.
* `-o` → Generates the HTML Dashboard Report in the specified folder.

Output:

```
Dashboard/
├── index.html
├── content/
├── images/
└── statistics.json
```

---

## View the Report

Open:

```
Dashboard/index.html
```

in your preferred web browser.

---

## Notes

* Run commands from the Apache JMeter `bin` directory.
* Use quotation marks if file or folder names contain spaces.
* Non-GUI mode is recommended for performance testing because it uses less CPU and memory.
