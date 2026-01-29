# Code-Level Examples

A common insecure pattern involves hashing passwords using fast, outdated algorithms.

## Insecure Example

```java
MessageDigest md = MessageDigest.getInstance("MD5");
byte[] hash = md.digest(password.getBytes());

This approach is insecure because MD5 is fast and predictable. Attackers can brute-force or precompute hashes easily.

BCryptPasswordEncoder encoder = new BCryptPasswordEncoder();
String hash = encoder.encode(password);

Here, a slow, adaptive hashing algorithm is used, making large-scale password cracking impractical.

Another frequent issue involves hardcoded encryption keys.

Insecure Example

SECRET_KEY = "my-super-secret-key"
cipher = AES.new(SECRET_KEY)

If this code is ever leaked, logged, or pushed to a repository, the encryption is permanently compromised.

Secure Example

Keys should be generated securely and stored in a dedicated key management system, never in source code.

The difference between these examples is not syntax—it is security thinking.