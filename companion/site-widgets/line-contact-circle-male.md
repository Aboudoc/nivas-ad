# Site widget — the LINE contact circle, male variant ("Ton")

- **Usage**: same round LINE contact bubble as `line-contact-circle.md`, but with
  the male presenter: **the calm, stylish young Thai agent from the website hero
  HUMOUR version** (the one sipping Thai iced tea in the shade with the tiny
  knowing smile). Codename in this repo: **"Ton"**.
- **⚠️ Character consistency**: Ton must be the SAME man as in the hero HUMOUR
  video (and the rival-agent scenes reuse the sweaty archetype — NOT him). **Attach
  2–3 clean face reference frames of him with every generation** — screenshots
  exported from the chosen hero take. The text prompt alone will not reproduce him.
- **His register** (vs P'Fon's warm energy): deadpan-cool — small gestures, slight
  smirk, effortless. The cha yen cameo is his signature.
- **Model**: Seedance 2.0 (accepts reference images) · **Format**: 1:1 square if
  available (else 9:16, subject centered chest-up) · 8 s · fixed camera · loop
- **Implementation**: use **Prompt B** and the pre-paste checklist from
  `line-contact-circle.md` — identical widget, just point it at this video file
  (e.g. `assets/line-circle-male.mp4`).

## Prompt A — video generation

```
Square 1:1 aspect, single continuous 8-second shot, fixed camera, photorealistic,
bright clean commercial studio look. CHARACTER REFERENCE: use the attached photos —
the presenter must be the same young Thai man as in the reference images.

A calm, stylish young Thai man around 30, smart casual shirt, effortless
deadpan-cool energy, stands against a soft light-blue-to-white gradient studio
background, framed chest-up and perfectly centered for a circular crop. He takes
one relaxed sip of bright-orange Thai iced tea from a plastic cup, gives the camera
a tiny knowing smile, points down toward the lower center of the frame (where a
chat button will be overlaid) with two fingers, ends with a small confident nod and
returns to the exact same relaxed pose as the start, cup lowered out of the bottom
area. Soft even lighting, no harsh shadows, minimal smooth motion only.

Loop-friendly: first and last frame nearly identical relaxed pose. Keep the lower
center of the frame clear of hands and cup at start and end for a button overlay.
No text, no logos.
```
