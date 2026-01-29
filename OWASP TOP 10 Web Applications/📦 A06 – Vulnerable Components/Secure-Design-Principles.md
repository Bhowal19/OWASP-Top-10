# Secure Design Principles

Secure design acknowledges that third-party code will fail.

Systems should be designed so that dependencies are constrained by architecture.
Clear boundaries, limited privileges, and defense in depth reduce the impact of component vulnerabilities.

Dependency selection should be intentional.
Popularity alone is not a security guarantee.
Maintenance activity, transparency, and responsiveness matter more.

Designs should assume delayed patching.
Even when fixes exist, deployment takes time.
Systems must remain safe during that window.

Most importantly, secure design treats the supply chain as part of the threat model.
If a system depends on it, it must defend against it.

Vulnerable components are not an anomaly.
They are the cost of modern software.
Secure systems are those that plan for that cost.
