# A07 – Identification & Authentication Failures

Authentication failures occur when systems incorrectly implement or rely on mechanisms used to verify a user’s identity.

At a glance, authentication appears simple.
A user provides credentials.
The system verifies them.
Access is granted.

In reality, authentication is one of the most complex and failure-prone parts of any system.
It must handle secrecy, lifecycle, recovery, abuse, automation, and scale.

A07 exists because many systems authenticate users successfully, yet still fail to protect identity.
Passwords are guessed.
Sessions are stolen.
Tokens are reused.
Recovery flows are abused.

When authentication fails, attackers do not need to bypass authorization or exploit logic.
They simply **become someone else**.

This makes authentication failures uniquely dangerous.
They turn the system against itself.
