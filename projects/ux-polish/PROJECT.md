---
schema: agentcompanies/v1
name: UX Polish
slug: ux-polish
description: >
  Audit and polish every screen to production quality. Focus on the
  Translator (voice orb) and Camera views first — these are the core
  experience. A traveler under stress must succeed on first try.
priority: high
---

# UX Polish

Audit every view and bring the UX to production quality.

## Scope

1. **Translator view (voice orb)** — Primary interaction. Audit: touch targets, state feedback (idle/listening/speaking/processing), language switching, bidirectional flow ("their turn"), error states.
2. **Camera view** — Point and translate. Audit: camera permissions flow, capture UX, translation overlay, loading states.
3. **Bottom navigation** — Tab switching, active states, badge indicators.
4. **Onboarding** — First-run experience. Profile setup (language, home city, phone). Must complete in under 60 seconds.
5. **All other views** — Currency, Explore, Phrases, Memory, Settings, Calls.

## Deliverables

Per screen:
- Priority-ordered list of UX issues (critical / nice-to-have)
- Proposed fix for each issue (specific enough for Engineering Lead to implement)
- Missing states identified (loading, empty, error, offline)

## Success Criteria

- Every screen has all states handled
- Primary actions are one-thumb, one-tap
- No dead ends in any flow
- Onboarding completes in under 60 seconds
