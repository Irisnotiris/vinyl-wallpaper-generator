---
name: vinyl-wallpaper-generator
description: Transform a photo, memory, sentence, emotion, story, object, or place into two matching fictional-vinyl-themed mobile wallpapers (cover version + record version). Both are 9:19.6 portrait, with a light gradient background echoing the subject colors, 1-2 hairline decorative curves, no music notes, no status bar, and a minimalist player progress bar at the bottom. The record version includes a tonearm with stylus resting on the outer groove. Use when the user wants to turn an image or idea into a pair of phone wallpapers with a vinyl record / music player aesthetic.
---

# Vinyl Wallpaper Generator

Turn a source photo or idea into two matching fictional-vinyl mobile wallpapers: one cover-art version, one single-record version with tonearm.

The result is a cohesive pair — same fictional release, same palette, same player UI — designed for phone lock/home screens.

## Mandatory Output

Generate exactly **two** images, both **9:19.6 portrait (width:height = 9:19.6)**:

1. **Cover wallpaper** — album cover art centered in the lower half, sitting just above the player bar.
2. **Record wallpaper** — one vinyl record centered in the lower half with a tonearm, sitting just above the player bar.

Both share: the same fictional release identity, the same gradient palette, the same hairline decoration style, and the same bottom player UI.

## Workflow

Follow these steps in order:

1. **Inspect source material** — if a photo is provided, read it and extract: primary anchor, supporting motifs (1-3 colors/textures/lines), material cue, emotional tension, privacy concerns (faces/names/plates). If only text is provided, extract mood, sonic character, place, time, sensory details, and one primary symbol.
2. **Build the fictional release** — invent artist name, album title, label, catalog number, format, sonic character, and concise design history. **Verify the artist name does not collide with a real musical act** via web search; replace any ambiguous name.
3. **Design the visual system** — choose palette (light gradient start color + a darker end color that echoes the cover/record main hue), typography, print texture, and vinyl pressing color/material.
4. **Generate a tracklist** — 2-3 tracks Side A, 2-3 Side B. Vary title length; do not copy the user's sentences literally.
5. **Generate the two wallpapers** — use the prompt templates in `references/prompt_templates.md`. Generate both in parallel.
6. **Verify** — check each image against the constraints below before delivering.

## Source Photo Analysis

When the user uploads a photo:

- Treat it as creative evidence, not a template to reproduce.
- Extract a **primary anchor** (strongest subject/shape/absence) for the cover.
- Extract **supporting motifs** (1-3 colors, textures, lines, shadows) carried across both wallpapers.
- Extract a **material cue** (surface texture) informing paper/vinyl/finishing.
- Identify **emotional tension** (warmth vs. distance, motion vs. stillness, etc.).
- Flag **privacy-sensitive details** (faces, names, addresses, plates, screens). Obscure, crop, or abstract them — never place source-image people in the wallpaper environment.
- Choose a transformation degree: direct photographic / editorial crop / abstracted translation / composite memory.

If the image is unreadable or too low-res, ask for a clearer version.

## Fictional Release Identity

The artist must be wholly fictional. Never use a real musician, band, producer, DJ, composer, or any alias/alternate spelling/near-copy of one.

Before finalizing, search the web for the proposed artist name and close variants. If any meaningful collision appears, discard and regenerate.

Choose names that feel like real independent-label acts — memorable, natural, culturally textured, not randomly generated or brand-like.

## Visual Design Rules

### Gradient background
- Start (top-left): pale warm cream white (`#FDF6EC`) or a pale tint matching the release mood.
- End (bottom-right): a **light, desaturated version of the cover/record's dominant hue** (e.g., if the record is cherry red, end in soft light cherry-warm `#E8C4B8`).
- The gradient must be **extremely gentle** — overall image stays light and pale. Never heavy, saturated, or dark.
- The end color is **derived from the subject**, not fixed.

### Decoration
- **1-2 hairline-thin** flowing curved lines only, in soft warm gold or a matching pale tint.
- **No music notes, no treble clefs, no musical symbols.**
- Lines are sparse, understated, meandering organically.

### Typography
- Choose fonts to match the source photo's mood and atmosphere — do not use one fixed style for every cover.
- **Warm & healing** (cozy, comfortable, healing, soft, everyday warmth) → rounded sans-serif, soft handwritten — e.g., Nunito, Quicksand, Comfortaa, Caveat, Kalam
- **Retro & nostalgic** (nostalgic, vintage, timeless, warm memory) → classic serif, typewriter, retro bold serif — e.g., Playfair Display, Bodoni, Alfa Slab One, Rye, Special Elite
- **Cool & futuristic** (calm, futuristic, tech, detached, avant-garde) → geometric sans-serif, monospace, futuristic display — e.g., Montserrat, Space Grotesk, JetBrains Mono, Orbitron, Audiowide
- **Calm & minimal** (peaceful, minimal, clean, crisp, restrained) → clean sans-serif, thin sans-serif — e.g., Inter, Helvetica, Roboto, Work Sans, Lato
- **Artistic & quiet** (artistic, quiet, dreamy, hazy, emotional) → elegant high-contrast serif, delicate handwritten — e.g., Didot, Bodoni, Cormorant Garamond, Playfair Display, Italianno, Parisienne
- **Classical & poetic** (classical, poetic, serene, Eastern aesthetic, ink wash landscape, calligraphy, traditional patterns, hanfu/architecture) → classical serif, elegant high-contrast serif (songti-like), delicate handwritten — e.g., Cinzel, Trajan Pro, Playfair Display, Cormorant Garamond, Italianno
- **Youthful & romantic** (youthful, romantic, lively, dreamy, summery) → flowing script/handwritten, lively serif — e.g., Caveat, Dancing Script, Permanent Marker, Sacramento, Allura, Abril Fatface
- **Dark & industrial** (dark, edgy, rough, street, powerful, gothic) → bold condensed, slab serif, gothic/decorative serif, distressed display — e.g., Oswald, Bebas Neue, Anton, Rockwell, Arvo, Bungee
- Cover title and artist name should share one coherent type system.

### No system UI
- **Absolutely no** status bar, notch, time display, signal icons, battery icons, carrier text, navigation bar, back button, return arrow, or any smartphone interface element.
- The top of each image must be completely clean empty gradient space.

### Composition
- Subject (cover or record) positioned in the **lower 40-45%** of the canvas, horizontally centered, **sitting just above the player bar** with minimal gap.
- Upper half is empty gradient negative space.
- Bottom-weighted composition.

## Player UI (both wallpapers)

At the very bottom, horizontally centered:

- A thin horizontal progress track: left portion filled in the release accent color (e.g., warm cherry red), right portion in soft warm gray.
- A small circular drag knob in the accent color.
- Above the bar: current time (left) and total time (right) in small warm sans-serif.
- Below the bar: **exactly three** minimalist line-icons — previous (rewind), play/pause, next (forward) — all in the accent color, thin stroke.
- Clean, flat, minimal. No glossy buttons, no 3D, no extra icons (no shuffle, no repeat, no share, no X).

## Cover Wallpaper Specs

- The album cover is a **clean square** with subtle paper edge thickness and soft natural contact shadow.
- Cover content: the primary anchor (from source analysis) rendered through the chosen visual treatments, with release title and artist name in a typography style chosen to match the source photo's mood and atmosphere (see Typography rules above).
- Risograph or subtle print texture is acceptable but must remain light.
- No tonearm on the cover wallpaper.

## Record Wallpaper Specs

- **Exactly one** vinyl record, fully visible, true circular shape, no cropping.
- Vinyl color/material: an intentional pressing (translucent, marble, splatter, smoke, etc.) relating to the concept — not automatically black.
- Center label: artist name, release title, catalog number, and label identity in the release typography. Optionally include a **simplified graphic or symbol derived from the source image** (the primary anchor) as a decorative motif. Small spindle hole in the center. Label background is determined by the overall visual system — no fixed color requirement.
- Subtle groove texture, natural contact shadow, visible edge thickness.

### Tonearm (critical placement)
- A **circular pivot base** (dark ring with lighter center) at the upper-right area, outside and above the record.
- A clean **white slender tonearm** extending from the base, diagonally down-left, curving gracefully over the record.
- The **stylus head** (small white rectangular cartridge) rests on the vinyl at the **OUTER RING** — near the upper-right edge, in the outer groove area, **far from the center label**.
- The stylus must be in the **outer half of the record's radius**, close to the rim — never near the center label.

## Negative Constraints (both wallpapers)

Avoid:
- Any ratio other than 9:19.6 portrait
- Status bar, notch, system UI, back button, or any text/icons at the top
- Music notes, treble clefs, or musical symbols
- Dark, heavy, or saturated gradients — keep it light and pale
- More than 2 decorative curves
- People, faces, hands in the product environment
- Shrink wrap, plastic, cellophane on the record
- Cropped, overlapping, or extra objects
- More than three player control icons
- Glossy CGI appearance or luxury-product staging
- Real artist names as the fictional act

## Output Delivery

After generating both images, deliver them together and provide:

### Release Concept
- Artist, Title, Format, Catalog No., Label, Sonic Character, Design History, Gradient palette

### Tracklist
- Side A and Side B with track numbers and titles

### Wallpaper Notes
- Cover concept, Record concept (vinyl color + tonearm), Source-derived elements used, Transformation degree

See `references/prompt_templates.md` for the complete image-generation prompt templates for both wallpapers.
