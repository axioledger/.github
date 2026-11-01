---
name: Security Issue
about: Report a security vulnerability or concern (non-critical only — for critical issues use SECURITY.md)
title: "[security] "
labels: "security"
assignees: ""
---

> ⚠️ **STOP — read this first.**
> If this is a **critical vulnerability** (exploitable, exposes user funds, private keys, or credentials), do **NOT** open a public issue.
> Follow the responsible disclosure process in [SECURITY.md](../../SECURITY.md) instead.
>
> This template is for **non-critical** security concerns: hardening, defense-in-depth, UX guardrails, and policy questions.

---

## Summary

<!-- What is the security concern? -->

## Area

- **Package / Component:** <!-- e.g. SecurityAlert, resolveTLP, NamespaceBadge, wallet auth -->
- **TLP level affected:** <!-- SAFE / CAUTION / BLOCKED / N/A -->
- **Attack surface:** <!-- UI, input validation, storage, network, cryptographic, access control -->

## Description

<!-- Explain the concern, threat model, or missing guardrail. -->

## Expected Behavior

<!-- What should the secure behavior be? -->

## Current Behavior

<!-- What is the current behavior that is concerning? -->

## Acceptance Criteria

- [ ] Threat is clearly scoped and documented
- [ ] Fix does not regress existing security behavior
- [ ] Tests cover the security-relevant paths
- [ ] Reviewed by at least one maintainer familiar with the area
- [ ] Docs updated if threat model changes

## References

<!-- CVE, security spec, audit report, or related issue -->
