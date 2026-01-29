# Detection

Detecting vulnerable components requires visibility into what the system is actually made of.

Traditional penetration testing may not reveal these vulnerabilities unless they are actively exploitable from the outside.
Source code review may miss them entirely.

Detection often begins with inventory.
Teams must know which components they use, in which versions, and where they are deployed.

Automated dependency analysis tools help, but they are not sufficient on their own.
They identify known vulnerabilities, but they do not assess exploitability in context.

Operational signals can also reveal component risk.
Unexpected outbound connections.
Strange runtime behavior.
Crashes triggered by malformed input.

Detection is challenging because vulnerable components do not announce themselves.
They wait quietly for someone else to find them.