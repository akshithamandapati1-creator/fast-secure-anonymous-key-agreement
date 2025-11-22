# Fast Secure and Anonymous Key Agreement Against Bad Randomness

This project implements a **fast, secure, and anonymous authenticated key agreement (AKA) protocol** designed to resist **bad randomness attacks** in cloud-computing environments. It is based on a certificateless public key cryptography (CL-PKC) model and supports **0-RTT (Zero Round Trip Time)** communication, enabling users to establish secure channels with cloud service providers (CSPs) efficiently.

---

## 🚀 Features

### ✔ Certificate-less Public Key Cryptography (CL-PKC)
Eliminates the need for certificates and reduces management overhead.

### ✔ 0-RTT Key Agreement
Enables a cloud user to send encrypted data **simultaneously** with the key-negotiation message.

### ✔ Security Against Bad Randomness
The protocol is resistant to:
- Weak or predictable random numbers  
- Malicious hypervisors predicting PRG states  
- Backdoored pseudorandom generators (like Dual EC PRG)

### ✔ User Privacy Protection
Ensures anonymity by preventing attackers (even KGC) from linking multiple messages to the same user.

---

## 📘 Overview

Cloud computing introduces challenges due to open networks, virtualization, and possible attacks such as:
- Impersonation  
- Eavesdropping  
- Randomness manipulation  
- Session-key compromise  

This project implements a robust solution that:
- Avoids the certificate management problems of traditional PKI systems  
- Provides secure, anonymous, and efficient key exchange  
- Ensures forward and backward secrecy  
- Keeps latency extremely low (≈2x faster than DH-based one-RTT protocols)

---

## 🏗 System Architecture

The project includes major components:

- **User Module** – Performs registration, login, key generation, and encrypted file operations  
- **Cloud Service Provider (CSP)** – Stores data, verifies requests, manages sessions  
- **Key Generation Center (KGC)** – Partially generates keys in the CL-PKC model  
- **Data Owner Module** – Uploads and manages secure cloud data  

### Included Design Diagrams
- Flowcharts  
- Class Diagram  
- DFD  
- System Architecture Diagram  

---

## 🛠 Technology Stack

| Component | Technology |
|----------|------------|
| Language | Java (J2EE: JSP, Servlets) |
| Frontend | JSP, HTML, CSS, JavaScript |
| Backend | MySQL |
| Server | Apache Tomcat / WebLogic |
| Additional Tools | JDBC, ODBC, JFreeChart |

---

## 📑 Installation Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/<akshithamandapati1-creator>/fast-secure-anonymous-key-agreement.git
cd fast-secure-anonymous-key-agreement
