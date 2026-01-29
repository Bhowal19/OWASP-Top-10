# Real-World Breaches Mapped to A02 – Cryptographic Failures

Cryptographic failures are not theoretical.
They are responsible for some of the most expensive and trust-destroying breaches in history.

What makes these incidents notable is that **encryption often existed**, but failed due to poor design or execution.

Equifax (2017)

### :contentReference[oaicite:0]{index=0} – 2017 Data Breach

Equifax exposed the personal data of over 140 million individuals.
While the breach is often associated with a vulnerable component, cryptographic failure played a critical role.

Sensitive data was stored in systems where encryption was either missing or ineffective.
Once attackers gained access, vast amounts of data were immediately readable.

This incident demonstrated a core A02 lesson:
If a single vulnerability grants access to unencrypted sensitive data, encryption has already failed.

🔓 LinkedIn (2012)

### :contentReference[oaicite:1]{index=1} – Password Breach

LinkedIn suffered a massive password breach when attackers obtained hashed passwords stored using SHA-1 without proper salting.

At the time, hashing was considered sufficient.
In reality, the algorithm choice made password recovery trivial at scale.

This breach redefined industry standards for password storage and highlighted how **outdated cryptography ages into vulnerability**.

🔓 Adobe (2013)

### :contentReference[oaicite:2]{index=2} – Encrypted but Exposed

Adobe stored user passwords using encryption rather than hashing, and reused encryption keys across users.

When attackers breached the system, they obtained both encrypted passwords and the cryptographic structure protecting them.
This allowed attackers to recover passwords and analyze patterns.

This incident reinforced a critical principle:
Encryption is not a substitute for purpose-built cryptographic controls.

🔓 Uber (2016)

### :contentReference[oaicite:3]{index=3} – Hardcoded Secrets

Uber’s breach involved credentials hardcoded in source code repositories.
While not a traditional “encryption failure,” it represents a **key management failure**, which is central to A02.

Once secrets are exposed, encryption becomes irrelevant.
Attackers can authenticate legitimately and access protected systems directly.

This breach highlighted how cryptographic strength is meaningless without secure key handling.

🔓 Cloud Metadata Attacks (Multiple Incidents)

### Cloud Service Breaches – Metadata Exposure

Numerous cloud breaches have involved attackers accessing cloud metadata services to extract credentials.

While cloud providers encrypt infrastructure, application-level cryptographic failures allowed attackers to:
- Access metadata endpoints
- Retrieve temporary credentials
- Decrypt or access protected resources

These incidents demonstrate that **cryptography does not compensate for poor isolation and access control**.

🧠 Product & AI Security Takeaway

A02 is not about choosing AES over DES.
It is about understanding that cryptography:

- Must be designed at the system level
- Must evolve with threat models
- Must assume breach
- Must protect data even when everything else fails

In Product Security, cryptography limits blast radius.
In AI Security, it protects trust, privacy, and irreversibility.

When cryptography fails, recovery is often impossible.
