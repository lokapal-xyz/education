---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Interacting with Non-DAO Smart Contracts'
weight: 105_000
---

DAOs do not operate in isolation—they often need to interact with external smart contracts such as DeFi protocols, NFT marketplaces, cross-chain bridges, and other dApps. These interactions can introduce new opportunities as well as security risks, making it essential for DAOs to manage them effectively.  

---

## **Why External Smart Contract Interactions Matter**  

DAOs engage with external contracts for various reasons, including:  
- **Liquidity management** – Providing or borrowing assets from DeFi platforms like Aave or Compound.  
- **Asset diversification** – Acquiring and managing NFTs or yield-bearing tokens.  
- **Protocol governance** – Voting in other DAOs or delegating governance rights.  
- **Cross-chain interactions** – Bridging assets between different blockchains.  
- **Service integrations** – Using oracle networks like Chainlink or automation tools like Gelato.  

---

## **Security Risks of External Smart Contract Interactions**  

While interacting with external contracts can be beneficial, it also introduces security concerns, including:  

### **Smart Contract Exploits**  
- If an external contract has a vulnerability, the DAO’s funds could be at risk.  
- Example: In the Curve Finance exploit (2023), vulnerabilities in a third-party contract led to significant losses.  

### **Governance Attacks**  
- DAOs relying on other protocols might be impacted by governance attacks on those protocols.  
- Example: A DAO staking in a governance token-based protocol could be affected by a flash loan attack, where an attacker manipulates voting outcomes.  

### **Dependency Risks**  
- External contract upgrades or governance changes can affect DAOs that rely on them.  
- Example: A governance change in Aave or Uniswap could impact a DAO’s liquidity strategies if those changes are not properly accounted for.  

### **Permission Management Issues**  
- Poorly designed access control can lead to unauthorized interactions, where an external contract might override DAO rules.  
- Example: If a DAO’s treasury interacts with an upgradable proxy contract, a malicious upgrade could drain funds.  

---

## **Best Practices for Secure DAO Interactions with External Contracts**  

To mitigate these risks, DAOs should adopt best practices when engaging with external smart contracts:  

### **Conduct Smart Contract Audits**  
- Before integrating with an external contract, verify that it has been properly audited.  
- Use audit reports to assess security posture.  

### **Implement Risk Management Strategies**  
- Use allow-lists to restrict interactions to trusted contracts.  
- Establish risk parameters (e.g., limit exposure to a percentage of the treasury).  
- Consider insurance protocols (e.g., Nexus Mutual or Risk Harbor) to mitigate losses.  

### **Monitor External Interactions**  
- Track transactions between the DAO and external protocols.  
- Set up alerting systems for suspicious activity.  
- Use on-chain analytics tools to monitor dependencies.  

### **Implement Time-Locks and Multi-Sig Approvals**  
- Require time delays before executing transactions involving large asset transfers.  
- Utilize multisig governance to require multiple approvals before interacting with external contracts.  

---

## **Designing DAO Frameworks for External Contract Interactions**  

DAOs can design governance frameworks to handle external interactions securely:  

### **DAO-Controlled Smart Contract Modules**  
- Instead of directly managing assets in external contracts, DAOs can use intermediate smart contracts to enforce additional security checks.  
- Example: A treasury management contract can limit the amount of funds exposed to an external protocol at any given time.  

### **Governance Approval for External Interactions**  
- Require governance votes for high-risk interactions (e.g., staking DAO funds in external protocols).  
- Automate risk assessment reports before proposal execution.  

### **Cross-DAO Coordination**  
- If a DAO is heavily dependent on another protocol, it should establish direct governance participation in that protocol’s decision-making.  
- Example: A lending protocol DAO may actively participate in Aave governance to influence policies that affect its own operations.  

