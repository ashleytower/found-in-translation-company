# Found in Translation — Paperclip Company

AI-powered on-the-ground travel companion. This Paperclip company package manages the autonomous team building and growing the app.

## Workflow

**Hub-and-spoke with autonomous CEO.** The CEO wakes hourly, assesses company state, delegates work to three specialists, identifies capability gaps, and proposes new hires to the board. Specialists wake on demand when assigned work.

## Org Chart

| Agent | Role | Model | Heartbeat | Icon | Reports To |
|-------|------|-------|-----------|------|------------|
| CEO | Chief Executive Officer | Sonnet | Hourly + on-demand | crown | Board (Ashley) |
| Engineering Lead | Full-stack developer | **Opus** | On-demand | code | CEO |
| UI/UX Designer | UX auditor & spec writer | Sonnet | On-demand | eye | CEO |
| Content Strategist | TikTok/IG content + Content Blitz Engine | Sonnet | On-demand | sparkles | CEO |

## Projects

| Project | Priority | Description |
|---------|----------|-------------|
| Production Readiness | Critical | Fix P0/P1 bugs from engineering audit |
| UX Polish | High | Audit and polish every screen to production quality |
| Audience Warmup | High | Build TikTok/IG audience using the Japan family story |

## Tech Stack

Next.js 14, TypeScript, Supabase, Gemini 2.5 Flash, Deepgram STT, Cartesia TTS, VAPI, Google Maps, Stripe. Deployed on Vercel.

## Getting Started

```bash
# Ensure Paperclip is running
npx paperclipai run

# Import this company
npx paperclipai company import ~/Documents/paperclip-companies/found-in-translation

# Open the dashboard
open http://127.0.0.1:3100
```

## Company Rules

1. All agents use Context7 for library documentation (never rely on training data)
2. All agents use the `paperclip` skill for Paperclip API interactions
3. All agents use autoresearch principles (verify, don't guess)
4. CEO proposes new hires with board approval required
5. No generic output — everything specific to this app, this story, this user base
