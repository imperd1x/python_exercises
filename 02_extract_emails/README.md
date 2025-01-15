# Extract Emails from Logs

## Overview
This exercise involves analyzing a log file to extract all email addresses and writing the unique addresses to an output file.

---

## Objectives
1. Read a log file and extract email addresses using regular expressions.
2. Remove duplicate email addresses.
3. Write the unique email addresses to a new file named `emails_extracted.txt`.

---

## Requirements
- **Input File Format:** The log file may contain lines such as:
  User1 accessed the system. Email: user1@example.com  
  Admin account used: admin@example.com for login.  
  Alert! Invalid access detected from root@maliciousdomain.org

---

## Example Output
For the following log file:

User1 accessed the system. Email: user1@example.com
Admin account used: admin@example.com for login. 
Alert! Invalid access detected from root@maliciousdomain.org



The output file `emails_extracted.txt` will contain:
user1@example.com 
admin@example.com 
root@maliciousdomain.org


---

## Instructions
1. Write a Python script to:
   - Open the log file.
   - Extract email addresses using a regular expression.
   - Remove duplicate emails.
   - Write the unique emails to `emails_extracted.txt`.
2. Run the script with the log file as input.

---

## Useful References
- [Python Regular Expressions](https://docs.python.org/3/library/re.html)
- [Python File Handling](https://docs.python.org/3/tutorial/inputoutput.html#reading-and-writing-files)

---

**Good Luck!**
