# Code-Level Examples

Logging failures are often visible in code as absence rather than error.

Consider authentication logic.

```java
if (authenticate(user)) {
    grantAccess();
}

The code works.
The login succeeds.
Nothing is recorded.

A secure system would capture context.

if (authenticate(user)) {
    log.info("User login success", user, requestMetadata);
    grantAccess();
}


Another common issue is logging only failures.

try:
    process_payment()
except Exception:
    log.error("Payment failed")


Successful but suspicious behavior remains invisible.

Logging that cannot be correlated, enriched, or analyzed is functionally equivalent to no logging at all.