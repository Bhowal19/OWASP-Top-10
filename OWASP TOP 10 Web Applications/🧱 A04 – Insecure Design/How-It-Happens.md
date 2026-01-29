# How Insecure Design Happens

Insecure design usually begins with pressure.

Teams are asked to move fast.
Deadlines matter more than edge cases.
Security is assumed to be “handled later.”

During early design discussions, the system is described in terms of happy paths.
Users sign up.
Users log in.
Users perform actions.

What is missing are the unhappy paths.
The malicious paths.
The abusive paths.

Design documents often describe what the system should do, not what it must never allow.
As a result, authorization rules are vague.
Rate limits are undefined.
Trust boundaries are blurred.

Insecure design also arises from overconfidence in controls that exist elsewhere.
Teams assume that network security, authentication, or cloud isolation will compensate for missing design-level defenses.

Once these assumptions are encoded into architecture, they become extremely expensive to correct.
At that point, developers are no longer fixing bugs.
They are fighting the system itself.

Insecure design is rarely intentional.
It is the natural outcome of building systems without a threat model.
