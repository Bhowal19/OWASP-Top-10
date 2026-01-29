# Detection

Insecure design is difficult to detect with automated tools because the system behaves exactly as designed.

Detection usually begins with architectural review.
Security engineers ask questions about intent, trust, and abuse.

They examine workflows rather than endpoints.
They look for missing constraints.
They ask what happens when a feature is used at scale or in unintended sequences.

During penetration testing, insecure design reveals itself through logic flaws.
The attacker does not break rules.
They follow them too well.

In production, signals include abuse patterns rather than exploit traces.
Sudden spikes in resource usage.
Financial loss without technical compromise.
Actions that appear legitimate but harmful.

Detection requires understanding not just how the system works, but how it can be **used against itself**.
