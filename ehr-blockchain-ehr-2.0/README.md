⚡ Eduverse – Blockchain Subsystem Setup (Based on EHR 2.0)

This subsystem manages appointments, PDF uploads, and record storage on blockchain + IPFS.
No Firebase/Live links — only decentralized backend.

🔧 Requirements

Install Node.js
👉 Download Node.js

Install Ganache (Local Ethereum Blockchain)
👉 Ganache

Install Truffle (Smart Contract Framework)
Open PowerShell/Terminal as Admin:

npm install -g truffle


Install IPFS (Kubo)
👉 IPFS Kubo Download

Configure IPFS (guide: here
)

Install Metamask Extension
👉 Metamask Chrome

Create/import wallet.

Connect to Ganache local blockchain (use RPC URL: http://127.0.0.1:7545).

⚙️ Setup Steps

Clone the repo into Eduverse:

git clone https://github.com/shamil-t/ehr-blockchain
cd ehr-blockchain


Install dependencies:

npm install --force


Open Ganache → Create a new workspace

Add Project → select truffle-config.js from repo.

Save Workspace.

Compile & migrate contracts:

truffle migrate


Start the blockchain server (local dApp):

npm start

🚨 Known Issues

Check this thread if IPFS doesn’t work properly:
👉 Issue #15