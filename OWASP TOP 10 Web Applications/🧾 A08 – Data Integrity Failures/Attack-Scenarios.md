# Attack Scenarios

A software vendor distributes updates over an unsecured channel.
Attackers intercept the update process and inject malicious code.
Customers install the update willingly.
The compromise spreads downstream.

In another scenario, a web application deserializes user-supplied data into server-side objects.
The application expects simple configuration data.
The attacker supplies a crafted payload that executes code during deserialization.
No authentication is bypassed.
No vulnerability is exploited in logic.
The system executes what it was told to trust.

A CI/CD pipeline builds artifacts and stores them in a shared repository.
An attacker with limited access replaces a legitimate artifact with a malicious one.
The deployment system retrieves it automatically.
Production is compromised without touching source code.

In each case, the attacker does not break controls.
They exploit the absence of verification.
