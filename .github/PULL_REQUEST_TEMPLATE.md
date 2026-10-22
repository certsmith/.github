## Description

Please provide a concise description of the changes introduced in this pull request and the rationale behind them.

Fixes #(issue)

---

## Type of Change

Please mark the options that apply:

- [ ] `fix`: Bug fix (non-breaking change which fixes an issue)
- [ ] `feat`: New feature (non-breaking change which adds functionality)
- [ ] `perf`: Performance improvement
- [ ] `refactor`: Code refactoring without behavioral alterations
- [ ] `docs`: Documentation updates or additions
- [ ] `chore`: Maintenance, dependency updates, or pipeline improvements
- [ ] `security`: Cryptographic hardening or security advisory remediation

---

## Validation and Testing

Please verify the validation steps completed:

- [ ] Multi-stage Docker build passes cleanly (`docker build -t certsmith:test .`)
- [ ] End-to-end ACME issuance test passes (`./tools/test-issuance.sh .env`)
- [ ] Trust Portal static export completes without errors (`pnpm build` in `web/`)
- [ ] TypeScript typecheck passes (`pnpm typecheck` in `web/`)
- [ ] Code formatting conforms to project standards (`pnpm format` in `web/`)
- [ ] No private keys, certificates, or unencrypted secrets are committed in this branch

---

## Cryptographic and Security Impact

Does this PR introduce changes to:
- Key ceremony scripts or default curve/key parameters? [Yes / No]
- Nginx TLS termination or cipher suites? [Yes / No]
- step-ca configuration generation or filesystem permissions? [Yes / No]

If Yes, please explain the security review conducted:

---

## Checklist

- [ ] My code follows the code style and conventions of this repository.
- [ ] I have updated the documentation accordingly.
- [ ] I have read and agree to the [Contributing Guidelines](CONTRIBUTING.md) and [Code of Conduct](CODE_OF_CONDUCT.md).
