# Mitigation

Mitigating authentication failures requires accepting that credentials will leak.

Passwords must be treated as weak signals, not proof.
Strong hashing, salting, and adaptive algorithms slow attackers but do not stop them.

Multi-factor authentication adds friction that attackers struggle to bypass at scale.
It transforms credential theft from a direct compromise into a partial failure.

Session management must be strict.
Sessions should expire.
Sessions should be bound to context.
Sessions should be invalidated aggressively when risk changes.

Authentication flows must be rate-limited and monitored.
Recovery mechanisms must be as hardened as primary login paths.

Mitigation succeeds when identity compromise becomes expensive, noisy, and short-lived.
