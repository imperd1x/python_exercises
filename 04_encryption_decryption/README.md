# Python Encryption and Decryption Challenge

## Overview
This challenge involves encrypting and decrypting data using the **AES (Advanced Encryption Standard)** algorithm in **CBC (Cipher Block Chaining)** mode. You'll use the Python `cryptography` library to secure sensitive data and verify the integrity of encryption and decryption processes.

---

## Objectives
1. Encrypt a plaintext using AES encryption in CBC mode with:
   - A randomly generated 16-byte key.
   - A randomly generated 16-byte Initialization Vector (IV).
2. Decrypt the ciphertext back to its original plaintext to verify the encryption process.
3. Print the encryption key, IV, ciphertext, and decrypted plaintext in a clear and readable format.

---

## Requirements
- **Input Text**: Platform Security Challenge
- **Python Library**: Use the `cryptography` library.

---

## Expected Output
1. A randomly generated 16-byte key and IV, displayed in hexadecimal format.
2. The ciphertext resulting from encrypting the input text, displayed in hexadecimal format.
3. The decrypted plaintext, which should match the original input.

Example Output:  
Key: 4fe5c5a6e54f19d4bb9a6f8dbe8c46f8  
IV: 5a9c3b8e5af15c1bb7c82db7d3e39f29  
Ciphertext: 3e4b9c5e21354f8ba32a19fdfb9e6a32b9a0db12c85c57b7  
Decrypted Plaintext: Platform Security Challenge

---

## Instructions
1. Install the `cryptography` library: 
    pip install cryptography
2. Write a Python script that:
   - Encrypts the input text using AES-CBC.
   - Decrypts the ciphertext back to plaintext.
3. Ensure that the output includes:
   - The generated encryption key and IV.
   - The ciphertext (in hexadecimal format).
   - The decrypted plaintext.
4. Run the script and verify the output.

---

## Hints
1. Use the `cryptography.hazmat.primitives.ciphers` module to implement AES encryption.
2. Padding may be required for AES encryption since the plaintext length must be a multiple of the block size (16 bytes).
3. Use `os.urandom` to generate secure random bytes for the key and IV.

---

## Useful References
- [cryptography Documentation](https://cryptography.io/en/latest/)
- [AES Encryption and Decryption in Python](https://cryptography.io/en/latest/hazmat/primitives/symmetric-encryption/)

---

**Good Luck!**
