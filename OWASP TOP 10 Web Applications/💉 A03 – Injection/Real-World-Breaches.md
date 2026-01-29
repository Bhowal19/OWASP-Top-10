# Real-World Breaches Mapped to Injection

Injection vulnerabilities are responsible for some of the most damaging breaches in history.
What makes these incidents notable is that many occurred in systems believed to be “modern” or “secure by default.”

🗄️ TalkTalk – SQL Injection Breach
TalkTalk suffered a major breach when attackers exploited a basic SQL Injection vulnerability.
Personal data of hundreds of thousands of customers was exposed.

The application was not ancient.
It was not experimental.
It was a production system with real users.

The breach demonstrated a recurring truth:
Injection does not require sophistication.
It requires opportunity.

🏦 Heartland Payment Systems – Injection at Scale
Heartland Payment Systems was breached through SQL Injection, leading to the theft of over 130 million credit card numbers.

The attackers did not break cryptography.
They did not bypass firewalls.
They injected commands into trusted systems and let the infrastructure betray itself.

This incident showed how injection can scale from a single input flaw into an industry-wide disaster.

🧬 GitHub – Indirect Injection Lessons
While GitHub has not suffered a classic SQL Injection breach, it has repeatedly highlighted injection risks in APIs and CI/CD pipelines.

Many vulnerabilities reported through GitHub involve command injection in automation scripts and workflows.
These are injection vulnerabilities in modern clothing.

Injection adapts to whatever system executes instructions.