CI/CD injection rarely begins with malicious intent.
It begins with convenience.

Pipelines are designed to be flexible.
They accept parameters.
They run scripts.
They pull code dynamically.
They react to pull requests, commits, tags, and environment variables.

This flexibility is the attack surface.

A common pattern involves user-controlled input being passed directly into shell commands inside pipelines.
Branch names, commit messages, PR titles, and environment variables are assumed to be safe because they originate from “developers.”

Attackers understand this assumption.

When a pipeline executes:
`bash build.sh $BRANCH_NAME`

the pipeline is trusting that `$BRANCH_NAME` contains data, not instructions.
The shell does not care.
It executes whatever it receives.

CI/CD injection also occurs through configuration files.
YAML pipelines may reference external scripts or templates.
Those references can be modified in pull requests.
If reviews focus on application code but not pipeline logic, the attacker wins.

The most dangerous failures occur when pipelines run with high privileges.
Cloud credentials.
Signing keys.
Deployment permissions.
Once injected, attackers inherit the trust of the pipeline itself.

Injection in CI/CD is not loud.
Builds still pass.
Deployments still succeed.
The compromise happens invisibly, upstream.
