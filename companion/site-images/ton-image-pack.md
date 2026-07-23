# Site images — the Ton presenter pack (STILL IMAGES, not video)

- **⚠️ These prompts generate IMAGES, not video** — use an image model
  (Grok Imagine / Higgsfield image mode), high resolution, portrait 2:3 unless noted.
- **⚠️ Character consistency**: Ton is the SAME man as the website-hero HUMOUR
  video and the male LINE widget (`line-contact-circle-male.md`) — the calm
  cha-yen agent. **Attach 2–3 clean face reference frames with every generation.**
  Same wardrobe in every image (smart casual shirt, light navy blazer over a plain
  tee) = recognizable brand presenter.
- **His register vs P'Fon**: she is warm-welcoming, he is deadpan-cool — small
  gestures, slight smirk, effortless confidence. Use whichever fits the page tone;
  the pose set mirrors `pfon-image-pack.md` so they are interchangeable.
- **Cutout rule**: clean gradient background + crisp edges → easy background
  removal; the pose leaves space on one side for text. Never any text/logo in the
  image; phone screens stay BLANK (real app UI composited later).

## Master prompt (fill {POSE})

```
STILL IMAGE, high-resolution photorealistic commercial photography, portrait 2:3.
CHARACTER REFERENCE: use the attached photos — the same young Thai man in every
image.

A calm, stylish young Thai man around 30, smart casual shirt with a light navy
blazer over a plain tee, effortless deadpan-cool confidence with a slight smirk,
studio shot against a clean soft light-blue-to-white gradient background, bright
even commercial lighting, no harsh shadows, three-quarter body framing, sharp
focus, crisp clean edges suitable for background removal and cutout use.

POSE: {POSE}

Composition leaves clear empty space on one side for a headline. No text, no
logos, no watermark. If a phone is in frame, its screen is plain dark and blank.
```

## The 9 poses and where each one is used on the site

| # | `{POSE}` | Site usage |
|---|---|---|
| 1 | `He holds a smartphone up beside his face, blank screen facing the camera, tapping it once with a knowing smirk.` | Hero banner + app-download section (composite the real app UI) |
| 2 | `He points to his left toward empty space with two fingers, one eyebrow raised, effortlessly inviting.` | Banners — headline/CTA sits where he points |
| 3 | `He gives a relaxed thumbs-up at chest height, small confident smile.` | Promo cards, pricing, testimonials |
| 4 | `He wears a slim call-center headset, leaning slightly forward, mid-friendly-conversation smile.` | Support / LINE admin-chat card |
| 5 | `He greets with a polite Thai wai, slight bow, calm warm smile.` | Welcome / onboarding / sign-up section |
| 6 | `He presents an invisible announcement beside him with one open palm, eyebrows raised, small grin.` | Flash promos, launch announcements |
| 7 | `He stands with hands in pockets, relaxed confident smile, slight head tilt.` | About / trust / "why Nivas" section |
| 8 | `He holds a set of condo keys out toward the camera with one hand and a proud smirk.` | Success stories / conversion section |
| 9 | `He casually sips bright-orange Thai iced tea from a plastic cup with a straw, eyes to camera, tiny knowing smile.` | His signature — lifestyle sections, blog, social avatars |

## Workflow

1. Generate pose 1 first, 3–4 variations; lock the best as the OUTFIT + look
   reference (add it to the reference photos for all other poses).
2. Generate the remaining poses with face refs + outfit ref attached.
3. Background-removal pass → export transparent PNGs (site) + originals (archive).
4. Composite the real app UI into pose 1's blank screen.
