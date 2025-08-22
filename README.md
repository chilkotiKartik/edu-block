# 🧩 Eduverse – Blockchain Subsystem

This repository contains the **blockchain-powered subsystem** for Eduverse.
It leverages **Ethereum Smart Contracts**, **IPFS (InterPlanetary File System)**, and **Metamask** to securely handle academic data such as **appointments, PDF storage, and records management**.

Unlike the original project (EHR 2.0), this version is **stripped down** to include only the **decentralized backend** — no Firebase or external live hosting.

---

## ✨ Features

* 📄 **Smart Contracts** for secure record handling
* 🌐 **IPFS integration** for decentralized file storage (e.g., PDFs, certificates)
* 🔒 **Blockchain-based authentication** via Metamask
* ⚡ Local Ethereum blockchain simulation with **Ganache**

---

## 🛠️ Prerequisites

Make sure you have the following installed:

1. **Node.js** → [Download](https://nodejs.org/en/download/)
2. **Ganache** (Local Ethereum blockchain) → [Download](https://trufflesuite.com/ganache/)
3. **Truffle** (Ethereum development framework):

   ```sh
   npm install -g truffle
   ```
4. **IPFS (Kubo)** → [Download](https://dist.ipfs.tech/#go-ipfs)

   * Setup guide: [IPFS Config](https://github.com/shamil-t/ehr-blockchain/issues/15#issuecomment-1333342345)
5. **Metamask Browser Extension** → [Install](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn?hl=en)

---

## ⚙️ Setup Guide

1. **Clone Repository**

   ```sh
   git clone https://github.com/shamil-t/ehr-blockchain
   cd ehr-blockchain
   ```

2. **Install Dependencies**

   ```sh
   npm install --force
   ```

3. **Start Ganache**

   * Create a **New Workspace**
   * Add Project → Select `truffle-config.js` inside repo
   * Save Workspace

4. **Compile & Deploy Contracts**

   ```sh
   truffle migrate
   ```

5. **Connect Metamask**

   * Open Metamask → Add Network manually
   * Network Name: `Ganache Local`
   * RPC URL: `http://127.0.0.1:7545`
   * Chain ID: `1337` (or as shown in Ganache)
   * Import one of the private keys from Ganache

6. **Run the Application**

   ```sh
   npm start
   ```

   App will be available on: **[http://localhost:3000](http://localhost:3000)**

---

## 🚨 Troubleshooting

* **WSL Issues (Windows users):** Update WSL with:

  ```sh
  wsl --update
  ```
* **IPFS errors?** → Check [this fix](https://github.com/shamil-t/ehr-blockchain/issues/15)

---

## 📬 Contact

For queries & collaborations:
📧 `eduverse-support@example.com`

---

✅ With this setup, you’ll have a **fully functional blockchain subsystem** running locally, ready to be extended for Eduverse features like **certificates, academic records, and decentralized student services**.
