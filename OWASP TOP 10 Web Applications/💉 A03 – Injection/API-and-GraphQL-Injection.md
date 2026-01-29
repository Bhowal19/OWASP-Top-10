# A03 – Injection in APIs and GraphQL

Injection did not disappear when applications moved from web forms to APIs.
It simply changed shape.

APIs are often perceived as safer because they are structured.
They accept JSON.
They enforce schemas.
They are not “raw SQL forms.”

This perception is dangerously wrong.

APIs still accept untrusted input.
That input is still used to construct queries, filters, conditions, and downstream requests.
The interpreter has changed, but the vulnerability remains.

In REST APIs, injection frequently appears in filtering and search endpoints.
Developers dynamically construct database queries based on user-provided parameters such as sort order, filters, or ranges.
When these parameters are concatenated into queries without strict binding, injection becomes possible.

GraphQL introduces a different but equally powerful attack surface.
Because GraphQL allows clients to define *what* data they want, attackers can manipulate query depth, complexity, and resolver behavior.
Injection in GraphQL is often less about syntax breaking and more about **logic manipulation**.

A GraphQL resolver may trust arguments blindly.
Those arguments are passed into database queries or internal services.
If resolver logic assumes “valid GraphQL input equals safe input,” injection follows.

The most dangerous aspect of API and GraphQL injection is **blast radius**.
APIs often sit directly on top of core business logic.
Once compromised, attackers bypass frontend controls entirely and operate at the system’s heart.

Injection survived the shift to APIs because the real problem was never HTML.
It was trust.
