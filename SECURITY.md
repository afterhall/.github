# Security Policy

Afterhall stores some of the most private data a person can have: personal messages, voice recordings, memories and the keys that release them to heirs. We treat every security report accordingly.

## Reporting a vulnerability

**Please do not open a public issue for security problems.**

Report vulnerabilities privately through GitHub's **"Report a vulnerability"** button in the Security tab of the affected repository, or by email to **security@afterhall.app**.

Please include:

- the affected component and version or commit
- steps to reproduce, or a proof of concept
- the impact you expect (data exposure, key release, dead man's switch bypass, …)

We aim to acknowledge reports within **72 hours** and to agree on a disclosure timeline with you. We are happy to credit reporters unless you prefer to stay anonymous.

## Especially sensitive areas

Please flag these clearly in your report:

- **Dead man's switch and key release:** anything that could trigger a release too early, block it, or let someone other than the designated trustee confirm it
- **Vault separation:** any path from the legacy vault to the raw data vault or the pseudonym key table
- **Access levels:** any way to read entries outside one's own sharing groups
- **Third-party data:** any way to recover pseudonymised names or to get other people's messages quoted
- **Backups and export:** leaks of keys or unencrypted data

## Supported versions

Afterhall has not had a public release yet. Until then, only the latest `main` branch receives security fixes.

## Please do not

- access or alter data that is not your own
- run tests against other people's installations
- run denial-of-service tests against hosted services
