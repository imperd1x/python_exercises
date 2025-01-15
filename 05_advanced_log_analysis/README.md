# Advanced Log Analysis

## Overview
This exercise challenges you to perform advanced log analysis by parsing a large log file, detecting anomalies, and extracting insights. You will focus on identifying patterns such as unauthorized access attempts, error rate spikes, and usage trends.

---

## Objectives
1. Parse a large log file and analyze its contents.
2. Identify anomalies, such as:
   - Unauthorized access attempts.
   - Suspicious IP activity (e.g., too many requests in a short time).
   - High error rates (HTTP 4xx or 5xx responses).
3. Generate a summary report with key insights.

---

## Requirements
- **Input File Format:** The log file may contain lines in the format:

192.168.1.2 - - [10/Jan/2025:15:01:10 +0000] "POST /login HTTP/1.1" 403 512
192.168.1.3 - - [10/Jan/2025:15:02:45 +0000] "GET /admin HTTP/1.1" 403 256
192.168.1.100 - - [10/Jan/2025:15:03:27 +0000] "GET /index.html HTTP/1.1" 200 1024
192.168.1.100 - - [10/Jan/2025:15:03:55 +0000] "GET /dashboard HTTP/1.1" 200 2048
...

---

## Expected Output
1. A summary of anomalies, including:
 - The top 3 IPs with the most unauthorized access attempts.
 - The percentage of requests resulting in HTTP 4xx and 5xx errors.
 - Any IPs with an unusually high number of requests (e.g., >100 in a minute).
2. A detailed report saved as `log_analysis_report.txt`.

Example Output:

--- Log Analysis Report 
--- Date Range: 10/Jan/2025 to 12/Jan/2025 
Total Requests: 1200

Top Unauthorized Access Attempts (HTTP 403):
192.168.1.2 - 15 attempts
192.168.1.3 - 12 attempts
10.0.0.5 - 10 attempts

Error Rates:
HTTP 4xx: 15.6% (187 requests)
HTTP 5xx: 2.3% (28 requests)

Suspicious IP Activity: 
192.168.1.100 made 320 requests on 10/Jan/2025 between 15:00 and 16:00.

---

## Instructions
1. Write a Python script to:
   - Open and read the log file.
   - Parse log entries to extract:
     - IP addresses.
     - Timestamps.
     - HTTP response codes.
   - Identify anomalies based on the objectives.
   - Generate a summary report as `log_analysis_report.txt`.
2. Run the script with the log file as input.

---

## Hints
1. Use Python's `datetime` module to handle and analyze timestamps.
2. Use `collections.Counter` to identify patterns in IP addresses and response codes.
3. Use a dictionary to group and count requests by IP and timestamp.

---

## Useful References
- [Python datetime Module](https://docs.python.org/3/library/datetime.html)
- [Python Counter - collections](https://docs.python.org/3/library/collections.html#collections.Counter)
- [Log Analysis Best Practices](https://example.com/log-analysis-best-practices) *(Replace with actual link)*

---

**Good Luck!**
