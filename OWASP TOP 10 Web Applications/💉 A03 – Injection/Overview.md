# A03 – Injection

Injection vulnerabilities occur when an application allows untrusted input to be interpreted as part of a command, query, or instruction.

At its core, injection is not a bug in syntax.
It is a **failure to separate data from instructions**.

Applications are built to process user input.
Databases, operating systems, template engines, and interpreters are built to execute commands.
Injection happens when these two worlds collide without a clear boundary.

Despite being one of the oldest vulnerability classes, injection remains one of the most exploited because it scales extremely well for attackers.
A single injection point can expose entire databases, execute arbitrary commands, or compromise underlying infrastructure.

Injection is dangerous not because attackers are clever,
but because systems are **too trusting by default**.
