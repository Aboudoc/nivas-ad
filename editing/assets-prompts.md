# The 4 reusable assets — build prompts & specs

Companion file to [capcut-guide.md](capcut-guide.md). Build these once; every
edit reuses them.

## 1. "TVC" subtitle preset (CapCut settings)

- Font: a bold rounded sans that renders Thai cleanly (e.g. **Kanit Bold** or
  CapCut's default Thai bold) · Size ≈ 8–10% of frame height
- Fill: pure white `#FFFFFF` · Stroke: black, thickness ~15% · no shadow box
- Position: bottom-center, baseline at ~22–25% from the bottom (inside TikTok's
  safe zone — clear of the caption/CTA UI)
- Animation: none (hard in/out on the VO timing — TVC style)
- Save as preset named `TVC` in CapCut (right-click the styled text → save preset).

## 2. "Sadvertising" subtitle preset (CapCut settings)

- Font: a light/regular weight of the same Thai family (e.g. **Kanit Light**) ·
  Size ≈ 6–7% of frame height
- Fill: white at ~90% opacity · NO stroke, NO box · very subtle soft shadow
- Position: bottom-center, ~25% from the bottom
- Animation: gentle 0.3 s fade in/out
- Save as preset named `SAD`. Used only on spots 6 and 13.

## 3. End-card template (CapCut project)

Create a 2 s project saved as `endcard-template`, duplicated into every edit:

- 0.0–0.3 s: pure black
- 0.3 s: Nivas Companion logo PNG fades in (0.4 s), centered, ~35% of frame width
- 1.0 s: download QR PNG fades in below the logo, ~18% width
- Tagline text (per spot, TVC preset, smaller size) above the QR
- Audio: silence — except the spot's final sting if the recipe calls for one
- Two variants: 9:16 and 16:9. Keep the logo/QR PNGs in `editing/assets/`
  (create the folder when the final logo files are ready).

## 4. Thai voice-over recording brief (send to the voice artist)

**Brief (Fiverr / voice123, ~30 €):** *"Native Thai voice-over for short social
ads. Conversational Bangkok Thai, natural energy, NOT announcer-style unless
marked. Record each line 3 times (normal / more energy / softer). Deliver dry
WAV, no music, no processing. Please also flag any line that sounds unnatural
and suggest a better phrasing — particles matter (ค่ะ/ครับ/นะ)."*

**Casting — 3 sessions cover everything:**
- **Voice A — female, 25–35** (P'Fon): most lines
- **Voice B — male, 30–45**: Ton variant, interviewer, binder man, young-man
  line (lighter read), + the DEEP horror-trailer read
- **Voice C — female, 50+** (auntie / fortune teller)

**Recording script:**

| Spot | Voice · tone | Line |
|---|---|---|
| 1 c1 | A · comic panic | ห้องนี้… ว่างมั้ยนะ… เดี๋ยวเช็คก่อนนะคะ! |
| 1 c2 | A · calm confident | ห้องว่างสามห้อง ใกล้บีทีเอสอโศก ส่งให้ลูกค้าแล้วค่ะ |
| 1 male | B · comic panic | ห้องนี้… ว่างมั้ยนะ… เดี๋ยวเช็คก่อนนะครับ! |
| 1 end | A · warm tagline | นิวาส คอมแพเนียน — สต็อกห้องของคุณ ครบ จบ ในมือถือ |
| 2 c1 | A · proud, then shocked | ห้องนี้เพิ่งว่างเลยค่ะ! — อ้าว!? |
| 2 c2 | B · DEEP trailer voice | ฝันร้ายที่เอเจนท์ทุกคนต้องเจอ… |
| 2 c3 | A · calm smile | สต็อกอัปเดตเรียลไทม์ค่ะ — ห้องข้างๆ ว่าง สวยกว่าด้วย |
| 5 c1 | A · anxious, respectful | แม่หมอคะ… ห้องไหนจะปล่อยออกคะเดือนนี้? |
| 5 c2 | C · deadpan oracular | สตูดิโอ ใกล้บีทีเอสอ่อนนุช… ลูกค้าทักมาสามคนแล้ว |
| 6 c4 | B · soft, moved (young read) | พี่ฟอนครับ… ผมจะหาห้องแรกของผมครับ |
| 7 c2 | A · deadpan | ห้องนี้… ดูแลตัวเองดีมากค่ะ |
| 7 VO | A · warm narrator | ทุกห้องมีหัวใจ… อย่าปล่อยให้รอนาน |
| 8 c1 | A · live-seller machine-gun | เหลือห้องเดียวค่ะ! พิมพ์หนึ่งในแชทเลย! |
| 8 c2 | A · deflated, then calm | อ้าว… มีคนจองไปแล้วค่ะ — ใช่ค่ะ นี่คือโฆษณา — สต็อกเรียลไทม์ มันเร็วแบบนี้แหละค่ะ |
| 9 c1 | A · deadpan flat | เดือนที่แล้ว ปิดสามสิบดีล… ปกติค่ะ |
| 9 int | B · muffled off-mic | ทำได้ยังไงครับ? |
| 9 c3 | A · deadpan, then to lens | แอปค่ะ. จบ. — ใช่ค่ะ นี่คือโฆษณา |
| 12 A | B · proud | สามสิบห้อง… อยู่ในนี้หมดครับ |
| 12 B | C · warm chuckle | อยู่ในสมุดหมดค่ะ… ถ้าป้าหาเจอนะ |

Note: even for clips where Seedance generated pinned audio, record the real VO
anyway — it is the replacement track whenever a native speaker flags the
generated pronunciation (the ค่ะ→ครับ incident).
