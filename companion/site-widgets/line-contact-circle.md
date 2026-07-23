# Site widget — the LINE contact circle (LivingInsider style)

- **Usage**: small looping video inside the round LINE contact bubble on the website
  (like LivingInsider's): a friendly presenter waves, points at the chat button,
  thumbs-up, loops. Invites visitors to tap and chat on LINE.
- **⚠️ Character consistency**: the presenter MUST be **P'Fon — the same Thai woman
  as the humour spots** (spot 1 motosai, spot 2 double-booking, hero sticky-notes).
  When generating, **attach 2–3 clean reference frames of her face** (exported from
  the chosen takes of the previous videos) as image inputs alongside the prompt —
  the text prompt alone will NOT reproduce the same person. For a male variant,
  swap the subject line for: `A friendly Thai man around 30 in a smart navy blazer
  over a plain t-shirt`.
- **Model**: Seedance 2.0 (accepts reference images) · **Format**: 1:1 square if
  available (else 9:16, subject centered chest-up) · 8 s · fixed camera · loop
- **Two prompts below**: A = generate the video · B = paste into Claude Code to
  implement the widget on the site.

## Prompt A — video generation

```
Square 1:1 aspect, single continuous 8-second shot, fixed camera, photorealistic,
bright clean commercial studio look. CHARACTER REFERENCE: use the attached photos —
the presenter must be the same Thai woman as in the reference images.

A friendly Thai woman around 30, light blazer, warm approachable energy, stands
against a soft light-blue-to-white gradient studio background, framed chest-up and
perfectly centered for a circular crop. She looks straight at camera with a warm
smile, gives a small welcoming wave, then points down toward the lower center of
the frame (where a chat button will be overlaid) and nods encouragingly, finishes
with a friendly thumbs-up and returns to the exact same neutral smiling pose as the
start. Soft even lighting, no harsh shadows, gentle motion only.

Loop-friendly: first and last frame nearly identical neutral smiling pose. Keep the
lower center of the frame clear of hands at start and end for a button overlay.
No text, no logos.
```

## Prompt B — site implementation (paste into Claude Code)

```
Add a floating LINE contact widget to the site, styled like LivingInsider's,
following the project's existing stack and conventions.

- Fixed position bottom-right (24px offsets, safe-area aware), above all content.
- A 96px circular bubble (72px on mobile) containing a looping video
  (assets/line-circle.mp4): autoplay, muted, loop, playsinline, poster fallback
  image, object-fit: cover, circular crop (border-radius: 50%), and a thin
  teal-to-green gradient ring around the circle.
- A green pill overlaid on the bottom edge of the circle, slightly overlapping it:
  the OFFICIAL LINE icon asset (provided — do not redraw it) + the Thai text
  "ปรึกษาฟรี", white text on LINE green #06C755, rounded-full.
- The whole widget is a single link to LINE_URL (const at the top of the component:
  "https://line.me/R/ti/p/@REPLACE_ME"), opening in a new tab with rel="noopener".
- Subtle attention pulse (gentle scale) every ~8 s; under prefers-reduced-motion,
  disable the pulse AND swap the video for the poster image.
- Lazy-load the video (don't fetch it before the widget is near the viewport).
- Accessibility: the link has aria-label "Chat with us on LINE / แชทกับเราทางไลน์",
  is keyboard-focusable with a visible focus ring.
- A small × dismiss button hides the widget for the session (sessionStorage).
```

## Integration notes

- The green LINE pill is an HTML overlay, never generated in the video. The LINE
  logo must be the official brand asset (LINE brand guidelines).
- Export the video compressed (mp4 + webm), a few hundred KB max — it loops forever
  on every page.
