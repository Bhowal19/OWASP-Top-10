# Mitigation

Mitigating cryptographic failures starts with understanding **what data actually needs protection**.

Sensitive data should be encrypted both in transit and at rest, using modern, well-vetted cryptographic standards. TLS must be enforced everywhere, not selectively.

Password handling must rely on purpose-built hashing algorithms designed for security, not speed. Encryption keys must never be stored alongside the data they protect.

Key management deserves special attention. Keys should be generated securely, stored in centralized key management systems, rotated regularly, and revoked when compromised.

Most importantly, teams must resist building their own cryptography. Custom implementations almost always introduce subtle weaknesses that attackers exploit later.

Mitigation is not about adding more encryption—it is about **applying the right cryptography in the right places**.
