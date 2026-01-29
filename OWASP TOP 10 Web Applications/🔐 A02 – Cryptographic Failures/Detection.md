# Detection

Cryptographic failures are often difficult to detect through surface-level testing because applications may appear to function correctly.

Detection usually begins with **design and architecture review**. Security reviewers examine where sensitive data exists, how it flows through the system, and whether it is protected at every stage.

During penetration testing, indicators include:
- Sensitive data visible in responses
- Credentials stored or transmitted in plaintext
- Missing HTTPS enforcement
- Predictable or reusable tokens

Source code reviews frequently uncover cryptographic misuse, such as deprecated algorithms, static keys, or custom encryption logic.

Operational signals also matter. If a breach results in immediate exposure of readable sensitive data, it is often an indicator that cryptographic protections were missing or ineffective.

Unlike injection flaws, cryptographic failures are rarely obvious—but their impact is usually catastrophic.
