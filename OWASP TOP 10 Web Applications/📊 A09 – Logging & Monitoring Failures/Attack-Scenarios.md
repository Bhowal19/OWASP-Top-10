# Attack Scenarios

An attacker gains access to a system using valid credentials.
No exploit is used.
The system logs nothing beyond a successful login.

The attacker escalates privileges through misconfigured roles.
No alert triggers.
The actions are allowed by design.

Over weeks, data is exfiltrated slowly to avoid detection.
Requests look normal.
Traffic stays under thresholds.

When the breach is finally discovered, logs are incomplete.
Critical events were never recorded.
The organization cannot determine what was accessed or when.

In another scenario, attackers deliberately trigger errors to map system behavior.
Verbose errors are logged locally but never forwarded.
Security teams never see reconnaissance in progress.

Attackers do not fear detection.
They fear investigation.
Logging failures ensure neither happens.
