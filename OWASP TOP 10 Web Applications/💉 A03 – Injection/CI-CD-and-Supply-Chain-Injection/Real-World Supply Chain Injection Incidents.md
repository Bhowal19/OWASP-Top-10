Supply chain attacks demonstrate injection at the highest level of impact.

SolarWinds – Build Pipeline Injection

The SolarWinds breach did not begin with an exploit against customers.
It began inside the build process.

Attackers injected malicious logic into the software build pipeline.
The resulting signed updates were distributed to thousands of organizations.

Customers trusted the update.
Systems executed it willingly.

This was injection at the supply chain level:
instructions introduced upstream, executed downstream, trusted everywhere.

No firewall could stop it.
No WAF could detect it.

npm Package Takeovers

Multiple npm ecosystem incidents have involved attackers injecting malicious code into popular packages.

Sometimes credentials were stolen.
Sometimes maintainers were compromised.
Sometimes abandoned packages were claimed.

Once published, the injected code propagated automatically through dependency trees.

Applications executed malicious logic during installation or runtime, often without developers ever touching the code directly.

This is injection without interaction.

CI Token Abuse Incidents

Numerous breaches have involved attackers extracting CI secrets via injected build steps.

Once attackers inject commands into a pipeline, they can:
- Dump environment variables
- Exfiltrate cloud credentials
- Sign malicious artifacts
- Deploy backdoored services

The pipeline becomes the attacker.

