# Attack Scenarios

A cloud storage bucket is created to share files internally.
Access controls are left open for convenience.
No one notices.
Search engines index it.
Sensitive data becomes public.

An application framework exposes a management console intended for debugging.
It is deployed to production without authentication.
Attackers discover it and gain full control over the application.

A container orchestration platform exposes an internal API without proper network segmentation.
An attacker compromises a low-privilege service and pivots through misconfigured internal endpoints.

In these scenarios, attackers do not bypass controls.
They follow them.
The system behaves exactly as configured.

Security misconfiguration enables attacks that leave no exploit trace.
There is no injection payload.
No malformed input.
Only access that should never have been possible.

This is why misconfiguration breaches often go unnoticed for long periods.
There is nothing “wrong” happening from the system’s perspective.
