# Detection

SSRF is difficult to detect because the traffic originates from legitimate servers.

Traditional intrusion detection systems focus on inbound attacks.
SSRF generates outbound requests.

Detection often begins with unusual outbound behavior.
Unexpected connections to internal IP ranges.
Requests to metadata endpoints.
Internal services accessed from components that should never interact.

Application logs may show strange URLs being processed.
However, without context, these appear as normal feature usage.

In cloud environments, SSRF is often detected after credential abuse.
Logs show API calls originating from application roles at unexpected times or scopes.

SSRF detection requires visibility into **where servers are talking**, not just who is talking to them.