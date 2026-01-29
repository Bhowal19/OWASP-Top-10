# A04 – Insecure Design

Insecure Design refers to weaknesses that originate **before code is written**.
Unlike implementation bugs, these flaws are baked into the system’s architecture, workflows, and assumptions.

An application with insecure design can be perfectly coded and still be fundamentally unsafe.

This category exists because many security failures are not caused by missing input validation or outdated libraries.
They are caused by systems that were never designed to resist abuse.

Insecure design emerges when teams focus on functionality without modeling how that functionality can be misused.
Attackers do not exploit syntax.
They exploit assumptions.

When design fails, every line of code faithfully implements insecurity.
