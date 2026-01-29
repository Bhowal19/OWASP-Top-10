# A06 – Vulnerable & Outdated Components

Vulnerable components are security risks introduced not by what a team builds, but by what it depends on.

Modern applications are no longer single codebases.
They are ecosystems assembled from frameworks, libraries, containers, runtime platforms, and third-party services.
Every dependency brings functionality.
Every dependency also brings its own attack surface.

A06 exists because software today is mostly written by someone else.

When a vulnerability is discovered in a component, the application using it becomes vulnerable immediately, often without any code changes.
The risk is inherited automatically.

This category is dangerous because responsibility is ambiguous.
Developers did not write the vulnerable code.
Operations teams did not deploy it incorrectly.
Yet the system is compromised all the same.

A06 represents the security cost of speed, reuse, and abstraction.
