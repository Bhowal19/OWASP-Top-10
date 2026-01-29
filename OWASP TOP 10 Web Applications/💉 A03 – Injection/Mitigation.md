# Mitigation

Mitigating injection vulnerabilities begins with a fundamental shift in how systems treat input.

All external input must be assumed hostile.
This includes data from users, APIs, files, and even internal services.

The most effective mitigation is **parameterization**.
Queries and commands must define their structure independently of user-supplied values.

Input validation helps, but it is not sufficient on its own.
Attackers are skilled at bypassing filters and escaping constraints.
Validation reduces noise.
Separation eliminates risk.

Least privilege also plays a critical role.
If an injected query executes, its impact should be limited.
Databases should not run with administrative privileges.
Operating system commands should be constrained.

Mitigation is successful when injection attempts become harmless input rather than executable logic.
