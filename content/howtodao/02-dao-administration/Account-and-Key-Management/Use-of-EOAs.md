---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Use of EOAs, Multisigs, and Smart Contract Wallets'
weight: 33_000
---

Effective account and key management is crucial for DAO security and governance. This section explores the three main types of wallets used in DAOs:  

- **Externally Owned Accounts (EOAs)** – Simple wallets controlled by a private key.  
- **Multisig Wallets** – Require multiple approvals for transactions.  
- **Smart Contract Wallets** – Programmable wallets with advanced security features.  

Each wallet type has distinct trade-offs in security, decentralization, and usability.  

---

## **Externally Owned Accounts (EOAs)**  

An EOA is a standard wallet controlled by a single private key, typically managed through wallets like MetaMask, Ledger, or Trezor.  

### **Advantages**  
- **Simplicity** – Easy to set up and use.  
- **Low Gas Costs** – No additional contract interactions.  
- **Full Control** – Only the keyholder can sign transactions.  

### **Challenges**  
- **Single Point of Failure** – If the private key is lost or compromised, access is permanently lost.  
- **No Built-in Recovery** – Unlike smart contract wallets, EOAs lack account recovery options.  
- **Risk of Centralization** – In a DAO setting, a single EOA controlling key functions undermines decentralization.  

### **DAO Use Cases**  
- Suitable for individual contributors receiving payments.  
- Used for low-privilege DAO roles where decentralization isn’t a concern.  

---

## **Multisig Wallets**  

A multisignature (multisig) wallet requires multiple signers to approve transactions. Popular multisig solutions include Gnosis Safe and TotalSig.  

### **How Multisigs Work**  
- Require M out of N signatures (e.g., 3 out of 5 signers).  
- Transactions are only executed if the required threshold is met.  

### **Advantages**  
- **Enhanced Security** – Prevents a single compromised key from executing transactions.  
- **Shared Control** – Ensures decisions involve multiple trusted parties.  
- **Built-in Governance** – Aligns with decentralized decision-making.  

### **Challenges**  
- **Slower Execution** – Transactions need multiple approvals, which can delay operations.  
- **Coordination Complexity** – Requires ongoing signer participation.  
- **Vulnerability to Collusion** – If a majority of signers collude, they can bypass security measures.  

### **DAO Use Cases**  
- Commonly used for treasury management.  
- Helps governance committees control high-privilege administrative actions.  
- Used for grant funding to ensure fair distribution.  

---

## **Smart Contract Wallets**  

A smart contract wallet is a programmable account that can enforce security rules. Examples include Safe Modules, Argent, and Kernel Smart Wallets.  

### **Features of Smart Contract Wallets**  
- **Customizable Permissions** – Define who can execute certain actions.  
- **Account Recovery Mechanisms** – Enable social recovery or multi-key setups.  
- **Gas Abstraction** – Some wallets allow fee payment in tokens instead of ETH.  

### **Advantages**  
- **Advanced Security** – Can include time locks, withdrawal limits, or multisig-like logic.  
- **Programmability** – Custom governance logic can be implemented.  
- **User-Friendly Recovery** – Reduces risks of permanent loss due to private key mismanagement.  

### **Challenges**  
- **Higher Gas Costs** – Smart contract execution requires more gas than EOAs.  
- **Complexity** – Requires proper configuration and security audits.  
- **Upgradeability Risks** – Poorly designed upgrades can introduce vulnerabilities.  

### **DAO Use Cases**  
- Ideal for governance-controlled contracts (e.g., automated treasury disbursement).  
- Used for DAO-based identity and access control.  
- Facilitates progressive decentralization by transitioning from a multisig to smart contract governance.  

---

## **Comparison: EOAs vs. Multisigs vs. Smart Contract Wallets**  

| **Feature**            | **EOA**  | **Multisig Wallet** | **Smart Contract Wallet** |
|-------------------|------|----------------|----------------------|
| **Security** | Low | High | Very High |
| **Decentralization** | None | Moderate | High |
| **Ease of Use** | High | Moderate | Lower |
| **Gas Costs** | Low | Moderate | High |
| **Customizability** | None | Low | High |
| **Best For** | Individuals | Treasury, Admin Control | Automated Governance |

DAOs should choose the right wallet type based on their governance needs, balancing security, decentralization, and usability.  

