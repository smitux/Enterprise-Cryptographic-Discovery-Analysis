# ECDAT

### Enterprise Cryptographic Discovery & Analysis Tool

> **Discover cryptography. Assess quantum risk. Recommend PQC. Prioritize migration.**

ECDAT is a cybersecurity project focused on helping organizations discover cryptographic usage, identify potentially quantum-vulnerable cryptographic assets, assess their risk, and support post-quantum cryptography (PQC) migration decisions.

This repository currently contains the **ECDAT proof-of-concept prototype**, developed as a foundation for further development and hackathon evaluation.

---

## 🎯 Problem

Modern enterprise environments use cryptography across different components, including:

- Source code
- Software dependencies and libraries
- Certificates and keys
- Network and TLS configurations
- Binaries and configuration files
- Applications and infrastructure

As cryptographic usage becomes distributed across these environments, maintaining visibility and assessing cryptographic risk can become difficult.

The challenge is not only to identify cryptographic algorithms, but also to understand:

> **What is being used? Where is it used? How vulnerable is it to future quantum attacks? What should be migrated first?**

---

## 💡 Our Approach

ECDAT aims to convert cryptographic findings into actionable security information.

### Core Workflow

**Enterprise Assets → Cryptographic Discovery → Cryptographic Inventory / CBOM → Quantum Risk Assessment → PQC Recommendation → Migration Prioritization**

---

## 🔍 Key Capabilities

### 1. Cryptographic Discovery

Identifies supported cryptographic usage from project and system inputs.

Examples include:

- Cryptographic algorithms
- Key sizes
- Certificates
- TLS configurations
- Cryptographic libraries
- Software dependencies

### 2. Cryptographic Classification

Organizes detected findings using information such as:

- Algorithm
- Key size
- Usage
- Asset
- Library
- Quantum status

### 3. Cryptographic Inventory / CBOM

Organizes discovered cryptographic components into a structured inventory that can be used for further analysis and migration planning.

### 4. Quantum Risk Assessment

Considers contextual factors such as:

- Algorithm vulnerability
- Key size
- Cryptographic usage
- Data sensitivity
- Data shelf-life
- Business criticality
- System exposure
- Migration complexity
- Quantum threat timeline

These factors can contribute to a **Quantum Risk Score on a 0–100 scale**.

### 5. PQC Recommendation

Maps potentially quantum-vulnerable cryptographic usage to suitable post-quantum alternatives based on its cryptographic purpose.

Examples:

- RSA / key establishment → ML-KEM or hybrid approaches
- ECDSA / digital signatures → ML-DSA or other suitable signature schemes

### 6. Migration Prioritization

Helps determine which cryptographic assets should be addressed first based on their risk and surrounding context.

---

## 🧪 Current Prototype

This repository contains the **ECDAT proof-of-concept prototype**.

The current prototype focuses on demonstrating the core concept and workflow rather than representing the complete enterprise-scale implementation.

### Prototype Workflow

**Discover → Identify → Analyze → Risk Score → Recommend → Prioritize**

The project will be expanded with additional capabilities as development progresses.

---

## 🏗️ Proposed Architecture

The broader ECDAT concept follows this workflow:

**Enterprise Assets → Cryptographic Discovery → Cryptographic Inventory / CBOM → Quantum Risk Assessment → PQC Recommendation → Migration Prioritization**

The proposed architecture represents the intended direction of the project and may be expanded as additional components are developed.

---

## 📊 Example Risk Assessment

| Asset | Cryptography | Risk Score | Priority |
|---|---|---:|---|
| Payment API | RSA-2048 | 92 | Critical |
| Legacy Server | Legacy Crypto | 83 | High |
| Identity Service | ECDSA-P256 | 74 | High |
| Internal Application | — | 61 | Medium |
| Analytics DB | AES-256 | 38 | Low |

> **Note:** These values are illustrative examples used to demonstrate the proposed risk-assessment and prioritization workflow.

---

## 🛠️ Technology Stack

**Backend:** Python, FastAPI

**Frontend:** React

**Cryptographic Analysis:** AST, Regular Expressions, OpenSSL, PyOpenSSL

**Network Analysis:** Scapy, TLS / X.509

**Data:** PostgreSQL, JSON, CBOM

**Post-Quantum Cryptography:** ML-KEM, ML-DSA, Hybrid Cryptography

> The technology stack may evolve as the prototype is further developed.

---

## 📁 Repository Structure

- `prototype/` — Current prototype implementation
- `screenshots/` — Prototype screenshots
- `docs/` — Technical and research documentation
- `demo/` — Prototype demonstration
- `README.md` — Project overview

The repository structure will evolve as the project develops.

---

## 📸 Prototype Screenshots

Screenshots of the current ECDAT prototype will be added here.

### Dashboard

Prototype screenshot will be added here.

### Cryptographic Inventory

Prototype screenshot will be added here.

### Quantum Risk Assessment

Prototype screenshot will be added here.

### PQC Recommendation

Prototype screenshot will be added here.

### Migration Prioritization

Prototype screenshot will be added here.

---

## 🎥 Prototype Demo

A demonstration of the current ECDAT prototype will be added here.

**Demo:** Coming Soon

---

## 📚 Research & References

ECDAT is informed by research covering:

- Cryptographic inventories
- Quantum threat timelines
- Post-quantum cryptography migration
- Organizational PQC migration
- Enterprise cryptographic agility
- Cryptographic Bill of Materials (CBOM)

### Key References

1. **On Criteria and Tooling for Cryptographic Inventories** — Schmitt et al.
2. **Quantum Threat Timeline** — Mosca & Piani
3. **Migration to Post-Quantum Cryptography** — NIST
4. **Transitioning Organizations to Post-Quantum Cryptography** — Joseph et al.
5. **Enterprise-Level Cryptographic Agility (ELCA)**
6. **NIST PQC Standards — FIPS 203 / FIPS 204**
7. **Cryptographic Bill of Materials (CBOM) — CycloneDX**
8. **Cryptographic Agility & Quantum Readiness Research**

Detailed papers, standards and source links will be maintained in the project documentation.

---

## ⚠️ Current Scope & Limitations

ECDAT is currently a **proof-of-concept prototype**.

Detection coverage depends on the inputs and scanning techniques supported by the implementation. The project does not claim complete or 100% discovery of all cryptographic usage.

The broader proposed system may require additional development for capabilities such as:

- Expanded asset scanning
- Advanced binary analysis
- Hardware / HSM discovery
- Cloud environment integration
- Advanced dependency analysis
- Continuous cryptographic monitoring
- Enterprise-scale deployment
- Migration execution and orchestration

These capabilities represent potential future development rather than claims about the current prototype.

---

## 🚀 Future Scope

Future development can extend ECDAT toward:

- Broader cryptographic asset discovery
- Improved CBOM generation
- Cryptographic dependency mapping
- Enhanced quantum-risk modelling
- Expanded PQC recommendation logic
- Continuous cryptographic change detection
- Cloud and infrastructure integrations
- Enterprise deployment
- Migration planning and execution support

---

## 📄 Project Documents

### Presentation

Add the project presentation link here.

### Detailed Technical Report

Add the detailed technical report link here.

### Research References

Add the research/reference document link here.

### Prototype Demo

Add the prototype demo link here.

---

## 👥 Team

### Team Mudrita

**Project:** ECDAT

**Hackathon:** Smart India Hackathon 2026

**Problem Statement:** SIH26164

Team members and individual roles will be added here.

---

## ⭐ Project Vision

> **Know your cryptography. Understand your quantum risk. Migrate what matters first.**
