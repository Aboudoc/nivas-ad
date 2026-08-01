# Editing guide — CapCut desktop (free)

CapCut desktop (free tier) is the tool for all spot edits: Thai auto-captions,
PNG overlays (fake UI, supers), speed curves, SFX library, 9:16/4K export, and a
direct pipeline to TikTok. Everything below uses free features (a few LUTs and
effects are Pro-gated — all workaroundable). Always keep BOTH the clean master
and the subtitled version of every edit.

## The 4 reusable assets (build once, before any edit)

1. **"TVC" subtitle preset** — bold white, black stroke, bottom 25% of frame
   (safe zone). Used on all comedy spots.
2. **"Sadvertising" subtitle preset** — thin white, no stroke, minimal. Used on
   spots 6 and 13.
3. **End-card template project** — black background + Nivas logo PNG + download
   QR, 1–2 s, gentle fade. Duplicated at the end of every edit.
4. **Recorded Thai voice-overs** — all VO lines from the spot files, recorded by
   a native speaker, imported before editing starts.

## Golden rules

- **Sound-swap exports**: spots designed for trending sounds (10 CCTV, 11 GRWM)
  are exported WITHOUT music — the trending sound is added inside the TikTok app
  to ride the trend.
- Hard cuts only (Thai TVC style) — the ONLY exception is soft cross-dissolves
  on the sadvertising spots (6, 13).
- Auto-captions: run on the imported VO track ("Auto captions" → Thai), then
  apply the preset. Verify Thai rendering manually.
- Export: 1080×1920 H.264 high bitrate for 9:16; 4K masters for spots 13–17.
  TikTok recompresses anyway — keep the masters.

## Per-spot editing table

| # | Spot | Structure | CapCut editing recipe |
|---|---|---|---|
| 1 | Day-in-the-life (P'Fon) | 3×8 s + male scooter variant (Ton) | Hard cuts; Thai VO then auto-captions with TVC preset; pop SFX on cut 1→2; QR end card |
| 1b | Standalone 8 s | edit recipe | Clip 1 cut at 5 s → real app screen recording (2 s) → 1 s end card; "pop" SFX on the cut |
| 2 | Horror double-booking | 3×8 s | Clip 2: green-teal LUT + vignette + grain + thunder; scratch-stop on the reveal; crash-zoom via scale keyframes at end of clip 1 |
| 3 | Aura walk | 1×8 s | Perfume orchestral → vinyl scratch on the fan reveal → resume; final super |
| 4 | Lakorn almost-kiss | 1×8 s | Strings cut DEAD on the phone buzz + one dry "ping" + ukulele sting; super on the frozen pucker |
| 5 | Fortune teller (mutelu) | 2×8 s | Mystical drone + temple bell; scratch-stop on the phone pull; super «แม่หมอยังใช้เลย» |
| 6 | Unsung agent | 4×8 s | Piano; soft cross-dissolves (the exception); «10 ปีต่อมา» on 1 s of black between clips 2–3; minimal captions; end in silence |
| 7 | Lonely room | 3×8 s (clip 3 = 3a 5 s + 3b 3 s) | Clip 1 desaturated, clips 2–3 punchy; warm VO; 3a→3b cut; end card |
| 8 | Live commerce | 2×8 s | Generic live-UI overlay: looping "1"-spam chat PNGs, heart stickers, animated viewer-counter text + grain + ring-light vignette; scratch on the freeze |
| 9 | Mockumentary | 3×8 s | Lower-third «พี่ฟอน — เอเจนท์อิสระ»; interviewer question as text + muffled voice; zoom punch-ins via keyframes if not in-gen |
| 10 | CCTV | 1×8 s | Slight desaturation + noise/scanline effect; timestamp + "CAM 04" mono font in corner; speed curve 1.2–1.5×; **export without music** → trending sound in TikTok |
| 11 | GRWM | 1×8 s | Beat-synced micro-zooms (keyframes) on each prop; keep «พร้อมค่ะ»; **export without music** (trending sound) |
| 12 | Vox-pop | 3×8 s | Question text top-of-frame on every clip; hard cuts A→B→C; paper-flutter SFX (B); beat of silence on C; invite stitches in the caption |
| 13 | First deal (4K) | 2×8 s | Piano; discreet supers; fade to black at the end; **4K export**; zero grain |
| 14 | Cha yen luxury (4K) | 1×8 s | Perfume orchestral; super on the sip; 4K export |
| 15 | Elevator mode (4K 16:9) | 1×8 s | Sultry track cut DEAD on the light blink + elevator "ding" + silence; supers «โหมดตัวเอง/โหมดลูกค้า»; derive 9:16 via keyframed crop |
| 16 | Rooftop pool (4K 16:9) | 1×8 s | Sunset R&B; super «ขายวิว… แต่ขอลองก่อนนะคะ» on the final look; 9:16 derivative |
| 17 | Into the rain (4K 16:9) | 1×8 s | Music swells ON the step into the rain (not after); two-beat supers; end card |

## Non-spot exports

- **LINE widgets**: no edit — circular crop happens in CSS on the site; just
  compress (a few hundred KB) + export a poster frame.
- **Website heroes**: export muted loops, mp4 + webm, ~1–2 MB target.
