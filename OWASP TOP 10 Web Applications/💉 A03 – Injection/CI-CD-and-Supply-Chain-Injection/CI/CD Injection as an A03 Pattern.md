CI/CD injection fits squarely into A03 because the underlying failure is unchanged.

Untrusted input is being interpreted as executable instructions.

The interpreter is not SQL or a shell alone.
It is the entire automation ecosystem.

The reason CI/CD injection is often missed in OWASP discussions is historical.
OWASP focused on runtime applications.
Modern breaches focus on build-time execution.

The category did not change.
The execution layer did.

Exploitation Flow: CI/CD Injection

A typical CI/CD injection flow looks like this:

An attacker submits a pull request.
They modify a pipeline configuration or influence a parameter.
The pipeline executes injected commands.
Secrets are accessed.
Artifacts are modified.
Signed, trusted outputs are produced.

Downstream systems deploy the compromised artifact.
The attacker never touches production directly.

This is why CI/CD injection is often detected months later.
The compromise travels forward in time.

Secure Design Thinking for CI/CD and Supply Chain

Defending against CI/CD and supply chain injection requires abandoning implicit trust.

Pipelines must treat all inputs as hostile, including those from internal developers.
Execution environments must be isolated.
Secrets must be scoped tightly and rotated frequently.

Build systems should separate:
- Code evaluation
- Artifact generation
- Signing
- Deployment

No single step should have universal trust.

Dependencies must be verified, pinned, and monitored.
Builds must be reproducible.
Artifacts must be attestable.

Most importantly, organizations must accept a hard truth:
If your pipeline is compromised, your product is compromised.

CI/CD security is not DevOps hygiene.
It is product security.


Injection Everywhere: The Final A03 Lesson

Injection is not about SQL.
It is about execution.

Wherever systems:
- Interpret input
- Execute instructions
- Trust upstream components

Injection exists.

Modern software systems are chains of interpreters.
CI/CD and supply chains are simply the most powerful ones.

If injection reaches them, the attacker does not need persistence.
They become part of the system itself.
