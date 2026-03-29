---
schema: agentcompanies/v1
name: Production Readiness
slug: production-readiness
description: >
  Fix all P0 and P1 bugs from the engineering audit. The app must be
  production-quality before audience building begins. No one downloads
  an app that breaks on first use.
priority: critical
---

# Production Readiness

Ship a version of Found in Translation that works reliably for real travelers.

## Scope

All P0 and P1 bugs from the FOU-1 engineering audit:

### P0 — Broken in Production
1. VAPI decision flow uses in-memory Maps (different Vercel isolates) — migrate to Supabase table
2. Language code mapping broken for TTS ("Spanish" → "sp" not "es") — needs ISO lookup map
3. No VAPI webhook authentication — add signature verification

### P1 — Security
4. Prompt injection via user fields in VAPI system prompt — sanitize inputs
5. No auth on `/api/call` and `/api/vapi/*` routes — add user authentication

### P2 — Code Quality (do after P0/P1)
6. Add `typecheck` and `ci` npm scripts
7. Create `.env.example`
8. Fix silent failures in useVapiCall

## Success Criteria

- Zero P0 bugs
- Zero P1 bugs
- `npm run ci` passes (lint + test + typecheck + build)
- All new fixes have regression tests
