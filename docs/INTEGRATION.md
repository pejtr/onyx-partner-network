# Partner Integration Guide

## 1. Choose an integration level

### Link / affiliate
Use tracked outbound URLs supplied by the partner program. This is the lowest-friction option.

### API
Use a documented partner API for catalog, availability, pricing, lead or conversion flows.

### Webhook
Use signed server-to-server events for conversion or status updates.

### MCP
Use a narrowly scoped MCP server when the partner exposes capabilities that benefit from tool-based orchestration.

## 2. Submit a partner manifest

Start from `examples/partner-manifest.example.json`. The manifest is public metadata only.

Never include:
- API keys or tokens
- signing secrets
- customer data
- private contract terms
- credentials or cookies

## 3. Attribution contract

Each integration should define:
- the source/campaign identifier
- click, lead or order identifier
- conversion status
- currency and value when applicable
- refund/cancellation semantics
- attribution window
- canonical partner/program identifier

Commercial commission terms stay outside the public manifest unless the partner explicitly publishes them.

## 4. Security boundary

Production credentials remain in private secret stores. Public examples use placeholders only. Server-to-server events should be authenticated and replay-resistant.

## 5. Stability

A schema or endpoint is stable only after it has an explicit version. Breaking changes require a new version or a documented migration path.
