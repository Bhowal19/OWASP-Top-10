# Attack Scenarios

A widely used logging library contains a remote code execution vulnerability.
An attacker sends a specially crafted input that triggers the vulnerable code path.
The application executes attacker-controlled commands.

The development team never wrote code that executes user input.
Yet the system is compromised.

In another scenario, a web framework dependency includes an insecure deserialization flaw.
An attacker supplies a malicious payload.
The framework processes it internally.
The application is breached without a single vulnerable line of business logic.

Supply chain attacks often begin far upstream.
A compromised package is published to a public registry.
Applications install it automatically.
Malicious code executes during build or runtime.

In these cases, attackers do not target the application directly.
They target the ecosystem around it.

The attack surface is no longer your code.
It is your dependency graph.
