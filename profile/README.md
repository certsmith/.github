# Certsmith Organization

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=22&duration=3000&pause=1000&color=2563EB&center=true&vCenter=true&width=650&lines=High-Assurance+Private+PKI+Appliance;6-Tier+ACME+v2+Automated+Issuance;Offline+Root+Authority+%26+Air-Gapped+Trust;Enterprise+Security+Infrastructure" alt="Certsmith Mission" />
</p>

<p align="center">
  <a href="https://github.com/certsmith/certsmith/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge" alt="License: MIT" />
  </a>
  <img src="https://img.shields.io/badge/pki-6--Tier_Hierarchy-0EA5E9.svg?style=for-the-badge" alt="6-Tier Hierarchy" />
  <img src="https://img.shields.io/badge/protocol-ACME_v2_(RFC_8555)-4F46E5.svg?style=for-the-badge" alt="ACME v2" />
  <img src="https://img.shields.io/badge/appliance-Docker_All--in--One-2496ED.svg?style=for-the-badge&logo=docker&logoColor=white" alt="Docker Appliance" />
  <img src="https://img.shields.io/badge/proxy-Nginx_TLS_Dual_Stack-009639.svg?style=for-the-badge&logo=nginx&logoColor=white" alt="Nginx" />
</p>

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=docker,nginx,react,ts,tailwind,linux,bash" alt="Technology Stack" />
  </a>
</p>

---

## Mission and Architecture

Certsmith is an open-source security engineering project dedicated to providing turnkey, high-assurance Public Key Infrastructure (PKI) appliances for homelabs, enterprise staging environments, and hybrid cloud topologies.

The core architecture strictly isolates offline root authority from operational intermediate issuing daemons. Six distinct issuing authorities serve both RSA and Elliptic Curve cryptographic profiles with automated certificate management via ACME v2 (RFC 8555):

- **CR1 (RSA 4096-bit)**: Maximum security and long-term validity for root-level anchors and core infrastructure.
- **CR2 (RSA 3072-bit)**: Enterprise standard for production services and general application workloads.
- **CR3 (RSA 2048-bit)**: High-throughput compatibility tier for legacy environments and edge devices.
- **CE1 (ECDSA P-384)**: High-assurance elliptic curve tier matching strict compliance requirements.
- **CE2 (ECDSA P-256)**: Modern, lightweight cloud-native default for containers and microservices.
- **CE3 (ECDSA P-521)**: Ultra-grade asymmetric elliptic curve tier for quantum-resistant transitional research.

---

## Primary Repositories

| Repository | Purpose | Visibility | Stack |
| :--- | :--- | :--- | :--- |
| [certsmith/certsmith](https://github.com/certsmith/certsmith) | All-in-one private CA appliance, offline forge tools, and React Router Trust Portal | Public | Docker, step-ca, Nginx, React Router 8 |
| [certsmith/.github](https://github.com/certsmith/.github) | Organization-wide community health files, issue forms, and governance policies | Public | GitHub Workflows, Issue Forms, Markdown |

---

## Community and Governance

We enforce standardized engineering guidelines across all projects under the Certsmith organization:

- [Security Policy](https://github.com/certsmith/.github/blob/main/SECURITY.md): Vulnerability reporting procedures and response commitments.
- [Contributing Guidelines](https://github.com/certsmith/.github/blob/main/CONTRIBUTING.md): Branching model, semantic commit conventions, and code standards.
- [Code of Conduct](https://github.com/certsmith/.github/blob/main/CODE_OF_CONDUCT.md): Contributor Covenant v2.1.
- [Support Center](https://github.com/certsmith/.github/blob/main/SUPPORT.md): Official support channels, FAQ, and technical discussions.
