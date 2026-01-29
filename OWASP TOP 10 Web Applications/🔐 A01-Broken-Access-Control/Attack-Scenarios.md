# Attack Scenarios

## Scenario 1: IDOR (Insecure Direct Object Reference)
An attacker modifies an object ID in a request and accesses another user's data.

## Scenario 2: Privilege Escalation
A normal user accesses an admin endpoint directly via API.

## Scenario 3: Missing Function-Level Authorization
Backend APIs assume frontend already validated permissions.

## Impact
- Unauthorized data access
- Account compromise
- Regulatory violations (GDPR, HIPAA)
