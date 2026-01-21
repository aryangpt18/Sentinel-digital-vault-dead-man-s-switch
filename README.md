# 🛡️ Legacy 404: AI-Powered Decentralized Dead Man's Switch

> **"Your digital legacy, secured by code and organized by AI."**

![Project Status](https://img.shields.io/badge/Status-Prototype-green)
![Tech Stack](https://img.shields.io/badge/Stack-Streamlit%20|%20Web3%20|%20Gemini%20AI-blue)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

## 📖 Overview
**Legacy 404** is a decentralized "Dead Man's Switch" designed to solve the problem of **Digital Inheritance**. 

Billions of dollars in crypto and digital assets are lost every year because owners pass away without sharing their private keys. Existing solutions rely on centralized trust (lawyers/banks) or are too rigid (instant transfer). 

**Legacy 404** combines **Blockchain Security** with **AI Intelligence** to ensure your assets are transferred to your chosen beneficiary *only* when you are truly gone, while protecting you against accidents or comas while you are alive.

---

## 🚀 Key Features

### 1. 💓 The Heartbeat Protocol
The system requires the owner to "Check-In" at regular intervals (e.g., every 30 days). This resets the **Smart Contract** timer. As long as the heart beats, the assets remain locked in the vault.

### 2. 🛡️ The Grace Period (Fail-Safe)
If a check-in is missed, the assets are **NOT** transferred immediately. 
- A **Grace Period** (e.g., 48 hours) triggers.
- Multi-channel notifications (Email/SMS) are sent to the owner.
- If the owner is alive (e.g., just forgot), they can **CANCEL** the transfer with one click.

### 3. 🚑 Guardian & Emergency Access
Solved the "Waiting Game" problem. If the owner passes away, the beneficiary can request **Emergency Access**.
- This triggers an immediate alert to the owner.
- If the owner does not veto/block the request within a set time (e.g., 24 hours), access is granted.
- **Guardian Feature:** If the owner is in a coma, the beneficiary can *extend* the timer to keep assets safe without stealing them.

### 4. 🤖 AI Executor (Powered by Gemini)
Raw data left behind is often messy ("My password is my dog's name + 123").
- We use **Google Gemini 1.5 Pro** to process the decrypted data.
- It turns unstructured notes into a **Professional Digital Will** (JSON format), organizing credentials, financial data, and personal messages instantly.

---

## 🛠️ Architecture & Tech Stack

The system follows a **Zero-Knowledge** architecture.

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Frontend** | **Streamlit (Python)** | The user interface for check-ins and vault management. |
| **Logic Layer** | **Python / Web3.py** | Handles the timer logic, role management, and state checks. |
| **Smart Contract** | **Solidity (Ethereum)** | *[Simulation Mode]* Manages the immutable rules of transfer. |
| **Storage** | **IPFS** | *[Concept]* Stores the encrypted data payload (passwords/files). |
| **Intelligence** | **Google Gemini API** | Cleans and structures the legacy data after decryption. |

### Security Flow
1. **Encryption:** User inputs are encrypted Client-Side using the Beneficiary's Public Key.
2. **Storage:** Encrypted payload is pinned to IPFS.
3. **Trigger:** Smart Contract releases the IPFS Hash (CID) only upon protocol expiration.
4. **Decryption:** Beneficiary uses their Private Key to unlock the data.

---

## ⚙️ Installation & Setup

Follow these steps to run the prototype locally:

**1. Clone the Repository**
```bash
git clone [https://github.com/YOUR_USERNAME/Legacy-404.git](https://github.com/YOUR_USERNAME/Legacy-404.git)
cd Legacy-404
