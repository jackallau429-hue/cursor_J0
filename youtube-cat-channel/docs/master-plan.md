# Master Plan — The Daily Meowsletter (v3.0)

> Living document. Edit as plan evolves.

---

## 1. Concept

A semi-automated YouTube channel where a real orange tabby cat plays a deadpan
news anchor, "reacting" to trending world news. AI-generated voiceover (reporter
narration) + cat footage (50% real / 50% AI) + sarcastic on-screen subtitles.

**Tagline:** *"Today's news, judged by a cat."*

**Why orange cat:** Universal "orange cat brain cell" meme — strong visual
identity, dramatic facial expressions, easy adult-cat filming, massive existing
audience pool (e.g., `@whatsupbeanie`, `@oranganator`).

---

## 2. Channel Identity

| Field | Value |
|---|---|
| **Channel name** | _PENDING — see `pending-decisions.md`_ |
| **Anchor cat name** | _PENDING_ |
| **Primary language** | English (highest RPM, widest audience, AI-friendly) |
| **Secondary** | Universal cat sounds — no translation needed |
| **Visual style** | Orange (#FF8C42) + Navy (#1B3A5C) + cream; news-broadcast layout |
| **Anchor persona** | Lazy, cynical, "wake me when it matters", tilted bow tie |

---

## 3. Income Model

| Source | When | Estimated share |
|---|---|---|
| YouTube AdSense (long-form 6–12 min) | After 1k subs + 4k watch hours | 60–70% |
| YouTube Shorts ad-share | Same threshold | 10–20% |
| Affiliate links (AI tools, cat products) | After 5k subs | 15–25% |
| Channel memberships / merch | Optional, post-10k subs | 5–10% |

**Path to $1,000/month (English, RPM ~$8):** 100k–150k monthly views.

**Realistic timeline:** Monetization at month 3, $1,000/month at month 6–9.

---

## 4. Content Pillars

| Pillar | Share | RPM | Format |
|---|---|---|---|
| World news hot takes (international) | 40% | $4–8 | Sarcastic reaction |
| Tech & AI news | 30% | $6–12 | Explainer + jab |
| Bizarre / weird news | 20% | $3–6 | Pure entertainment |
| Money / crypto | 10% | $8–15 | Skeptical commentary |

**Avoid:** politics, religion, race/nationality, celebrity gossip with copyright
risk.

---

## 5. Output Cadence

| Format | Length | Frequency | Best post time (UTC+8) |
|---|---|---|---|
| Shorts | 30–50s | Daily × 1 | 21:30 |
| Weekly long-form recap | 6–8 min | Sunday × 1 | 20:00 |
| Bi-weekly deep-dive | 8–12 min | Saturday × 1 (alt weeks) | 20:00 |

---

## 6. Tool Stack

### Paid (your subscriptions)

| Tool | Cost | Replaces |
|---|---|---|
| **Cursor Pro** | US$20/mo | Claude Pro, ChatGPT Plus, automation scripting |

### Free (external — required)

| Tool | Use | Notes |
|---|---|---|
| Bing Image Creator | Thumbnails, cat expressions | DALL-E 3 free |
| Leonardo.ai | Backup image gen | 150 free credits/day |
| Hailuo AI / Kling | AI cat video clips | Free tier |
| Microsoft Edge TTS | Reporter voiceover | Free, multilingual |
| Azure Speech (optional) | Higher-quality TTS | 500k chars/mo free |
| CapCut (PC + mobile) | Editing | Free |
| Pixabay / Freesound | Cat sounds, BGM | CC0 |
| Canva (free) | Thumbnails, banner | Upgrade later |
| Google Trends | Topic research | Free |
| VidIQ free | YouTube SEO | Free tier |

### Cursor model assignment

| Model | Used for |
|---|---|
| Claude Opus 4.7 | Creative scripts, punchlines |
| Claude Sonnet 4.6 | Daily SOP (scripts, SEO) — daily driver |
| GPT-5.3 Codex | Python automation scripts |
| Gemini 3.1 Pro | Long-context news triage |
| GPT-5.5 | English native-pass refinement |
| Composer 2 | Quick edits |

---

## 7. Daily Workflow (target ≤25 min after automation)

```
[Cursor: trends script]   →  daily_trends.py outputs ranked headlines
        ↓
[Cursor: Claude]          →  writes 45-second Shorts script
        ↓
[Hailuo / phone]          →  generate / film 5–6 cat clips (5s each)
        ↓
[Edge TTS]                →  reporter voiceover
        ↓
[CapCut master template]  →  drag clips + voice + auto-subtitle + tweak
        ↓
[Cursor: SEO writer]      →  title / description / tags
        ↓
[Bing Image Creator]      →  thumbnail (using prompt template)
        ↓
[YouTube Studio]          →  schedule upload (21:30 UTC+8)
```

Sunday adds a 6–8 min recap = ~2 extra hours.

---

## 8. Automation Roadmap (Cursor scripts)

| Priority | Script | Saves |
|---|---|---|
| P0 | `daily_trends.py` — fetch Google Trends + Reddit, rank by virality | 5 min/day |
| P0 | `news_to_script.py` — batch-convert 10 headlines → Claude scripts | 30 min/week |
| P1 | `prompt_factory.py` — generate 50 cat-video prompts in batch | One-time 2h |
| P1 | `seo_writer.py` — title/desc/tags formatter | 3 min/day |
| P2 | `youtube_uploader.py` — YouTube Data API auto-schedule | 2 min/day |
| P2 | `analytics_tracker.py` — read YT Analytics, surface patterns | 3 h/month |
| P3 | `competitor_radar.py` — monitor top 10 similar channels | 1 h/week |

---

## 9. Copyright / Compliance Rules

- ✅ Own cat footage + AI-generated cats + CC0 stock only
- ✅ News content = headlines + paraphrase only (no clip reuse > 5s)
- ✅ AI / self-recorded voiceover only
- ✅ YouTube Audio Library or Pixabay BGM only
- ❌ No re-uploading other creators' cat clips
- ❌ No politically / religiously divisive topics
- ❌ No copyrighted news b-roll

---

## 10. Risks & Mitigations

| Risk | Mitigation |
|---|---|
| YouTube AI-slop crackdown | Human review every script; ≥40% real cat footage |
| Adult-cat = boring assumption | False — proven by `@whatsupbeanie`, `@thatlittlepuff` |
| Content fatigue | Rotate 4 pillars; A/B test thumbnails weekly |
| Account strike | Stay in safe topics; avoid copyrighted news visuals |
| Burnout | Automation first; aim ≤25 min/day after month 2 |

---

## 11. Realistic Growth Forecast

| Month | Subs | Monthly views | Est. revenue (USD) |
|---|---|---|---|
| 1 | 50–200 | 1k–5k | $0 (below threshold) |
| 3 | 1,000–2,000 | 30k–60k | $50–200 (just monetized) |
| 6 | 5,000–8,000 | 150k–250k | $800–1,500 |
| 9 | 12,000–20,000 | 400k–600k | $2,000–4,000 |
| 12 | 25,000–40,000 | 700k–1.2M | $4,000–8,000 |

Assumes English, RPM ~$8, 5 Shorts + 1 long-form per week, consistent A/B testing.
