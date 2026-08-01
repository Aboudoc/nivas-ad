# Creative Producer brief — Nivas motion-design pipeline

**Paste-this-to-start**: in a Claude session with the **Higgsfield MCP connector**
active, open this repo and say: *"Read pipeline/creative-producer-brief.md and
execute Mission 1 with the motion-design skill."*

## Role & toolchain

You are the **Creative Producer** for Nivas Companion's ad content. Toolchain:
Claude (Fable 5) + the Higgsfield MCP connector + the repo-local skill at
`.claude/skills/motion-design/SKILL.md` (classicMD/highMD flow: brief → single
storyboard sheet → Seedance 2.0 video). This repo is the brand memory — read
before creating:

- `README.md` — the two brand grammars + the 7 golden rules
- `companion/social-agents/real-thai-style.md` — hard-won generation lessons
- `editing/capcut-guide.md` + `editing/assets-prompts.md` — post pipeline

## Non-negotiable rules (learned the hard way, they override the skill)

1. **Logos and app UI are NEVER generated** — always `media_upload` the real
   logo PNG / real app screenshots and animate around them. A generated logo or
   screen is garbage by definition.
2. **No generated Thai text** — models mangle Thai script; supers/taglines are
   burned in post (CapCut), not in-gen. Storyboard frame captions (English, 2–4
   words) are allowed on the storyboard sheet only, never in the final video.
3. Check `mcp__higgsfield__balance` BEFORE any run; announce the cost plan.
4. Companion identity = vibrant Thai-market (tropical teal + warm accents,
   emoji-forward energy); Nivas Global = quiet luxury. Never mix the two.
5. Outputs go to `outputs/` (gitignored) — report job IDs + files back.

## Mission 1 — the Nivas end-sting ("jingle")

A motion-design logo sting that closes EVERY spot (it upgrades the static
end-card template in `editing/capcut-guide.md`).

- **Flow**: classicMD · **Duration**: 5 s · **Formats**: master 9:16 AND a 16:9
  version (two runs)
- **Asset**: the official Nivas Companion logo PNG (uploaded — see rule 1)
- **Mood**: vibrant tropical premium — deep teal base, warm amber/coral accents,
  soft light sweeps; energetic but clean (this closes comedy AND emotional
  spots, so no gag, no aggression)
- **Ending**: static logo lock, final ~1 s dead stable (it must freeze-frame
  cleanly for CapCut)
- **Sound**: none in-gen; the sonic signature is added in post
- **Storyboard**: 6 frames (light sweep in → logo assembles from tropical
  particles/ribbons → lock → hold)

## Mission 2 — the classic app-feature ad

The straightforward "what the app does" promo — the counterpart to the story
spots.

- **Flow**: classicMD · **Duration**: 15 s · **Format**: 9:16
- **Assets**: real app screenshots uploaded via `media_upload` (Home hero, the
  stock list, bulk import, calendar) — the motion animates AROUND these real
  screens (pans, parallax, floating device frames); it never redraws them
- **Storyboard**: 8 frames — hook (a chaotic paper/sticky-note swirl calming
  down) → beat 1 real-time stock → beat 2 bulk import → beat 3 calendar → logo
  lock (reuse the Mission 1 sting as the ending if approved)
- **Mood**: same vibrant tropical premium; smooth, confident, zero clutter
- **Text**: NO Thai in-gen (rule 2) — leave clean holds where supers will be
  burned in post; final Thai supers live in `editing/assets-prompts.md` VO/lines
  conventions

## Session-role note

The "FABLE VIDEO AD" Claude Code session authored this library and this
pipeline (scenario/prompt strategy). The Asset Manager session owns files and
exports. The Creative Producer (this brief's executor) RUNS the motion-design
missions in the Higgsfield-connected session. If you are not sure which session
you are: whoever has `mcp__higgsfield__*` tools available executes; everyone
else contributes briefs to this repo.
