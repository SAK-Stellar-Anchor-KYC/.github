<p align="center">
  <img src="https://github.com/user-attachments/assets/969c0de8-da7b-4a13-b549-66e5cbed576f" alt="video-Ancla" />
</p>

<h2 align="center">“Security You Can Anchor To.”</h2>

---

## 📑 Table of Contents
1. Problem Statement  
2. Target Users & Needs  
3. Solution Overview  
4. Core Features  
5. MVP Architecture  
6. Success Criteria  
7. Team  

---

## 1. 🚨 Problem Statement  
### **What real-world problem are we solving?**

Stellar Anchors currently operate **manual, isolated and repetitive KYC/AML processes**.  
Every Anchor verifies users **from scratch**, even if the user has already completed KYC elsewhere.

This creates:

- ⏳ Long onboarding times  
- 💸 High operational costs  
- 📂 Duplicate document uploads  
- 🔐 Increased security exposure  
- 🚫 Poor scalability across the network  

### **Who is affected?**

- Regulated Anchors  
- Users interacting with multiple anchors  
- On/off-ramp companies  
- Platforms requiring compliance  

### **Why is this urgent now?**

The Stellar ecosystem is expanding, and recent incidents — such as the **July 2024 Fractal ID breach** — revealed a major vulnerability:

> Multiple companies store full KYC datasets → multiplied attack surface.

Since Stellar users frequently interact with several Anchors, the risk increases.

👉 A **unified, encrypted, permission-controlled KYC Vault** is needed **now**.

---

## 2. 🎯 Target Users & Needs  

### **Primary User**
**Stellar Anchors**

### **Core Needs**
- Reduce compliance workload  
- Eliminate duplicated KYC  
- Lower operational cost  
- Improve onboarding speed  
- Maintain regulatory compliance  

### **Current Workaround**
Each Anchor runs its own KYC process:

- Custom forms  
- Manual verification  
- Re-uploading documents  
- Non-reusable workflows  

---

## 3. 🧩 Solution Overview  

### **Main Idea**
**SAK provides a unified and automated KYC system with a ZK-based encrypted Vault.**  
Users complete KYC **only once**, and Anchors verify user validation through SAK.

This eliminates:

- Repeated uploads  
- Duplicate identity capture  
- Manual re-verification  
- Multiple sensitive data silos  

---

### **User Journey**
1. User completes KYC once via **SAK**  
2. SAK validates:  
   - Documents  
   - Region  
   - KYC tier (BASE / SEPA / AAA)  
3. Anchor requests access  
4. User approves  
5. Anchor activates deposits, withdrawals or RWA operations  

---

### ⭐ Why Stellar?
- Built around **SEP-12**  
- Reduces compliance workload  
- Standardizes KYC flows  
- Ideal for remittances, payments & RWA  
- **Soroban** enables permission control + auditing  

---

## 4. ⚙️ Core Features  

### **Feature 1: One-Time KYC Submission**
User completes KYC only once through SAK.  
✔️ Working if: The system stores & retrieves the KYC record.

---

### **Feature 2: Anchor KYC Lookup**
Anchors request KYC data and receive **status + verification tier**.  
✔️ Working if: Anchor sees validated user information.

---

### **Feature 3: Automatic KYC Tier Assignment**
Document type + region → BASE / SEPA / AAA.  
✔️ Working if: User receives correct tier.

---

### **Stretch Goals**
- Consent-based access panel  
- Soroban permissions contract  
- Fully encrypted ZK-based Vault  

---

## 5. 🏗️ MVP Architecture  

### **Stack**
- **Frontend:** Next.js + TailwindCSS  
- **Backend:** Node.js  
- **Smart Contracts:** Soroban (permissions + audit)  
- **Database:** PostgreSQL  
- **ZK:** Noir (Aztec)  
- **Storage:** Encrypted off-chain Vault (or simulated in demo)  

---

### **Flow Diagram**

---

## 6. 🧪 Success Criteria  

- ✔️ A user can complete KYC once via SAK  
- ✔️ An Anchor can read KYC data **without duplication**  
- ✔️ Automatic tier assignment operates correctly  
- ✔️ User can grant/revoke anchor access *(to validate with mentors)*  
- ✔️ Onboarding to a second Anchor is instant  
- ✔️ Fast onboarding flow for users  

---

### 7. 👥 Team  

## 🛠️ Tech Stack

<p align="center">
  <table>
    <tr>
      <td align="center">
        <img src="https://github.com/user-attachments/assets/4079a4f0-8ab5-43bf-8a02-267c5c471691" width="140" /><br/>
        <sub><b>Diego Raúl Barrionuevo</b></sub>
      </td>
      <td align="center">
        <img src="https://github.com/user-attachments/assets/4079a4f0-8ab5-43bf-8a02-267c5c471691" width="140" /><br/>
        <sub><b>Leandro Masotti</b></sub>
      </td>
      <td align="center">
        <img src="https://github.com/user-attachments/assets/4079a4f0-8ab5-43bf-8a02-267c5c471691" width="140" /><br/>
        <sub><b>Manuel Jimenez Garro</b></sub>
      </td>
      <td align="center">
        <img src="https://github.com/user-attachments/assets/4079a4f0-8ab5-43bf-8a02-267c5c471691" width="140" /><br/>
        <sub><b>Gonzalo Chacón</b></sub>
      </td>
      <td align="center">
        <img src="https://github.com/user-attachments/assets/4079a4f0-8ab5-43bf-8a02-267c5c471691" width="140" /><br/>
        <sub><b>Augusto F. Rios Choque</b></sub>
      </td>
    </tr>
  </table>
</p>


---

## 8. **FAQ**
### Unified KYC Infrastructure for Stellar Anchors – FAQ

In an increasingly global economy, financial institutions are more vulnerable to illicit criminal activities. Know Your Customer (KYC) standards are designed to protect financial institutions against fraud, corruption, money laundering and terrorist financing.

- ✔️ What problem does this solution address?
KYC (Know Your Customer) processes are currently broken in the Stellar ecosystem:
Anchors repeat KYC for every user.
Onboarding is slow.
Compliance costs are high.
Centralized KYC creates a huge attack surface (e.g., Fractal ID breach).
Goal: Reduce redundancy, improve security, and streamline onboarding.

- ✔️ Who is affected by the current KYC challenges?
Anchors
Users
Wallets & Apps
The entire Stellar ecosystem

- ✔️ Why do current KYC solutions fail?
Redundant KYC processes across multiple anchors.
Centralized data storage → vulnerable to breaches.
Manual verification slows operations.
No shared infrastructure for identity verification.

- ✔️ What is the proposed solution?
Users complete KYC once.
Data stored in an encrypted KYC Vault.
Anchors verify identity via SEP-12 protocol.

Zero-Knowledge proofs ensure secure verification without exposing sensitive data.
- ✔️ How does this help the ecosystem?
Eliminates repeated KYC checks.
Enables instant onboarding.
Reduces compliance costs.
Minimizes data exposure.
Improves interoperability across Stellar anchors.

- ✔️ How does the system work in practice?
Scenario 1: New User Registration
User completes KYC with an anchor (e.g., Ripio).
SAK verifies KYC via API.
User can transact (e.g., ARS → USDC).
Other anchors can retrieve verified KYC data.
Scenario 2: Returning User
User initiates a transaction with another anchor (e.g., Anclap).
System retrieves previously validated KYC via SAK API.
Transaction proceeds seamlessly without re-verification.

- ✔️ Why is this important?
Security: Encrypted, decentralized storage (IPFS + encryption).
Efficiency: One-time KYC for multiple anchors.
Flexibility: Works across wallets, apps, and anchors.
Speed: Faster onboarding and transactions.

- ✔️ What’s next on the roadmap?
Data storage: IPFS + encryption for immutable, secure blobs.
Real-world testing: Integration with Anclap (Argentina) anchor API.

---

