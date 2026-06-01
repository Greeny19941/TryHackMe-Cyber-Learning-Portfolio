# 🔐 Cryptography Concepts 

## Overview
This lab provided a short introduction to fundamental cryptography concepts, reinforcing key ideas around encryption, decryption, and secure communication. It focused on both symmetric and asymmetric encryption, along with real-world applications such as HTTPS.

---

## 📌 Core Concepts

### Plaintext vs Ciphertext
- **Plaintext**: Original readable message
- **Ciphertext**: Encrypted, unreadable version of the message

Encryption transforms plaintext → ciphertext, while decryption reverses it.

---

## 🔑 Encryption Types

### Symmetric Encryption
- Uses the **same key** for both encryption and decryption
- Example used: **Caesar Cipher**
- If the shift value is known, encryption/decryption is trivial
- Vulnerable to key distribution problems

🧠 Key takeaway:
> Fast and efficient, but insecure key sharing is a major weakness

---

### Asymmetric Encryption
- Uses a **key pair**:
  - Public key (shared openly)
  - Private key (kept secret)
- Data encrypted with one key can only be decrypted with the other

#### Real-world usage:
- Used in **HTTPS** secure web communication

---

## 🌐 HTTPS & Key Exchange

How secure web browsing works:

1. Browser requests website’s **public key**
2. Website provides certificate containing public key
3. Browser verifies certificate via a **Certificate Authority (CA)**
4. Once trusted:
   - Browser and server establish a **shared session key**
5. Symmetric encryption is then used for performance

🧠 Key takeaway:
> Asymmetric encryption is used to securely exchange keys, not for bulk data transfer

---

## 🏛️ Certificate Authorities (CA)

- Trusted third-party organisations
- Validate ownership of public keys
- Ensure authenticity of websites

If valid:
- Browser displays 🔒 padlock icon
- Connection is considered secure

---

## 🔁 Key Distribution Problem

### Problem:
- How do two parties securely share a secret key without interception?

### Solution:
- Asymmetric encryption removes the need to directly share the secret key
- Secure key exchange enables safe symmetric encryption afterwards

---

## 🔐 Caesar Cipher (Practical Example)

- Simple substitution cipher
- Each letter is shifted by a fixed number
- Example: shift of 3
  - A → D
  - B → E

### Limitations:
- Only 25 possible shifts (0–25)
- Easily brute-forced
- Not secure for modern use

---

## ⏱️ Human vs Computer Encryption

The lab demonstrated:
- Manual encryption/decryption is slow and error-prone
- Computers perform cryptographic operations instantly
- Even small brute-force tasks (e.g., 26 Caesar shifts) become tedious manually

---

## 🧠 Key Takeaways

- Symmetric encryption is fast but requires secure key exchange
- Asymmetric encryption solves the key distribution problem
- HTTPS combines both methods for secure communication
- Certificate Authorities provide trust verification
- Classical ciphers (like Caesar Cipher) are educational but insecure

---

## 🧪 Lab Context
- Platform: TryHackMe  
- Topic: Cryptography Fundamentals  
- Difficulty: Introductory / Foundational  

---

## 🚀 Summary
This lab reinforced the importance of modern cryptographic systems and how they balance security and performance using a hybrid approach of asymmetric and symmetric encryption.
