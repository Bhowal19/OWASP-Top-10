# Mitigation

Mitigating insecure design starts with acknowledging that security is not a layer added later.
It is a property of system behavior.

Threat modeling is the primary defense.
Before building features, teams must identify assets, adversaries, and abuse cases.
This shifts thinking from “how it works” to “how it breaks.”

Security requirements must be explicit.
Ownership rules.
Rate limits.
State transitions.
Failure conditions.

These requirements should exist before code and be enforced consistently.

Mitigation also involves removing unnecessary complexity.
The more flexible a system is, the more opportunity it provides for abuse.
Secure systems are intentionally constrained.

Insecure design is mitigated not by patches, but by decisions.
