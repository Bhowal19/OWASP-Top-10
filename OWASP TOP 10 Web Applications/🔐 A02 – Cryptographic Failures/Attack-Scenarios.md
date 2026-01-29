# Attack Scenarios

Consider a real-world scenario involving a healthcare web application storing patient records.

The application uses HTTPS, which gives users confidence that their data is protected.  
However, inside the backend, sensitive medical records are stored in a database without encryption at rest.

An attacker gains access through an unrelated vulnerability—perhaps SQL Injection or compromised credentials.  
Once inside, the attacker does not need to break encryption. The data is already readable.

In another common scenario, passwords are hashed using an outdated algorithm like MD5 without salting.  
An attacker obtains the password database through a breach. Instead of cracking passwords one by one, they use precomputed rainbow tables and recover thousands of user passwords in minutes.

A cloud-based application may encrypt files before storing them in object storage, but store the encryption key in an environment variable accessible to all application instances.  
When attackers exploit a server-side vulnerability, they retrieve both the encrypted data and the key from the same system—rendering encryption meaningless.

Transport-layer failures are equally dangerous.  
If HTTPS is not enforced everywhere, attackers positioned on the same network can intercept sensitive data through man-in-the-middle attacks. Login credentials, session tokens, and personal data can all be exposed without the attacker ever touching the server.

In all these cases, the attacker does not defeat cryptography.  
They simply **walk around it**.
