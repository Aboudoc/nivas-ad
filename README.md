# Nivas Ad — Video Prompt Library

AI video generation prompts for the two **Nivas** brands, organized by video need.
Goal: be able to generate new content at any time **while keeping the same creative
line and brand image**, without starting from scratch.

Platform: [Higgsfield](https://higgsfield.ai) · generation constraint: **8-second clips max**.

---

## Two brands, two grammars

| | **Nivas Companion** | **Nivas Global** |
|---|---|---|
| Audience | Freelance real-estate agents in Bangkok | International clients (luxury) |
| Tone | Warm, Thai TVC codes (slapstick + deadpan), the agent's daily life (motosai, LINE, BTS, cha yen) | Quiet luxury, Chanel / Louis Vuitton grammar: one slow move, golden light, desire |
| Language | Thai (dialogue + supers) | No dialogue; universal visuals |
| Formats | 16:9 website hero · 9:16 social | 16:9 cinematic · 9:16 paid social |

## Model choice (on Higgsfield, same credit balance)

| Use case | Model | Why |
|---|---|---|
| Shots without dialogue (hero, luxury) | **Seedance 2.0** — default | Most photorealistic (skin, fabric, architecture), 2K, low cost |
| Shots where a character **speaks** | **Kling 3.0** | Best lip-sync on the market (phoneme-level), ~6 credits/clip |
| Iterations, readable on-screen text/UI | Gemini Omni Flash | Conversational editing, but capped ~720p — never for a final shot |
| Big-budget option | Veo 3.1 | Native 48 kHz audio, but 40–70 credits/clip |

## Golden rules (apply to ALL prompts)

1. **Never generate text or logos in-model** — AI mangles text, and Thai script even more.
   Titles, supers, end cards and logos = always added in post-production.
2. **Never generate app UI** — shoot an over-the-shoulder angle with the screen neutral or
   angled away, then composite a real screen recording in post.
3. **Real Thai voice-over in post** (no AI audio for Thai) — Thai audiences instantly detect
   a synthetic voice. Have every line proofread by a native speaker
   (the particles ค่ะ/นะ carry the tone).
4. **3–4 takes per prompt**, keep the best one.
5. **Perfect loop (website hero)**: on Kling, set *first frame = last frame* with the same
   image; on Seedance, the constraint is written into the prompt.
6. **Luxury end card (Global)**: 1.5 s of black, NIVAS logotype alone, silence. The logo
   never appears *inside* the world of the film.

## Repository layout

```
companion/
  hero-site/            Homepage background video — 16:9, fixed shot, 8 s, loop, muted
    pro-bts-chong-nonsi.md      PRO version: the BTS S-curve at Chong Nonsi + MahaNakhon
    aerial-skyline-loop.md      Variant: aerial skyline, clouds only — loop-friendliest
    wat-arun-sunset-loop.md     Variant: Wat Arun pastel sunset, matches the Global hero still
    humour-tvc-condo.md         HUMOUR version: slapstick/deadpan inside a single frame
    humour-sticky-notes.md      HUMOUR version 2: sticky-note storm + deadpan look to camera
  social-agents/        9:16 spot for Facebook/TikTok/Reels targeting BKK freelance agents
    clip1-chaos-motosai.md      Spot 1 (day-in-the-life), 3×8 s: the chaos
    clip2-twist-lobby.md        … the twist
    clip3-payoff-key-handover.md … the payoff + end card
    montage-8s-standalone.md    Single 8 s clip variant (editing recipe)
    spot2-clip1-double-booking.md Spot 2 (horror parody), 3×8 s: the double booking
    spot2-clip2-horror-parody.md  … the Thai ghost-film swerve
    spot2-clip3-realtime-save.md  … saved by real-time stock + end card
    spot3-aura-walk.md            Spot 3 (single 8 s): sexy-funny perfume-ad parody
    spot4-lakorn-almost-kiss.md   Spot 4 (single 8 s): lakorn soap-opera almost-kiss parody
  site-widgets/         Small looping videos embedded in the website UI
    line-contact-circle.md        Round LINE chat bubble presenter (looping video)
  site-images/          STILL-image prompts (not video) for website illustration
    pfon-image-pack.md            8 P'Fon presenter poses (cutout-ready) mapped to site sections
global/
  template-master.md    THE modular luxury template ({AGENT_NATIONALITY}, {CLIENT_…}, {DOG_CLAUSE}…)
  nationality-codes.md  Per-nationality codes table: outfits, dog, accent color
  examples/             Filled-in templates, ready to copy-paste
    chinese-couple-thai-agent.md
    russian-solo-russian-agent.md
    japanese-solo-french-agent.md
```

## Typical workflow

1. Pick the prompt file matching the need (or fill in `global/template-master.md`).
2. Generate 3–4 takes on Higgsfield with the model listed at the top of the file.
3. Post-production: real Thai VO · supers/end card · UI compositing · logo.
4. Export: website hero = compressed muted mp4/webm autoplay-loop; social = 9:16 with
   burned-in Thai subtitles (sound is often off on mobile).

## Extending the library (keeping the line)

- **New Companion prompt**: reuse the "Thai TVC" grade (punchy natural light, warm skin
  tones, saturated greens, slight film grain) and the agent daily-life codes
  (orange motosai vest, LINE, BTS, spiral notebook, cha yen). One file = one 8 s shot.
- **New Global nationality**: add a row in `nationality-codes.md`
  (aspirational — never caricatural — outfit, dog breed, accent color),
  then create the filled-in example in `examples/`.
- File naming: `kebab-case`, describing the content of the shot.

## Roadmap

- `companion/features/` — 8 s snippets per feature (bulk import, calendar) with
  UI composited in post.
