# Apache JMeter - CSV Data Set Config

## What is CSV Data Set Config?

CSV Data Set Config allows JMeter to read test data from an external CSV file.

Instead of hardcoding values inside requests, variables can be loaded dynamically from the CSV file.

---

## Why Use It?

- Data Driven Testing
- Easy maintenance
- Reusable test plans
- Supports large datasets
- Improves scalability

---

## Variable Syntax

Variables are referenced using:

${variableName}

Example:

${id}

---

## Example CSV

id

1

2

3

4

5

---

## Example Request

/users/${id}

Actual Requests

/users/1

/users/2

/users/3

/users/4

/users/5

---

## Common Properties

Filename

Location of CSV file.

Variable Names

Column names.

Delimiter

Usually comma (,)

Recycle on EOF

Restart reading after end of file.

Stop Thread on EOF

Stops execution after file ends.

Sharing Mode

Controls how multiple threads share CSV data.

---

## Best Practices

Store CSV files separately.

Use meaningful variable names.

Never hardcode large datasets.

Use UTF-8 encoding.

Keep CSV clean and organized.

---

## Summary

CSV Data Set Config is one of the most powerful Config Elements in JMeter. It enables data-driven testing by supplying request data from external CSV files.