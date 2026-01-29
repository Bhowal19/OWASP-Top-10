# Code-Level Examples

Authentication failures often appear in code that looks reasonable.

Consider password verification logic.

```java
if (inputPassword.equals(storedPassword)) {
    authenticateUser();
}

The comparison works.
The logic is clear.
The failure lies in how the password is stored.

If the password is stored in plaintext or weakly hashed, compromise is inevitable.

Session management issues are even subtler.

res.cookie("session", sessionId);


If the session ID is predictable, long-lived, or transmitted without proper flags, it becomes an attack vector.

Secure authentication code rarely looks complex.
The complexity lies in everything around it:
storage, lifecycle, rotation, expiration, and invalidation.

Authentication failures are not syntax errors.
They are context failures.