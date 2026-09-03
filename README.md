# ECDAT

### Enterprise Cryptographic Discovery & Analysis Tool

> **Discover cryptography. Assess quantum risk. Recommend PQC. Prioritize migration.**

ECDAT is a cybersecurity project focused on helping organizations understand where cryptography is being used, identify potentially quantum-vulnerable cryptographic assets, assess their risk, and support post-quantum cryptography (PQC) migration decisions.

This repository currently contains the **ECDAT proof-of-concept prototype**, developed as a foundation for further development and hackathon evaluation.

---

## 🎯 Problem

Modern enterprise environments use cryptography across many different components, including:

- Source code
- Software dependencies and libraries
- Certificates and keys
- Network and TLS configurations
- Binaries and configuration files
- Applications and infrastructure

As cryptographic usage becomes distributed across these environments, organizations can face difficulty in maintaining visibility over their cryptographic assets.

The challenge is not only to identify cryptographic algorithms, but also to understand:

> **What is being used? Where is it used? How vulnerable is it to future quantum attacks? What should be migrated first?**

---

## 💡 Our Approach

ECDAT aims to convert cryptographic findings into actionable security information.

### Core Workflow

```text
Enterprise Assets
       ↓
Cryptographic Discovery
       ↓
Cryptographic Inventory / CBOM
       ↓
Quantum Risk Assessment
       ↓
PQC Recommendation
       ↓
Migration Prioritization

# ECDAT

### Enterprise Cryptographic Discovery & Analysis Tool

> **Discover cryptography. Assess quantum risk. Recommend PQC. Prioritize migration.**

ECDAT is a cybersecurity project focused on helping organizations understand where cryptography is being used, identify potentially quantum-vulnerable cryptographic assets, assess their risk, and support post-quantum cryptography (PQC) migration decisions.

This repository currently contains the **ECDAT proof-of-concept prototype**, developed for hackathon evaluation and further development.

---

## 🎯 Problem

Modern enterprise environments use cryptography across many different components, including:

- Source code
- Software dependencies and libraries
- Certificates and keys
- Network and TLS configurations
- Binaries and configuration files
- Applications and infrastructure

Cryptographic usage can become difficult to track and assess consistently across these environments.

The challenge is not only to identify cryptographic algorithms, but also to understand:

> **What is being used? Where is it used? How vulnerable is it to future quantum attacks? What should be migrated first?**

## 🔍 Key Capabilities

### 1. Cryptographic Discovery

ECDAT is designed to identify cryptographic usage from supported inputs and environments.

Examples include:

- Cryptographic algorithms
- Key sizes
- Certificates
- TLS configurations
- Cryptographic libraries
- Software dependencies

### 2. Cryptographic Classification

Detected cryptographic findings can be organized using information such as:

- Algorithm
- Key size
- Usage
- Asset
- Library
- Quantum status

Example:

```json
{
  "algorithm": "RSA",
  "key_size": 2048,
  "usage": "TLS certificate",
  "asset": "payment-api",
  "library": "OpenSSL",
  "quantum_status": "vulnerable"
}
