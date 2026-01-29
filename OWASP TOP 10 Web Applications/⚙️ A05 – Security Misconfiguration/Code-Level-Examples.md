# Code-Level Examples

Security misconfiguration often appears as harmless configuration choices in code or infrastructure files.

Consider a web application deployed with debug mode enabled.

```python
app.run(debug=True)
This configuration provides verbose error messages and stack traces.
In production, it can reveal internal logic, file paths, secrets, and framework internals.

Another common example involves permissive access controls.

{
  "Version": "2012-10-17",
  "Statement": [{
    "Effect": "Allow",
    "Principal": "*",
    "Action": "*",
    "Resource": "*"
  }]
}


This configuration technically works.
It allows the system to function without friction.
It also removes all security boundaries.

The code is not broken.
The configuration is not invalid.
The system is insecure because the rules allow it to be insecure.

Security misconfiguration is rarely a coding mistake.
It is a decision encoded into configuration.


