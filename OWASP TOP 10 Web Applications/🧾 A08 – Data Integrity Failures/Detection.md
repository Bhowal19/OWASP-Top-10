# Detection

Detecting integrity failures is challenging because systems continue to operate normally.

Traditional monitoring focuses on errors and outages.
Integrity failures produce neither.

Detection often begins after anomalous behavior appears.
Unexpected outbound traffic.
Unauthorized actions performed by trusted services.
Logic behaving correctly but producing harmful outcomes.

Audit trails are critical.
Without cryptographic verification, it is difficult to determine whether data or code was altered legitimately.

CI/CD integrity failures may be detected through mismatches between source code and deployed artifacts.
However, many organizations lack the visibility to make this comparison.

Integrity failures are often discovered too late, after trust has already been abused.