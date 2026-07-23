# Site images — the P'Fon presenter pack (STILL IMAGES, not video)

- **⚠️ These prompts generate IMAGES, not video** — use an image model
  (Grok Imagine / Higgsfield image mode), high resolution, portrait 2:3 unless noted.
- **⚠️ Character consistency**: P'Fon must be the SAME Thai woman as the humour
  spots and the LINE widget. **Attach 2–3 clean face reference frames with every
  generation** — the text alone will not reproduce her. Same wardrobe in every
  image (light blazer over a white top) = recognizable brand presenter.
- **Why this pack**: successful Thai real-estate sites are built on
  presenter cutouts — a person holding the app, pointing at headlines, thumbs-up
  on promo cards, headset on the support widget. One consistent presenter across
  all surfaces = instant brand recognition.
- **Cutout rule**: clean gradient background + crisp edges → easy background
  removal; the pose leaves space on one side for text. Never any text/logo in the
  image; phone screens stay BLANK (real app UI composited later).

## Master prompt (fill {POSE})

```
STILL IMAGE, high-resolution photorealistic commercial photography, portrait 2:3.
CHARACTER REFERENCE: use the attached photos — the same Thai woman in every image.

A friendly Thai woman around 30, light blazer over a white top, warm approachable
smile, studio shot against a clean soft light-blue-to-white gradient background,
bright even commercial lighting, no harsh shadows, three-quarter body framing,
sharp focus, crisp clean edges suitable for background removal and cutout use.

POSE: {POSE}

Composition leaves clear empty space on one side for a headline. No text, no
logos, no watermark. If a phone is in frame, its screen is plain dark and blank.
```

## The 8 poses and where each one is used on the site

| # | `{POSE}` | Site usage |
|---|---|---|
| 1 | `She holds a smartphone up beside her face, blank screen facing the camera, her other hand pointing at it with a delighted smile.` | Hero banner + app-download section (composite the real app UI on the screen) |
| 2 | `She points to her left toward empty space with an open palm, eyebrows raised, inviting.` | Banners — headline/CTA sits where she points |
| 3 | `She gives a big confident thumbs-up toward camera, grinning.` | Promo cards, pricing, testimonials |
| 4 | `She wears a slim call-center headset, one hand touching the earpiece, mid-friendly-conversation smile.` | Support / LINE admin-chat card |
| 5 | `She greets with a graceful Thai wai, slight bow, warm welcoming smile.` | Welcome / onboarding / sign-up section |
| 6 | `She looks wide-eyed and excited, both hands framing an invisible announcement beside her.` | Flash promos, launch announcements |
| 7 | `She stands arms crossed, relaxed confident smile, slight head tilt.` | About / trust / "why Nivas" section |
| 8 | `She holds a set of condo keys out toward the camera with both hands and a proud smile.` | Success stories / conversion section |

## Workflow

1. Generate pose 1 first, 3–4 variations; lock the best as the OUTFIT + look
   reference (add it to the reference photos for all other poses).
2. Generate the remaining poses with face refs + outfit ref attached.
3. Background-removal pass → export transparent PNGs (site) + originals (archive).
4. Composite the real app UI into pose 1's blank screen.
