# Security Policy

## Supported Versions

Security updates and critical vulnerability fixes are applied to the active branch and releases according to the following schedule:

| Version | Supported | Maintenance Tier |
| :--- | :--- | :--- |
| `main` (Latest) | Yes | Active Security Fixes & Feature Development |
| `< 1.0.0` | Limited | Critical Security Patches Only |

---

## Reporting a Vulnerability

The Certsmith team takes the security of our cryptographic infrastructure and appliances seriously. If you identify a potential security vulnerability in any Certsmith repository, please disclose it responsibly.

### How to Report

1. **GitHub Private Vulnerability Reporting (Preferred)**:
   - Go to the repository where the vulnerability exists (e.g., [certsmith/certsmith](https://github.com/certsmith/certsmith)).
   - Navigate to the **Security** tab.
   - Click **Report a vulnerability** to initiate an encrypted, private disclosure advisory.

2. **Direct Security Contact**:
   - If GitHub Private Vulnerability Reporting is unavailable, send an encrypted email to:
     `certsmith@dyzulk.com`

### Information to Include

Please provide as much relevant technical detail as possible:
- Type of vulnerability (e.g., private key leakage, privilege escalation, ACME authentication bypass, denial of service).
- Step-by-step reproduction instructions or proof-of-concept scripts.
- Affected issuing tier (CR1-CR3, CE1-CE3), appliance component (Nginx, step-ca), or Trust Portal route.
- Assessment of potential impact and severity.

### Response Timeline and Commitments

- **Initial Acknowledgment**: Within 48 hours of receipt.
- **Triage and Impact Assessment**: Within 5 business days.
- **Resolution and Patch Release**: Timeframes vary based on severity, targeting 14 business days for critical vulnerabilities.
- **Coordinated Disclosure**: We request that you avoid public disclosure until an official fix has been published.
