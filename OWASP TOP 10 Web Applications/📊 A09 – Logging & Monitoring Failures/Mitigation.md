# Mitigation

Mitigating logging and monitoring failures requires designing for detection.

Security-relevant events must be logged deliberately.
Authentication attempts.
Authorization decisions.
Privilege changes.
Sensitive operations.

Logs must include context.
Who performed the action.
What was affected.
Where it originated.
When it occurred.

Monitoring must focus on behavior, not just errors.
Abuse often looks like success.
Alerts must reflect that reality.

Logs must be centralized, protected, and retained.
Attackers often attempt to erase evidence.
Logs stored only locally cannot be trusted.

Mitigation succeeds when attackers cannot operate quietly.
