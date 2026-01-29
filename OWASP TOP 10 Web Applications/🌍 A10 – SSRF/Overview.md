# A10 – Server-Side Request Forgery (SSRF)

Server-Side Request Forgery occurs when an application allows an attacker to influence or control requests made by the server itself.

At a surface level, SSRF appears simple.
An application fetches a URL.
The attacker changes that URL.
The server makes a request.

In reality, SSRF is dangerous because servers live in a position of trust.
They can access internal networks.
They can reach private services.
They can query cloud metadata endpoints.
They can authenticate to other systems automatically.

When SSRF exists, attackers do not attack the server.
They **become the server**.

A10 exists because modern architectures increasingly rely on internal HTTP-based communication.
Microservices, cloud APIs, metadata services, and internal admin panels all assume the server is a trusted actor.

SSRF breaks that assumption completely.
