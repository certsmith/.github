# Contributing to Certsmith

Thank you for your interest in contributing to Certsmith. We welcome contributions to improve our private CA appliance, offline forge tools, and Trust Portal documentation.

---

## Code of Conduct

All contributors and maintainers are expected to adhere to the [Code of Conduct](CODE_OF_CONDUCT.md). Please read it before participating in our discussions, issues, or pull requests.

---

## Development Workflow

### 1. Issue First Policy

For substantial architectural modifications, new cryptographic curves, or feature proposals, please open an issue using the appropriate template or start an RFC discussion before writing code.

### 2. Branching Strategy

- Develop all changes in focused feature or bugfix branches derived from `main`.
- Branch naming convention:
  - `feat/<short-description>`: New features or capabilities.
  - `fix/<short-description>`: Defect repairs.
  - `docs/<short-description>`: Documentation improvements.
  - `chore/<short-description>`: Tooling, dependency, or CI/CD updates.

### 3. Commit Message Standards

Certsmith strictly adheres to the Conventional Commits specification:

```
<type>(<optional scope>): <description>

[optional body]

[optional footer(s)]
```

Common types:
- `feat`: A new feature or cryptographic tier capability.
- `fix`: A bug fix.
- `docs`: Documentation changes only.
- `refactor`: Code change that neither fixes a bug nor adds a feature.
- `perf`: Code change that improves performance.
- `test`: Adding missing tests or correcting existing tests.
- `chore`: Changes to build process, dependency bumps, or auxiliary tools.

Examples:
- `feat(pki): introduce support for custom validity extensions in CE2 tier`
- `fix(nginx): correct upstream timeout during ACME challenge evaluation`
- `docs(guides): add Caddy v2 reverse proxy trust store instructions`

---

## Local Verification Requirements

Before opening a pull request, ensure all relevant verification checks pass:

### Appliance & Core Tooling
- Verify the multi-stage Docker build succeeds cleanly:
  ```bash
  docker build -t certsmith:test .
  ```
- Run the issuance test harness against a test `.env`:
  ```bash
  ./tools/test-issuance.sh .env
  ```

### Trust Portal Frontend (`web/`)
- Run typecheck and static bundle compilation:
  ```bash
  pnpm --prefix web typecheck
  pnpm --prefix web build
  ```
- Run code formatting via Prettier:
  ```bash
  pnpm --prefix web format
  ```

---

## Submitting Pull Requests

1. Push your branch to your fork or branch on GitHub.
2. Open a Pull Request targeting the `main` branch.
3. Complete the pull request checklist in full.
4. Address review feedback promptly. All PRs require review approval and clean CI validation before merging.
