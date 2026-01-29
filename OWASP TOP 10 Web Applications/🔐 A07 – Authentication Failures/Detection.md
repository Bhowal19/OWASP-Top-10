# Detection

Detecting authentication failures requires observing behavior over time, not single requests.

Credential stuffing and brute-force attacks often appear as normal login traffic.
Only volume, velocity, and distribution reveal abuse.

Session hijacking is even harder to detect.
From the application’s perspective, the session is valid.
There is no error, no anomaly in logic.

Detection relies on signals.
Unusual login patterns.
Geographic inconsistencies.
Rapid account switching.
Repeated authentication failures followed by success.

Logs matter.
Authentication systems without detailed logging operate blind.
Without visibility into attempts, failures, and session lifecycle events, abuse becomes invisible.

Authentication failures are often detected by users first.
By the time alerts trigger, damage is already done.