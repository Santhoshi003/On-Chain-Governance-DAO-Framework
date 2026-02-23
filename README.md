# Decentralized On-Chain Governance & Voting Platform

A full-stack decentralized governance application built using **Solidity (Hardhat)** for smart contracts and **Next.js** for the frontend.

This platform enables transparent, secure, and flexible on-chain decision-making by supporting both **Standard (1 Token = 1 Vote)** and **Quadratic Voting** mechanisms.

---

## Overview

This project demonstrates the practical implementation of blockchain-based governance for DAOs and decentralized communities.

It integrates secure smart contract logic with a modern Web3-enabled frontend interface, allowing users to create proposals, delegate voting power, and participate in governance seamlessly.

---

## Project Structure

* `/contracts` – Smart contracts (`GovernanceToken.sol`, `MyGovernor.sol`)
* `/frontend` – Next.js decentralized application with Tailwind CSS
* `/scripts` – Deployment scripts
* `/test` – Unit tests for governance logic

---

## Key Features

### ERC-20 Governance Token

* Built-in vote delegation
* Snapshot-based voting for accurate vote tracking
* Secure on-chain vote management

### Dual Voting Mechanisms

* **Standard Voting:** 1 Token = 1 Vote
* **Quadratic Voting:** Voting cost follows the formula
  [
  Cost = (Number\ of\ Votes)^2
  ]

This allows more balanced and fair governance participation.

### Web3 Governance Dashboard

* Wallet connection
* Proposal creation with selectable voting model
* Real-time proposal tracking
* Secure vote casting interface

---

## Technology Stack

* Solidity
* Hardhat
* Next.js
* Tailwind CSS
* Ethers.js
* Docker
* Ethereum Local Network

---

## Setup & Execution

To run the project:

### Start the Local Blockchain

```bash
npm install
npx hardhat node
```

Deploy the smart contracts in a new terminal:

```bash
npx hardhat run scripts/deploy.js --network localhost
```

Update the deployed contract addresses in:

```
frontend/config.ts
```

Then start the frontend:

```bash
cd frontend
npm install
npm run dev
```

Access the application at:

```
http://localhost:3000
```

---

## Troubleshooting

* Ensure Node.js v18 or later is installed.
* Confirm contract addresses are correctly updated in the frontend configuration.
* Install required build tools if facing Hardhat dependency errors.

---

## Project Significance

This project highlights:

* Smart contract development expertise
* DAO governance implementation
* Web3 frontend integration
* Full-stack blockchain architecture design
