# 🔐 Information Security Lab 2 - Spring 2025

This repository contains solutions for **Lab 2** completed as part of the **CIS 675 - Information Security** course at **Cleveland State University**. The lab focuses on foundational cybersecurity concepts, including a simulated **Spectre Attack**, **Port Scanning** using Metasploit and Nmap, and various **Cryptographic operations**. All exercises were executed in a secure virtual lab environment.

---

## 📁 Lab Structure

The lab is divided into three key modules:

### 1️⃣ Spectre Attack Simulation
**Objective:** Understand speculative execution vulnerabilities and simulate a side-channel attack to extract sensitive data.

- **Environment:** Kali Linux (Sandbox), `spectre.c` exploit
- **Steps:**
  - Download and compile `spectre.c`
  - Execute the program repeatedly to leak secret data via cache timing
- **Key Concepts:** Speculative execution, cache side-channel, CPU vulnerability

**Deliverables:**
- Screenshot of downloaded file
- Compilation command (`gcc -msse2 spectre.c`)
- Execution and output showing leaked secret
- Annotated explanation of how the CPU leaks the value

📎 *Located in* `Spectre-Attack/`  
📷 *Screenshots in* `Spectre-Attack/screenshots/`

---

### 2️⃣ Port Scanning with Nmap & Metasploit
**Objective:** Identify open ports, running services, and OS details using Nmap and Metasploit tools.

- **Tools Used:** Nmap, Metasploit Framework, Dmitry
- **Tasks Performed:**
  - Host discovery using `nmap -sn`
  - Service and OS detection using `nmap -sV -O`
  - Database-integrated scans using `db_nmap`
  - Metasploit info gathering with `msfconsole`
  - Bonus scan using Dmitry with full option set (`-winsepfb`)
- **Key Concepts:** Network scanning, enumeration, service fingerprinting, attack surface identification

**Deliverables:**
- Nmap scans of specific and top 100 ports
- Screenshots from Metasploit’s console
- Dmitry results showing DNS, WHOIS, and banner grabbing

📎 *Located in* `Port-Scanning/`  
📷 *Screenshots in* `Port-Scanning/screenshots/`

---

### 3️⃣ Cryptography, Encoding & Numbering Systems
**Objective:** Explore encoding, hashing, and both symmetric & asymmetric encryption mechanisms in Linux.

- **Tools Used:** OpenSSL, md5sum, sha1sum, sha512sum, md5deep
- **Tasks Performed:**
  - Generate and compare hash values (MD5, SHA1, SHA512)
  - Base64 encode/decode files
  - AES-256-CBC encryption and decryption
  - Multi-stage encoding + encryption
  - Asymmetric key generation and encryption/decryption using RSA

- **Key Concepts:**
  - Hash function collision resistance
  - File integrity via hashes
  - Confidentiality through symmetric & asymmetric encryption
  - Base64 as an encoding layer (not encryption)

**Deliverables:**
- Scripts and commands for each operation
- Screenshots showing hash consistency and decryption accuracy
- Explanations for encryption utilities used (e.g., OpenSSL)

📎 *Located in* `Cryptography/`  
📷 *Screenshots in* `Cryptography/screenshots/`

---

## 💻 Technologies & Tools
- Kali Linux
- Metasploit Framework
- Nmap
- OpenSSL
- Dmitry
- GNU Bash
- md5sum / sha1sum / sha512sum

---

## 🛡️ Disclaimers
All attacks, simulations, and security testing shown in this repository were performed in an isolated, controlled lab environment for academic purposes only. **No live networks or unauthorized systems were targeted.**

---

## 👩‍💻 Author

**Krutika Diwathe**  
Master’s in Computer Science – Cleveland State University  
Course: CIS 675 – Information Security  
GitHub: [github.com/krutika-dev](https://github.com/krutika-dev)

---

## 🔗 License

This project is licensed for **academic showcase and demonstration** purposes only. No part of this repository may be reused in live environments or for malicious activity.
