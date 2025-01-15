# File Hashing and Verification

## Overview
This exercise involves verifying the integrity of a file by calculating its hash and comparing it with a known hash value.

---

## Objectives
1. Calculate the **SHA-256 hash** of a file.
2. Compare the calculated hash with a known hash to verify file integrity.
3. Print whether the file's integrity is verified or compromised.

---

## Requirements
- **Input File:** Any file for which you want to calculate the hash.
- **Known Hash:** A precomputed SHA-256 hash value to compare with.

---

## Example Output
For the file `example.txt` containing:
Platform Security


If the known hash is:
b44e9c7e141e4cb55ae89b1bc338b489a9d2457e8c306e88243f16b1743f6fef


The script will output:
Integrity verified! File hash matches the known hash: b44e9c7e141e4cb55ae89b1bc338b489a9d2457e8c306e88243f16b1743f6fef


---

## Instructions
1. Write a Python script to:
   - Read the input file and calculate its SHA-256 hash.
   - Compare the calculated hash with the known hash.
   - Print whether the file's integrity is verified or compromised.
2. Run the script with the input file and known hash as arguments.

---

## Useful References
- [Python hashlib Library](https://docs.python.org/3/library/hashlib.html)
- [File Handling in Python](https://docs.python.org/3/tutorial/inputoutput.html#reading-and-writing-files)

---

**Good Luck!**
