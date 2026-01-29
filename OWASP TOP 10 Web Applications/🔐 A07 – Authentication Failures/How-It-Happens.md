# How Authentication Failures Happen

Authentication failures rarely stem from a single mistake.
They emerge from a chain of assumptions.

Developers assume users will choose strong passwords.
They assume attackers will not automate login attempts.
They assume session tokens will remain secret.
They assume recovery flows will not be abused.

These assumptions hold during testing.
They collapse in production.

One of the most common causes is over-reliance on passwords.
Passwords are shared, reused, phished, leaked, and guessed.
Systems that treat passwords as sufficient proof of identity inherit all of these weaknesses.

Another cause is flawed session management.
Tokens are long-lived.
Tokens are predictable.
Tokens are not invalidated after logout or password change.
Once stolen, they provide persistent access.

Authentication failures also occur in edge cases.
Password reset flows.
Account recovery.
First-time login.
Single sign-on integrations.

These flows are often implemented hastily and tested lightly.
Attackers focus on them relentlessly.

Authentication breaks not because teams do not understand login.
It breaks because identity is treated as a feature rather than a security boundary.
