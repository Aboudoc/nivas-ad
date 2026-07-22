# Nivas Global — Master template (8 s luxury film)

- **Usage**: THE modular template for all Nivas Global films. One generation =
  one target nationality. Replace every `{VARIABLE}` (see `nationality-codes.md`),
  or copy a ready-made example from `examples/`.
- **The luxury grammar in 8 s**: one single slow camera move, one single idea,
  golden light, inhabited silence. We don't show the app, we show desire.
- **Model**: Seedance 2.0 (skin / silk / marble rendering)
- **Format**: `{ASPECT}` — 16:9 cinematic or 9:16 paid social · 8 s · continuous shot
- **Post-production (house signature)**: 1.5 s of black at the end, NIVAS logotype
  alone, silence. The logo never appears *inside* the world of the film.

## Variables

| Variable | Values |
|---|---|
| `{ASPECT}` | `16:9` or `9:16` |
| `{CAMERA}` | `dolly-in toward the window` or `lateral glide along the room` |
| `{AGENT_NATIONALITY}` + `{AGENT_OUTFIT}` | see the agents table in `nationality-codes.md` |
| `{CLIENT_COMPOSITION}` | `an elegant {X} couple` / `a distinguished {X} gentleman alone` / `a sophisticated {X} woman alone` |
| `{CLIENT_OUTFIT}` | see the clients table in `nationality-codes.md` |
| `{DOG_CLAUSE}` | `A pristine {BREED} walks beside them, perfectly composed.` — or empty |
| `{ACCENT_COLOR}` | see the clients table |

## Prompt

```
8-second ultra-luxury commercial, single continuous shot, {ASPECT},
slow cinematic {CAMERA}, 35mm anamorphic look, shallow depth of field,
photorealistic skin and fabric texture.

A breathtaking {AGENT_NATIONALITY} female real-estate agent with an haute-couture
supermodel presence, {AGENT_OUTFIT}, walks slowly through a vast Bangkok penthouse —
Italian marble floors, silk curtains breathing in the air-conditioning, floor-to-
ceiling windows revealing the golden Bangkok skyline at sunset.

With one graceful gesture she presents the view to {CLIENT_COMPOSITION}, dressed in
{CLIENT_OUTFIT}. {DOG_CLAUSE} The clients' expression shifts from composure to quiet
awe.

Lighting: warm golden-hour sun flooding the room, soft atmospheric haze, champagne
and amber tones, deep elegant shadows, one accent of {ACCENT_COLOR}.
Grade: high-end French fashion-house film — Chanel / Louis Vuitton commercial
aesthetic, muted quiet-luxury palette, restrained sensuality, effortless wealth.
No text, no logos, no music cues.
```
