# Attack Scenarios

Imagine a login form that checks credentials against a database.
The developer constructs a SQL query using user-supplied values.

An attacker enters carefully crafted input that alters the logic of the query.
Instead of validating credentials, the database is instructed to always return success.
Authentication is bypassed without knowing a single password.

In another scenario, a file upload feature allows users to process images.
Behind the scenes, the application calls an operating system command to manipulate the file.
The attacker injects additional shell commands into the filename.
The server executes them blindly.

Injection is not limited to SQL or operating systems.
Modern applications are vulnerable through:
- NoSQL queries
- LDAP lookups
- XPath expressions
- Template engines
- Cloud service queries

In real-world breaches, attackers rarely stop at proof of concept.
Once injection is confirmed, it becomes a pivot point.
Databases are dumped.
Systems are enumerated.
Credentials are harvested.
Infrastructure is mapped.

Injection is rarely the final step.
It is the **entry point**.
    