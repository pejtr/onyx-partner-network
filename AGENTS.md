# Agent instructions

This is a **public repository**.

Before non-trivial work read:
- `README.md`
- `TODO.md`
- `SECURITY.md`
- `docs/PUBLIC_REPO_NO_TRUST.md`

## Documentation continuity

When public API contracts, integration patterns, schemas, security expectations or supported partner capabilities change, update README/TODO/relevant docs in the same PR.

## NO-TRUST publication rule

Do not copy content from private repositories, connected accounts, chats or local machines into this repository without explicit sanitization.

Never publish:
- secrets or secret-shaped values,
- internal infrastructure,
- real account/project identifiers,
- private prompts/memory,
- user/customer data,
- non-public commercial terms,
- proprietary internal routing/risk logic,
- privileged recovery procedures.

Use placeholders and public architecture roles.

## Truth

Use the state chain:
`CODE → TESTS/QA → PR → MERGED → DEPLOYED/LIVE`

A merge or green CI run is not production verification.
