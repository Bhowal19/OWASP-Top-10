# A02 – Cryptographic Failures in AI & LLM Systems

Cryptographic failures in AI systems are more subtle and often more damaging than in traditional applications.

AI systems process and generate data at scale.
They ingest:
- User prompts
- Proprietary datasets
- Internal documents
- Sensitive personal information

When cryptography fails in AI pipelines, the impact is not limited to data exposure.
It can permanently contaminate models, logs, and downstream outputs.

One common failure is **unencrypted prompt and response storage**.
Prompts may contain confidential business logic, legal documents, or medical data.
If stored or logged in plaintext, this data becomes a breach waiting to happen.

Another failure arises in **model training pipelines**.
Training data is often aggregated from multiple sources and environments.
If datasets are stored without encryption or integrity guarantees, attackers can access or manipulate them.
This can lead not only to data leakage, but to **model poisoning**.

API key exposure is one of the most frequent AI-related cryptographic failures.
LLM API keys hardcoded into applications or stored in plaintext configuration files allow attackers to:
- Abuse paid resources
- Extract model outputs
- Perform indirect data exfiltration

In AI systems, cryptographic failures also intersect with **privacy guarantees**.
Once sensitive data is exposed to a model, it may be memorized.
Unlike traditional databases, this leakage may not be reversible.

For AI security, cryptography must protect:
- Data at rest (datasets, embeddings, logs)
- Data in transit (API calls, plugins, agents)
- Secrets (API keys, signing keys, credentials)
- Model artifacts (weights, fine-tuned outputs)

Failure in any of these areas transforms AI from an innovation engine into a compliance and trust disaster.
