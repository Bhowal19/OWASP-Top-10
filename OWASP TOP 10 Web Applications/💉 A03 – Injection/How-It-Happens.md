# How Injection Happens

Injection vulnerabilities are almost never created intentionally.
They emerge from normal development practices under real-world constraints.

Developers often build queries dynamically.
User input is concatenated into SQL statements, shell commands, or template logic because it feels natural and flexible.
Early testing works fine because developers use expected input.
The system behaves correctly.

The problem appears when the application encounters **unexpected input**.

An application expects a username.
The attacker provides a fragment of a database query.
The application does not distinguish between the two.

This happens because the system treats all input as trusted text, rather than as untrusted data that must remain inert.

Injection also thrives in environments where speed matters more than structure.
Rapid feature delivery, legacy codebases, and inconsistent coding standards create fertile ground for injection flaws.

Another contributor is abstraction leakage.
Developers may rely on frameworks or ORMs but bypass safeguards for performance or convenience.
Once raw queries are introduced, the protection layer disappears silently.

Injection is not a failure of intelligence.
It is a failure of **boundaries**.
