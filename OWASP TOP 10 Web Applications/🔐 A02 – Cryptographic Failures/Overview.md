# A02 – Cryptographic Failures

Cryptographic Failures occur when an application **fails to correctly protect sensitive data**, either because encryption is missing, weak, misused, or completely misunderstood.

This category does not mean “encryption was not used at all.”  
In many real-world incidents, encryption *was present*, but it was applied **incorrectly**, **incompletely**, or **without understanding the threat model**.

Cryptography is often treated as a checkbox:
> “We encrypted it, so we’re safe.”

In reality, cryptography is only effective when:
- The right algorithms are chosen
- Keys are generated, stored, rotated, and revoked securely
- Data is protected **in transit, at rest, and during processing**
- Developers understand *what they are protecting and from whom*

When any of these assumptions break, cryptography becomes a **false sense of security** rather than a defense.

This vulnerability class frequently leads to:
- Mass data breaches
- Credential exposure
- Regulatory violations
- Long-term trust erosion
