# ONYX Partner Network

**Public partner, affiliate and integration gateway for the ONYX / OPTIMATEO ecosystem.**

ONYX Partner Network is the public boundary for companies, affiliate programs, SaaS providers and creators that want to integrate with our distribution network.

> Public here means **integration surface**, not production source code. Core attribution, payment, orchestration, scoring and internal ONYX OS services remain private.

## What partners can use

- Partner onboarding and technical integration documentation
- Versioned partner manifest format
- Affiliate / revenue-share integration patterns
- Webhook and API conventions
- MCP-ready integration guidance
- Public examples that contain no production credentials
- GitHub Issues for partnership and integration requests

## Network model

```text
Traffic / Audience
      ↓
ONYX distribution nodes
      ↓
Partner matching & offer routing
      ↓
Tracked conversion
      ↓
Attribution
      ↓
Partner / network revenue share
```

The commercial terms are agreed per partner or program. This repository does **not** promise a fixed commission rate.

## Partner types

- Travel and accommodation
- SaaS and AI tools
- Creator economy
- E-commerce
- Wellness and education
- Local businesses and venues
- Financially compliant affiliate programs
- APIs, MCP servers and integration providers

## Start here

1. Read [Integration Guide](docs/INTEGRATION.md).
2. Copy [partner-manifest.example.json](examples/partner-manifest.example.json).
3. Validate it against [partner-manifest.schema.json](spec/partner-manifest.schema.json).
4. Open a **Partner application** issue.
5. Never put API keys, secrets, customer data or private contracts in this repository.

## Architecture boundary

### Public

- schemas
- SDK/examples
- documented endpoints
- onboarding
- partner directory metadata
- integration recipes

### Private

- ONYX OS internals
- LeadOS internals
- payment credentials and signing secrets
- commission calculation engine
- fraud/risk scoring
- private partner contracts
- internal MCP capability graph
- customer and conversion data

## Status

The public partner interface is being versioned incrementally. Treat examples as integration contracts only after they are explicitly marked stable.

## Security

See [SECURITY.md](SECURITY.md). If you discover a vulnerability or accidentally expose a credential, do **not** open a public issue containing the sensitive data.

---

Built as the public integration edge of the **ONYX / OPTIMATEO** ecosystem.
