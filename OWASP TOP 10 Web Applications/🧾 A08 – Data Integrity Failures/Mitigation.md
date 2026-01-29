# Mitigation

Mitigating data integrity failures requires systems to **prove trust instead of assuming it**.

Code, updates, and artifacts must be signed and verified before execution.
Data that triggers behavior must be authenticated and validated.
Serialization mechanisms must be restricted or replaced with safer formats.

CI/CD pipelines must enforce integrity from source to production.
Artifacts should be immutable and traceable.
Each stage must verify what it receives.

Least privilege reduces impact.
Even if integrity fails, compromised components should not have unlimited power.

Mitigation is successful when systems refuse to act on unverified input, even if that input appears valid.
