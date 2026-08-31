# Contributing to AXIOLEDGER ($AXQ)

Thank you for contributing to **axioledger** — the **Core Settlement / DAO** pillar of the [AXIOLEDGER](https://github.com/axioledger) ecosystem.

## Clean-Room Engineering

Absolutely no copying of copyrighted source code. All contributions must comply with the open-source license standards (MIT / Apache-2.0 for SDKs; BSL 1.1 for core contracts).

## GPG Signing (Required)

All commits and pull requests **must** be signed with a GPG key to protect the software supply chain:

```bash
git config --global commit.gpgsign true
git config --global user.signingkey YOUR_KEY_ID
```

Unsigned commits to `main`, `ledger`, or `dev` branches will be automatically rejected by branch protection rules.

## Repository & Branch Naming

All repositories follow the `axq-*` prefix convention:
- Example repos: `axq-core-contracts, axq-ans-sdk`

Branch naming:
| Prefix | Use |
|---|---|
| `feat/axq-*` | New feature |
| `fix/axq-*` | Bug fix |
| `security/axq-*` | Security patch — requires Security Auditor approval |
| `docs/axq-*` | Documentation update |

Always branch from `dev`:
```bash
git checkout dev && git pull upstream dev
git checkout -b feat/axq-your-feature
```

## Development Standards

**Rust (consensus/node components):**
```bash
cargo test --all
cargo clippy -- -D warnings
cargo fmt --check
```

**TypeScript/Node.js (`@axioledger/*` packages):**
```bash
npm test
npx eslint . --ext .ts,.tsx
npx tsc --noEmit
```

## Pull Request Process

1. All tests must pass
2. GPG signature required on all commits
3. Reference related issues
4. Minimum **2 core maintainer** approvals
5. Cryptographic / consensus changes require **Security & FIM Auditor** approval

## Security Issues

**Do NOT open public issues for security vulnerabilities.**  
Follow the [Security Policy](SECURITY.md) — use GitHub private security advisories.

---

*AXIOLEDGER — AXIOLEDGER Ecosystem · Genesis v0.0.0*
