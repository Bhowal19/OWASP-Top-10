# Attack Scenarios

A large consumer platform experiences a credential stuffing attack.
Attackers use leaked username-password pairs from unrelated breaches.
Thousands of accounts are compromised without exploiting a single vulnerability.

From the system’s perspective, every login is valid.
From the user’s perspective, their account is gone.

In another scenario, a password reset mechanism allows unlimited attempts.
Attackers enumerate email addresses.
They trigger reset flows repeatedly.
Some users fall victim to phishing.
Others lose access due to account lockouts.

Session fixation attacks exploit systems that accept session identifiers from users.
An attacker forces a victim to use a known session ID.
Once the victim logs in, the attacker inherits the authenticated session.

Single sign-on misconfigurations allow attackers to forge identity assertions.
The application trusts the identity provider blindly.
The attacker logs in as any user.

In all these cases, the system behaves correctly according to its design.
The design itself is the vulnerability.
