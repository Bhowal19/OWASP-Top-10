# Detection

Injection vulnerabilities often reveal themselves through inconsistent or unexpected application behavior.

During manual testing, security engineers observe how the application reacts to malformed input.
Unexpected errors, time delays, or logic changes can indicate that input is being executed rather than processed.

Automated scanners can identify common injection patterns, but they often miss context-specific cases.
False positives are common, and false negatives are dangerous.

Source code review is one of the most reliable detection methods.
Patterns such as string concatenation, dynamic query construction, and direct command execution are red flags.

In production environments, injection attempts frequently appear in logs.
Repeated malformed inputs, unusual query errors, or abnormal response times can signal exploitation attempts.

Detection is difficult because injection does not always cause failure.
Sometimes, it works exactly as the attacker intends.