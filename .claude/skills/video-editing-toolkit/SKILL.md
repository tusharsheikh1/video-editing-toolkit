---
name: video-editing-toolkit
description: Search, browse, and match motion graphics assets, cutouts, icons, vectors, and overlays from Video Editing Toolkit to video scripts or editing concepts.
---

# Video Editing Toolkit Asset Matching & Search Skill

Use this skill to quickly find, recommend, and match motion design assets, overlays, vectors, audio, and cutouts from the repository for video editing projects and voiceover scripts.

The repository contains **6,200+ production-ready assets**:
- **3,460+ Brand SVG Logos** (`icons/svg/brands/`)
- **2,000+ UI & Media Vector Icons** (`icons/svg/ui/`)
- **370+ PNG Motion Cutouts & Objects** (`png-assets/`)
- **320 Lossless WAV Sound Effects** (`audio/sound-effects/`) across 28 categories
- **5 Cinematic 3D LUTs** (`luts/`)
- **Alpha/Luma Matte Transitions** (`transitions/`)
- **Subtitle & Caption Templates** (`captions/`)

## Directory Structure & Asset Types

```
.
├── audio/
│   ├── sound-effects/    # 320 lossless WAV SFX (whooshes, risers, booms, impacts, UI, etc.)
│   ├── background-music/ # Background tracks (.mp3)
│   └── ambience/         # Atmospheric audio beds
├── b-roll/
│   ├── lifestyle/        # Video clips (.mp4) and photographic cutouts
│   ├── nature/           # Environment footage
│   ├── city/             # Urban footage
│   └── technology/       # Tech clips
├── captions/             # Subtitle templates (.srt, .vtt)
├── editing-templates/    # NLE project templates (Premiere Pro, AE, Resolve, CapCut)
├── icons/
│   ├── svg/
│   │   ├── brands/       # 3,400+ SVG brand and platform logos (CC0)
│   │   └── ui/           # 2,000+ SVG UI, editing tool, media controls (ISC/MIT)
│   ├── png/              # High-res UI icons & brand logos
│   └── animated/         # Looping animated GIF reactions
├── luts/                 # 3D cinematic LUTs (.cube) with previews
├── motion-graphics/      # 3D icon collages and abstract visual scenes
├── overlays/             # Light rays bursts, page curls, atmospheric effects
├── png-assets/
│   ├── cutouts/          # Classical statues (01-36), body parts, gestures, people silhouettes
│   ├── stickers/         # Badges, shapes, sparkles, fire frames, lightning, particles
│   └── objects/          # Clocks, compasses, money, cards, chess, crypto, devices, masks
├── titles-and-text/      # Text overlays and typography cutouts
├── transitions/          # Alpha/Luma matte transition SVGs (wipes, iris, slashes)
├── ui-assets/            # Dark mode UI buttons, video player frames
└── vectors/
    ├── illustrations/    # 3D & 2D scene/character illustrations (illustration_*.png)
    ├── arrows/           # Directional pointers and visual flow arrows (arrow_*.png)
    └── infographics/     # Market charts, coin growth, productivity graphs (chart_*.png)
```

## Key Search & Match Workflow

When the user asks to find assets for a script, topic, or scene:

1. **Identify the Core Theme**:
   - **Finance & Wealth**: Search `png-assets/objects/money_*`, `crypto_*`, `card_*`, `vectors/infographics/chart_*`
   - **Sound Design & Foley**: Search `audio/sound-effects/` by category (`whooshes`, `risers-and-fallers`, `impacts`, `pops`, `booms-and-bass`, `interface`, etc.) or check `audio/sound-effects/CATALOGUE.md`.
   - **Cinematic Grading**: Recommend `luts/slay-01-amber.cube` (warm sunset), `slay-02-fade.cube` (film matte), `slay-03-neon.cube` (cyberpunk/night), `slay-04-film.cube` (teal & orange), `slay-05-portrait.cube` (soft skin tones).
   - **Time & Urgency**: Search `png-assets/objects/object_alarm-clock_*`, `object_hourglass_*`, `icons/png/icon_clock_*`, or `audio/sound-effects/time/`
   - **Brands & Tech Logos**: Search `icons/svg/brands/<brand-name>.svg`
   - **UI & Media Controls**: Search `icons/svg/ui/<tool-or-control>.svg`
   - **Strategy & Leadership**: Search `png-assets/objects/chess_*`, `png-assets/objects/object_compass_*`
   - **Emotions & Reactions**: Search `icons/animated/*.gif`, `png-assets/cutouts/people_*`, `vectors/illustrations/illustration_angry*`
   - **Art & Philosophy**: Search `png-assets/cutouts/01_` through `36_` (classical sculptures, busts, marble heads)
   - **Transitions & Cuts**: Search `transitions/matte_*` or `audio/sound-effects/whooshes/` and `swishes-and-zips/`
   - **Visual Effects & Accents**: Search `png-assets/stickers/sparkle_*`, `lightening_*`, `fire*`, `overlays/effect_*`

2. **Check Index Metadata**:
   - Inspect `PNG_INDEX.md` for raster PNG asset keywords and pixel dimensions.
   - Inspect `audio/sound-effects/CATALOGUE.md` and `sounds.json` for audio loudness, sync points, and usage advice.
   - Consult `ASSET-LICENSES.csv` for exact licensing terms.

3. **Output Format**:
   Return matching assets in a clean markdown table:
   | Asset Name | Relative Path | Type | Recommended Cue / Technique |
   |------------|---------------|------|-----------------------------|
   | `money_cash-stacks-fanned.png` | `png-assets/objects/money_cash-stacks-fanned.png` | PNG Cutout | In on "doubled revenue", scale pop |
   | `riser-heavy-cinematic-01.wav` | `audio/sound-effects/risers-and-fallers/...` | Audio SFX | Sync peak with graphic reveal |
   | `slay-04-film.cube` | `luts/slay-04-film.cube` | 3D LUT | Apply as Lumetri input LUT |
