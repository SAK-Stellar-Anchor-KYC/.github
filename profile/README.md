# SAK: Unified KYC Infrastructure for Stellar

**SAK** is a unified KYC infrastructure for the Stellar ecosystem. It introduces a shared, encrypted identity layer that allows users to complete KYC once, while enabling anchors to securely verify identities via SEP-12 without handling sensitive raw data.

---

## Vision & Mission

**Vision:** To establish a secure, reusable identity verification layer for Stellar that eliminates redundancy and strengthens data protection.

**Mission:** To provide anchors with a streamlined, privacy-preserving KYC system where users verify once and transact everywhere.

---

## The Challenge vs. The Solution

| Current Landscape | SAK Solution |
| :--- | :--- |
| **Redundancy** | Users complete KYC **only once**; reusable across all anchors. |
| **High Friction** | **Instant onboarding** for returning users; no repeated document uploads. |
| **Security Risks** | **Data minimization**: Anchors verify status/tier without storing raw documents. |
| **High Costs** | Reduced operational overhead through a **shared infrastructure**. |

---

## Core Features

- **One-Time Submission:** Centralized KYC record storage and retrieval.
- **Anchor KYC Lookup:** Anchors request and receive **Status + Verification Tier** (BASE / SEPA / AAA) securely via SEP-12.
- **Automatic Tiering:** Intelligent assignment of compliance tiers based on document type and region.
- **SEP Compatibility:** Native support for SEPs 10, 12, and 24 to ensure full ecosystem interoperability.

---

## How It Works

SAK functions as a secure proxy between users and anchors.

1.  **User** uploads data once via SAK Web.
2.  **SAK** validates and encrypts the identity data.
3.  **Anchor** requests verification via API (SEP-12).
4.  **SAK** returns the validity status and tier via ZK Proofs, protecting user privacy.

<div align="center">
  <img width="800" alt="SAK Flow Diagram" src="https://github.com/user-attachments/assets/9e5841e3-0349-46b8-a915-25a120901594" />
</div>

---

## Team

<div align="center">

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/Kalchaqui">
        <img src="https://github.com/user-attachments/assets/4079a4f0-8ab5-43bf-8a02-267c5c471691" width="80" alt="Diego"><br>
        <b>Diego Raúl Barrionuevo</b>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/leandromasotti">
        <img src="https://github.com/user-attachments/assets/426f321b-130d-41ea-a254-994859d655f2" width="80" alt="Leandro"><br>
        <b>Leandro Masotti</b>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/ManuelJG1999">
        <img src="https://github.com/user-attachments/assets/3d535208-1054-4c5e-8253-3740d12e78f0" width="80" alt="Manuel"><br>
        <b>Manuel Jiménez Garro</b>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/gchacon011">
        <img src="https://github.com/user-attachments/assets/5b8e9ee6-d6c8-45dc-8b18-9511fa09fd06" width="80" alt="Gonzalo"><br>
        <b>Gonzalo Chacón</b>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/SphinxBSD">
        <img src="https://github.com/user-attachments/assets/941dc8ad-ba99-4b8e-bfd8-33f2eb2ebd1b" width="80" alt="Augusto"><br>
        <b>Augusto F. Rios</b>
      </a>
    </td>
  </tr>
</table>

</div>

---

## Roadmap

We are continuously working to improve SAK and expand its capabilities within the Stellar ecosystem. Our future plans include:

- **Encrypted Data Storage (IPFS):** Implement immutable, encrypted identity blobs using IPFS as the decentralized storage layer.
- **Real-World Pilot (Anclap – Argentina):** Begin integration testing with Anclap to validate SAK’s workflow, anchor requests, and KYC interoperability in a production-like environment.
- **ZK Passport Integration:** Add zero-knowledge proof–based identity verification, enabling users to confirm their identity without exposing personal documents.

---

<div align="center">
  
Project created for the **Casa Stellar Argentina Hackathon, 2025**.
  
</div>
