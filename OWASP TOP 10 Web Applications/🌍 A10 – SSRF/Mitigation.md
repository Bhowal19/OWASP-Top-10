# Mitigation

Mitigating SSRF requires eliminating implicit trust in outbound requests.

Servers must not be allowed to fetch arbitrary destinations.
URL allowlists should be enforced.
DNS resolution should be validated.
IP ranges should be restricted explicitly.

Network-level controls are critical.
Servers should not be able to reach internal admin interfaces or metadata endpoints unless absolutely necessary.
Cloud providers offer controls to restrict metadata access.
They must be used intentionally.

Request libraries should be configured defensively.
Redirects should be limited.
Protocols should be restricted.
Timeouts should be enforced.

Mitigation succeeds when an attacker-controlled URL cannot cause the server to cross a trust boundary.
