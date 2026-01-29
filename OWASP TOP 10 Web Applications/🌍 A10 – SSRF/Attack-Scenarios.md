# Attack Scenarios

A web application allows users to submit a URL for image processing.
The backend fetches the image and resizes it.
An attacker supplies a URL pointing to an internal admin service.
The server retrieves it successfully.
Sensitive internal data is returned in the response.

In a cloud-hosted application, an attacker uses SSRF to access the cloud metadata endpoint.
The server fetches credentials associated with its role.
The attacker extracts temporary access keys.
They now have direct access to cloud APIs.

In a microservices environment, an internal billing service listens on a private network without authentication.
SSRF allows attackers to send requests to it.
Invoices are generated.
Accounts are modified.
No perimeter control is triggered.

In these scenarios, firewalls, authentication, and access control all exist.
They fail because the **request originates from a trusted server**.

SSRF is not about bypassing security.
It is about abusing trust.
