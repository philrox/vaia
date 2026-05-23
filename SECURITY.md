# Security Policy

## Supported Versions

This project is in active early development. Only the `main` branch is supported.

## Reporting a Vulnerability

**Do not open public GitHub issues for security vulnerabilities.**

Please report security issues privately by emailing:

**philipp.sparoutz@gmail.com**

Include:

- Description of the vulnerability
- Steps to reproduce
- Potential impact
- (Optional) Suggested fix

We will acknowledge receipt within 72 hours and aim to provide a fix within 7 days for critical issues.

## Scope

VAIA handles agent wallets and on-chain transaction signing. Particularly sensitive areas:

- Wallet key handling and derivation
- Polymarket V2 / Hyperliquid transaction signing
- Arc smart contract interactions
- API keys and secrets in environment configuration
- Dashboard authentication and authorization

## Disclaimer

This software is provided as-is during the hackathon period (May 2026) and is not audited. Do not use it with significant real funds without an independent security review.
