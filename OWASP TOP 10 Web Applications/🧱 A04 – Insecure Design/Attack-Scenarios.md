# Attack Scenarios

Consider a financial application that allows users to transfer funds between accounts.
The design assumes that users will only transfer money between accounts they own.

The system authenticates users correctly.
The code validates inputs correctly.
Yet the design never explicitly enforces ownership.

An attacker discovers they can reference another user’s account identifier.
The transfer succeeds.
Funds move.
No vulnerability scanner detects this.

In another scenario, an e-commerce platform allows unlimited coupon generation because marketing requirements demanded flexibility.
No abuse case was considered.
Attackers automate coupon creation and drain revenue.

Insecure design often appears in rate-limited features.
Password reset mechanisms without throttling.
Search endpoints without cost modeling.
API endpoints designed for convenience, not resilience.

These attacks are not clever.
They are logical.
They exploit what the system allows by design.

When attackers succeed, defenders often say:
“There was no vulnerability.”

From a design perspective, that is the problem.
