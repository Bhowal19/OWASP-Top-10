# How SSRF Happens

SSRF usually begins with a legitimate feature.

Applications fetch URLs to:
Preview links.
Download files.
Integrate third-party APIs.
Process images.
Validate webhooks.

The developer assumes that the URL points to an external resource.
The server assumes it is safe to fetch.
Neither considers what else the server can reach.

The vulnerability appears when user-controlled input is passed directly into request logic.
The server does not distinguish between public internet destinations and internal resources.

In cloud environments, SSRF becomes more dangerous because infrastructure exposes metadata services on internal IP addresses.
These services are designed to be accessible only from trusted servers.
SSRF turns user input into that trusted server.

SSRF also thrives in microservice architectures.
Internal services are not authenticated because they assume network-level trust.
An attacker using SSRF bypasses that trust boundary entirely.

SSRF is rarely introduced by malicious code.
It is introduced by **implicit trust in where requests will go**.
