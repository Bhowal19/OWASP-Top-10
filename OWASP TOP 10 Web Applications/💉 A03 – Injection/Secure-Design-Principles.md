# Secure Design Principles

Secure design treats injection as an architectural concern, not an implementation detail.

Systems should be built so that untrusted input can never alter control flow.
This is achieved through strong abstractions that make unsafe behavior impossible or extremely difficult.

Frameworks, ORMs, and APIs should enforce safe defaults.
When developers must opt out of safety, the risk should be explicit and justified.

Defense in depth matters.
Even if injection occurs, additional layers such as access control, monitoring, and isolation limit damage.

Most importantly, secure design assumes failure.
It assumes that input validation will eventually be bypassed.
It assumes that developers will make mistakes.
And it builds systems that remain safe anyway.

Injection is solved not by smarter developers,
but by **better system boundaries**.
