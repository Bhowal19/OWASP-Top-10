# A03 – Injection in CI/CD Pipelines and the Software Supply Chain

Injection does not stop at applications.
It follows execution.

Modern software systems execute far more than code written by developers.
They execute:
- Build scripts
- Pipeline definitions
- Dependency manifests
- Configuration files
- Workflow instructions
- Third-party automation logic

CI/CD systems are interpreters.
Package managers are interpreters.
Infrastructure-as-Code engines are interpreters.

Wherever instructions are executed, injection becomes possible.

The difference is scale.
A successful injection in CI/CD does not compromise one application.
It compromises **everything that application produces**.
