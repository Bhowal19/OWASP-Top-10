# Mitigation

Mitigating vulnerable components requires accepting a difficult truth:
dependency risk cannot be eliminated, only managed.

The first step is visibility.
Teams must maintain accurate records of the components they rely on.
Without this, response is impossible.

Updates must be treated as a security activity, not just a maintenance task.
When vulnerabilities are disclosed, organizations must be able to assess impact and deploy fixes quickly.

Isolation reduces risk.
Components should run with minimal privileges.
A vulnerability in one library should not grant access to the entire system.

In some cases, mitigation means removal.
Unused dependencies should be eliminated.
Features that exist only because a library made them convenient should be questioned.

Mitigation succeeds when dependency compromise does not equal system compromise.
