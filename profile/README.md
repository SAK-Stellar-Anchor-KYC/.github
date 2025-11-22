<p align="center">
  <img src="https://github.com/user-attachments/assets/969c0de8-da7b-4a13-b549-66e5cbed576f" alt="video-Ancla" />
</p>

<h2 align="center">Security You Can Anchor To.</h2>

## Table of Contents
1. SAK
2. Target Users & Needs  
3. Solution Overview  
4. Core Features  
5. MVP Architecture  
6. TEAM  
7. FAQ  

---

## 1. Stellar Anchor KyC  
### **What IS SAC?**

SAK is a unified KYC infrastructure for Stellar anchors, designed to correct defective identity verification processes in the ecosystem. Currently, anchors verify users from scratch in a redundant manner, leading to slow onboarding, high costs, duplicate document uploads, and security risks from centralized data storage, such as the 2024 Fractal ID breach. <br><br>
The solution allows users to complete KYC only once in an encrypted and decentralized vault that uses IPFS for immutable blobs and zero-knowledge proofs for privacy, enabling anchors to query verified data via SEP-12 without exposing sensitive information.<br><br>
This improves efficiency with instant onboarding, reduces compliance expenses, minimizes data exposure, and enhances interoperability between anchors and apps.
In practice, a new user verifies with an anchor and can transact immediately, while returning users seamlessly switch to others without re-verification.

This creates:

-  Long onboarding times  
-  High operational costs  
-  Duplicate document uploads  
-  Increased security exposure  
-  Poor scalability across the network  

### **Who is affected?**

- Regulated Anchors  
- Users interacting with multiple anchors  
- On/off-ramp companies  
- Platforms requiring compliance  

## 2. Target Users & Needs  

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

## 3. Solution Overview  

**Our infra delivers a unified KYC proxy aligned with (SEPs 10/12/24), enabling one-time user verification and permissioned KYC access that any anchor can reuse..**  

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

### Why Stellar?
- Built around **SEP-12**  
- Reduces compliance workload  
- Standardizes KYC flows  
- Ideal for remittances, payments & RWA  
- **Soroban** enables permission control + auditing  

---

## 4. Core Features  

### **Feature 1: One-Time KYC Submission**
User completes KYC only once through SAK.  
- Working if: The system stores & retrieves the KYC record.

---

### **Feature 2: Anchor KYC Lookup**
Anchors request KYC data and receive **status + verification tier**.  
- Working if: Anchor sees validated user information.

---

### **Feature 3: Automatic KYC Tier Assignment**
Document type + region → BASE / SEPA / AAA.  
- Working if: User receives correct tier.

---

### **Stretch Goals**
- Consent-based access panel  
- Soroban permissions contract  
- Fully encrypted ZK-based Vault  

---

### **Flow Diagram**

<img width="1099" height="626" alt="image" src="https://github.com/user-attachments/assets/9e5841e3-0349-46b8-a915-25a120901594" />


---

## 6. Success Criteria  

- A user can complete KYC once via SAK  
- An Anchor can read KYC data **without duplication**  
- Automatic tier assignment operates correctly  
- User can grant/revoke anchor access *(to validate with mentors)*  
- Onboarding to a second Anchor is instant  
- Fast onboarding flow for users  

---

### 7. Team  

<div align="center">

<table>
  <tr>
    <!-- Diego -->
    <td align="center">
      <a href="https://github.com/Kalchaqui">
        <img src="https://github.com/user-attachments/assets/4079a4f0-8ab5-43bf-8a02-267c5c471691" width="120" alt="Diego Raúl Barrionuevo"><br>
        Diego Raúl Barrionuevo
      </a>
    </td>
    <!-- Leandro -->
    <td align="center">
      <a href="https://github.com/leandromasotti">
        <img src="https://github.com/user-attachments/assets/426f321b-130d-41ea-a254-994859d655f2" width="120" alt="Leandro Masotti"><br>
        Leandro Masotti
      </a>
    </td>
    <!-- Manuel -->
    <td align="center">
      <a href="https://github.com/ManuelJG1999">
        <img src="https://github.com/user-attachments/assets/3d535208-1054-4c5e-8253-3740d12e78f0" width="120" alt="Manuel Jiménez Garro"><br>
        Manuel Jiménez Garro
      </a>
    </td>
    <!-- Gonzalo -->
    <td align="center">
      <a href="https://github.com/gchacon011">
        <img src="https://github.com/user-attachments/assets/5b8e9ee6-d6c8-45dc-8b18-9511fa09fd06" width="120" alt="Gonzalo Chacón"><br>
        Gonzalo Chacón
      </a>
    </td>
    <!-- Augusto -->
    <td align="center">
      <a href="https://github.com/SphinxBSD">
        <img src="https://github.com/user-attachments/assets/941dc8ad-ba99-4b8e-bfd8-33f2eb2ebd1b" width="120" alt="Augusto F. Rios Choque"><br>
        Augusto F. Rios Choque
      </a>
    </td>
  </tr>
</table>

</div>


---

## 8. **FAQ**
### Unified KYC Infrastructure for Stellar Anchors – FAQ

KYC in Stellar is broken: Anchors repeat verifications, causing slow onboarding, high costs, and security risks from centralized data (e.g., Fractal ID breach). Goal: Reduce redundancy, enhance security, and speed up processes.
- Who is affected?
Anchors, users, wallets/apps, and the entire Stellar ecosystem.
- Why do current solutions fail?
Redundant processes across anchors, vulnerable centralized storage, manual verifications, and no shared identity infrastructure.
- What is the proposed solution?
Users do KYC once, stored in an encrypted Vault. Anchors verify via SEP-12 using zero-knowledge proofs for secure, data-minimizing checks.
- How does it benefit the ecosystem?
Eliminates repeats, enables instant onboarding, cuts costs, reduces data exposure, and boosts interoperability.
- How does it work?
New User: Completes KYC with one anchor (e.g., Ripio); SAK verifies/stores; instant transactions; others access verified data.
Returning User: Switches anchors (e.g., Anclap); retrieves prior KYC via API; seamless without re-verification.

- Why is this important?
Offers encrypted decentralized storage (IPFS), one-time KYC efficiency, flexibility across tools, and faster operations.





---

