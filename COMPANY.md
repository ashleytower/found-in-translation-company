---
schema: agentcompanies/v1
name: Found in Translation
slug: found-in-translation
version: 1.0.0
website: https://foundintranslation.app
repo: https://github.com/ashleytower/found-in-translation
mission: >
  Be the world's best on-the-ground travel companion. Help the 2 billion
  annual international travelers translate, call, navigate, price-check,
  and understand in real-time in any country — regardless of language
  barriers. Build to 10,000 active users with Travel Memory Pass converting.
goals:
  - Ship a production-quality PWA that travelers trust with real money
  - Build a warm audience on TikTok and Instagram using the real Japan family story
  - Reach 10,000 active users
  - Convert free users to Travel Memory Pass (paid tier)
requirements:
  secrets:
    - NEXT_PUBLIC_GOOGLE_API_KEY
    - NEXT_PUBLIC_DEEPGRAM_API_KEY
    - NEXT_PUBLIC_CARTESIA_API_KEY
    - VAPI_API_KEY
    - NEXT_PUBLIC_SUPABASE_URL
    - NEXT_PUBLIC_SUPABASE_ANON_KEY
    - STRIPE_SECRET_KEY
---

# Found in Translation

An AI-powered on-the-ground travel companion. Unlike every other travel app, it works *while you're there* — not before. It solves the real problems that happen the moment you land: you can't read the menu, you can't call the restaurant, you don't know if that price is a rip-off, and your friend isn't around to ask.

## What We Do

- **Voice Translation** — Tap the orb, speak, get instant bidirectional translation with natural voice output (Deepgram STT → Gemini → Cartesia TTS)
- **Camera Translation** — Point at signs, menus, products — instant OCR + translation via Gemini Vision
- **AI Phone Calls** — AI calls the restaurant, hotel, or taxi in the local language on your behalf via VAPI
- **Price Check** — Take a photo of a price tag, converts it to your home currency, and checks if the same product is cheaper at home
- **Currency Conversion** — "How much is this at home?" answered instantly with live rates
- **Dish Identification** — Point at food, know what it is, what's in it, and whether you can eat it (dietary/allergy aware)
- **Explore** — Nearby restaurants, pharmacies, transit — filtered by your preferences, in the local language
- **Travel Memory** — Geo-tagged timeline of your trip, preferences learned over time

## The Real Story

The founder's 11-year-old daughter was in Japan using the app and gave it a thumbs up when it worked. Real family. Real trip. Real problem solved. That is the product demo. That is the TikTok.

## Tech Stack

Next.js 14 (App Router) + TypeScript, Supabase (Auth + DB + Storage + Edge Functions), Gemini 2.5 Flash, Deepgram WebSocket STT, Cartesia WebSocket TTS, VAPI AI phone agent, Google Maps Platform, Stripe subscriptions. Deployed on Vercel.

## Company Rules

1. **Every agent must use Context7** to fetch current library documentation before writing code or making API calls. Never rely on training data for framework/SDK questions.
2. **Every agent must use the `paperclip` skill** for all Paperclip API interactions — heartbeats, issues, comments, checkout.
3. **Every agent must use `autoresearch` principles** — modify, verify, keep/discard, repeat. No guessing. No hallucinating.
4. **CEO proposes new hires with justification.** Board (Ashley) approves or rejects.
5. **No generic output.** Every piece of work must be specific to this app, this tech stack, this story, this user base.
