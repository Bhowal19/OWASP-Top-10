# A08 – Software & Data Integrity Failures

Data Integrity Failures occur when systems **do not verify that code, updates, or data are trustworthy before acting on them**.

Unlike availability or confidentiality failures, integrity failures are dangerous because nothing appears broken.
The system runs.
Processes complete.
Results are returned.

The problem is that the system can no longer guarantee that what it is executing or processing is authentic.

A08 exists because modern systems depend heavily on external inputs:
Software updates.
CI/CD artifacts.
Serialized objects.
Messages from queues.
Third-party plugins.
AI model inputs and outputs.

If integrity is not enforced, attackers do not need to breach the system.
They only need to influence what the system trusts.

When integrity fails, systems betray themselves.
