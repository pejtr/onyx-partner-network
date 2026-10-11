# Public Repository NO-TRUST Documentation Policy

This repository is public. Treat every committed byte as permanent disclosure.

## Before every documentation/code change

1. Verify repository visibility is still public.
2. Assume attackers, competitors, scrapers and automated models will read the diff.
3. Use placeholders for all environment-specific identifiers.
4. Run secret scanning where available.
5. Review the diff manually before merge.

## Never publish

- secrets, tokens, passwords, recovery codes or cookies,
- private customer/user/partner data,
- connected-account data,
- production database contents,
- internal/private hostnames, IPs or tunnels,
- cloud/account/project/tenant identifiers,
- privileged admin/recovery/bypass procedures,
- private prompts, memory or training examples,
- non-public partner contracts, discounts, margins or commercial terms,
- proprietary fraud/risk/routing scores or thresholds,
- absolute personal filesystem paths,
- signed/temporary media URLs,
- logs or screenshots containing identifiers.

## Public-safe patterns

Prefer:
- `API_BASE_URL`
- `PROJECT_ID`
- `PARTNER_ID`
- `WEBHOOK_SECRET`
- "private backend service"
- "rate limited"
- "managed secret store"

Document public contracts, not exploitable private topology.

## Truth rule

Distinguish intended architecture, implemented code, verified runtime and verified production. Never claim a feature is live solely because it exists in code or CI passed.

## History rule

Deleting a secret later does not remove it from public git history. If sensitive content is ever committed, treat it as exposed and rotate/revoke it.
