# Count IP Addresses in Logs

## Overview
This exercise focuses on analyzing log files to count the frequency of each IP address. The script will identify the top 3 most frequent IP addresses in the log file.

---

## Objectives
1. Read a log file and extract IP addresses from each line.
2. Count the frequency of each IP address.
3. Print the top 3 most frequent IP addresses.

---

## Requirements
- **Input File Format:** The log file should contain lines in the format:
  192.168.1.1 - - [10/Jan/2025:15:45:27 +0000] "GET / HTTP/1.1" 200 1234

---

## Example Output
For the following log file:
192.168.1.1 - - [10/Jan/2025:15:45:27 +0000] "GET / HTTP/1.1" 200 1234 
192.168.1.2 - - [10/Jan/2025:15:46:10 +0000] "GET /login HTTP/1.1" 200 532 
192.168.1.1 - - [10/Jan/2025:15:47:05 +0000] "POST /form HTTP/1.1" 403 256


The output will be:
192.168.1.1: 2 
192.168.1.2: 1


---

## Instructions
1. Write a Python script to:
   - Open the log file.
   - Extract IP addresses from each line.
   - Count the occurrences of each IP address.
   - Print the top 3 most frequent IP addresses.
2. Run the script with the log file as input.

---

## Useful References
- [Python String Methods](https://docs.python.org/3/library/stdtypes.html#string-methods)
- [Python Collections - Counter](https://docs.python.org/3/library/collections.html#collections.Counter)

---

**Good Luck!**
