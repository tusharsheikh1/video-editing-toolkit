---
name: editvault
description: Search, browse, and match motion graphics assets, cutouts, icons, vectors, and overlays from EditVault to video scripts or editing concepts.
---

# EditVault Asset Matching & Search Skill

Use this skill to quickly find, recommend, and match motion design assets, overlays, vectors, audio, and cutouts from the repository for video editing projects and voiceover scripts.

## Directory Structure & Asset Types

The repository contains curated assets organized into:

```
├── b-roll/
│   ├── lifestyle/        # Video clips (.mp4) and photographic cutouts
│   ├── nature/           # Environment footage
│   ├── city/             # Urban footage
│   └── technology/       # Tech clips
├── vectors/
│   ├── illustrations/    # 3D & 2D scene/character illustrations (illustration_*.png)
│   ├── arrows/           # Directional pointers and visual flow arrows (arrow_*.png)
│   └── infographics/     # Market charts, coin growth, productivity graphs (chart_*.png)
├── png-assets/
│   ├── cutouts/          # Classical statues (01-36), body parts, gestures, people silhouettes
│   ├── stickers/         # Badges, shapes, sparkles, fire frames, lightning, particles
│   └── objects/          # Clocks, compasses, money, cards, chess, crypto, devices, masks
├── icons/
│   ├── png/              # High-res UI icons and brand logos (Adobe, YouTube, IG, etc.)
│   ├── animated/         # Looping animated GIF reactions (verified, bonus, happy, etc.)
│   └── svg/              # Scalable vector icons
├── audio/
│   ├── background-music/ # Background tracks (.mp3)
│   ├── sound-effects/    # SFX risers, whooshes, clicks
│   └── ambience/         # Atmospheric audio beds
├── overlays/             # Light rays bursts, page curls, atmospheric effects
├── motion-graphics/      # 3D icon collages and abstract visual scenes
├── titles-and-text/      # Text overlays and typography cutouts
├── backgrounds/          # Grass fields, empty rooms, background backdrops
├── ui-assets/            # Dark mode UI buttons, video player frames
└── editing-templates/    # NLE project templates (Premiere Pro, AE, Resolve, CapCut)
```

## Key Search & Match Workflow

When the user asks to find assets for a script, topic, or scene:

1. **Identify the Core Theme**:
   - **Finance & Wealth**: Search `png-assets/objects/money_*`, `crypto_*`, `card_*`, `vectors/infographics/chart_*`
   - **Time & Urgency**: Search `png-assets/objects/object_alarm-clock_*`, `object_hourglass_*`, `icons/png/icon_clock_*`
   - **Strategy & Leadership**: Search `png-assets/objects/chess_*`, `png-assets/objects/object_compass_*`
   - **Emotions & Reactions**: Search `icons/animated/*.gif`, `png-assets/cutouts/people_*`, `vectors/illustrations/illustration_angry*`
   - **Art & Philosophy**: Search `png-assets/cutouts/01_` through `36_` (classical sculptures, busts, marble heads)
   - **Visual Effects & Accents**: Search `png-assets/stickers/sparkle_*`, `lightening_*`, `fire*`, `overlays/effect_*`
   - **Software & Brands**: Search `icons/png/logo_*` (Premiere, Photoshop, After Effects, YouTube, Instagram)

2. **Check Index Metadata**:
   - Inspect `PNG_INDEX.md` for exact resolution and keyword descriptions.
   - For license confirmation, consult `ASSET-LICENSES.csv`.

3. **Output Format**:
   Return matching assets in a clean markdown table:
   | Asset Name | Relative Path | Recommended Use / Cue |
   |------------|---------------|-----------------------|
   | `money_cash-stacks-fanned.png` | `png-assets/objects/money_cash-stacks-fanned.png` | In on "doubled revenue" |

4. **Editing Advice**:
   - For cutouts (`png-assets/cutouts/`): Recommend pop-up / scale bounce with paper tear texture or drop shadow.
   - For stickers (`png-assets/stickers/`): Recommend flash frame (3-5 frames) on beat drops.
   - For overlays (`overlays/`): Recommend Screen / Add blend mode in Premiere / After Effects.
