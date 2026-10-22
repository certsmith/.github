# Certsmith Support

Welcome to the Certsmith support directory. This document outlines available resources, self-service diagnostics, and communication channels for receiving assistance.

---

## 1. Documentation and Guides

Before opening a support request or issue, please review our comprehensive guides:

- **Root CA Trust Store Installation**:
  - Detailed cross-platform installation steps for Linux, macOS, Windows, Android, iOS, Docker, Java, and Node.js are available on the Trust Portal web frontend (`/guides/root-ca`).
- **ACME Client Configuration**:
  - Copy-paste configuration recipes for Certbot, Lego, Caddy, Traefik, and acme.sh (`/guides/acme-clients`).
- **Cryptographic Specifications**:
  - Review the architecture matrix in the [certsmith/certsmith](https://github.com/certsmith/certsmith) repository README.

---

## 2. Community Q&A and Discussions

For setup questions, homelab architecture advice, and general troubleshooting:

- **GitHub Discussions**:
  Visit [Certsmith Discussions](https://github.com/orgs/certsmith/discussions) to ask questions or share implementation configurations.

---

## 3. Reporting Defects and Vulnerabilities

- **Software Defects and Bugs**:
  If you have encountered a bug or reproducible malfunction, submit a report using the [Bug Report Form](https://github.com/certsmith/certsmith/issues/new?template=01_bug_report.yml).
- **Security Vulnerabilities**:
  For private disclosures concerning cryptographic flaws or credentials, please follow our [Security Policy](SECURITY.md). Never submit vulnerability reports through public channels.

---

## 4. Operational Self-Diagnostics

When troubleshooting an appliance deployment, verify system health using standard diagnostics:

```bash
# Check container logs
docker logs certsmith

# Query health endpoints
curl -fsS http://localhost/health
curl -fsS http://localhost/healthz

# Run automated issuance validation
./tools/test-issuance.sh .env
```
