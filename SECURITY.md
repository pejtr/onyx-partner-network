# Security Policy

Do not publish credentials, customer data, private contracts or production configuration in this repository.

## Report a vulnerability

If a report contains sensitive details, do not open a public GitHub issue. Contact the repository owner through a private channel and include only the minimum information needed to reproduce the issue.

## Integration requirements

- Credentials must live in private secret stores.
- Examples must use placeholders.
- Webhooks should be authenticated and replay-resistant.
- Partner capabilities should follow least privilege.
- Production ONYX OS internals are intentionally outside this public repository.
