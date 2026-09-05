# Image Generation Prompt Templates

Use these templates when generating the two wallpapers. Replace all `{placeholders}` with values derived from the source material and the fictional release. Generate both images in parallel.

Recommended dimensions: **width=940, height=2048** (9:19.6 ratio).

---

## Template 1: Cover Wallpaper

```
Exactly one 9:19.6 portrait mobile wallpaper (width:height = 9:19.6, very tall and narrow).

BACKGROUND: A very subtle, light gradient from {pale_start_color} at the top-left to {light_subject_hue_end_color} at the bottom-right — the dark end echoes the {dominant_subject_color} of the album cover. The gradient is extremely gentle, keeping the overall image light and pale, not saturated or heavy. No scenery, no rooms, no furniture.

DECORATION: Only ONE or TWO very thin, delicate, flowing curved lines across the background — hairline-thin strokes in {decoration_line_color}, meandering gently. Minimal and sparse. Absolutely NO music notes, NO treble clefs, NO musical symbols.

CRITICAL: Absolutely NO status bar, NO notch, NO time display, NO signal icons, NO battery icons, NO carrier text, NO phone system UI, NO navigation bar, NO back button, NO return arrow, NO text or icons at the top of the image. The top of the image must be completely clean empty gradient space.

Lower-center of the image (positioned in the lower 45% of the canvas, horizontally centered, sitting just above the player bar): The album cover art for '{album_title}' by {artist_name}. {cover_visual_description — primary anchor, visual treatments, symbolic anchor, composition}. At the top of the cover, small refined caps text '{artist_name}'. Below the main visual, large warm elegant serif title '{album_title}'. The cover is a clean square with subtle paper edge thickness and soft natural contact shadow. {print_texture_description}.

Bottom of the image (very bottom): A minimalist music player progress bar UI, horizontally centered, directly beneath the cover. Thin horizontal track line — left portion filled in {accent_color}, right portion in soft warm gray. Small circular {accent_color} drag knob. Above bar left: '{current_time}', above bar right: '{total_time}'. Below bar: three minimalist line-icons — previous (rewind), play/pause (triangle), next (forward) — all in {accent_color}, thin stroke. Clean flat minimal style. No extra icons.

Overall light, pale, airy, warm, minimal aesthetic. No people, no hands. Bottom-weighted composition with empty gradient space on top.
```

---

## Template 2: Record Wallpaper

```
Exactly one 9:19.6 portrait mobile wallpaper (width:height = 9:19.6, very tall and narrow).

BACKGROUND: A very subtle, light gradient from {pale_start_color} at the top-left to {light_subject_hue_end_color} at the bottom-right — the dark end echoes the {dominant_subject_color} of the vinyl record. The gradient is extremely gentle, keeping the overall image light and pale, not saturated or heavy. No scenery, no rooms, no furniture.

DECORATION: Only ONE or TWO very thin, delicate, flowing curved lines across the background — hairline-thin strokes in {decoration_line_color}, meandering gently. Minimal and sparse. Absolutely NO music notes, NO treble clefs, NO musical symbols.

CRITICAL: Absolutely NO status bar, NO notch, NO time display, NO signal icons, NO battery icons, NO carrier text, NO phone system UI, NO navigation bar, NO back button, NO return arrow, NO text or icons at the top of the image. The top of the image must be completely clean empty gradient space.

Lower-center of the image (positioned in the lower 45% of the canvas, horizontally centered, sitting just above the player bar): Exactly ONE vinyl record, fully visible, true circular shape, no cropping, no second record. {vinyl_color_and_material_description — e.g., translucent cherry red with cream marble swirl}. Center label in {label_color} with {label_text_color} warm serif text: '{artist_name}', '{album_title}', '{catalog_number}', '{label_name}'. Small spindle hole. Subtle vinyl groove texture. Natural soft contact shadow beneath the record. Subtle vinyl edge thickness visible.

TONEARM — critical placement: A circular pivot base (dark ring with lighter center) located at the upper-right area of the image, outside and above the record. From this base, a clean white slender tonearm extends diagonally down-left, curving gracefully over the upper-right quadrant of the record. The stylus head (small white rectangular cartridge) rests precisely on the vinyl surface at the OUTER RING of the record — near the upper-right edge, in the outer groove area, FAR from the center label. The stylus must be positioned in the outer half of the record's radius, close to the rim, not near the center label. This mirrors a turntable needle playing the beginning tracks on the outer edge of a vinyl record. The arm is minimal and sleek, no complex mechanics visible.

Bottom of the image (very bottom): A minimalist music player progress bar UI, horizontally centered, directly beneath the record. Thin horizontal track line — left portion filled in {accent_color}, right portion in soft warm gray. Small circular {accent_color} drag knob. Above bar left: '{current_time}', above bar right: '{total_time}'. Below bar: three minimalist line-icons — previous (rewind), play/pause (triangle), next (forward) — all in {accent_color}, thin stroke. Clean flat minimal style. No extra icons.

Overall light, pale, airy, warm, minimal aesthetic. No people, no hands, no shrink wrap, no plastic. Bottom-weighted composition with empty gradient space on top. The record with tonearm is the clear focal point.
```

---

## Placeholder Reference

| Placeholder | Description | Example |
|---|---|---|
| `{pale_start_color}` | Gradient start (top-left), pale warm | `#FDF6EC` (pale warm cream white) |
| `{light_subject_hue_end_color}` | Gradient end (bottom-right), light desaturated version of subject hue | `#E8C4B8` (soft light cherry-warm) |
| `{dominant_subject_color}` | The main color of cover/record | `cherry red` |
| `{decoration_line_color}` | Hairline curve color | `soft warm gold` |
| `{accent_color}` | Player UI accent color | `warm cherry red` |
| `{artist_name}` | Fictional artist (verified no collision) | `Slow Lantern` |
| `{album_title}` | Album title | `Candlewood` |
| `{catalog_number}` | Label catalog number | `HL-014` |
| `{label_name}` | Fictional label | `Half-Light Records` |
| `{cover_visual_description}` | Cover art description derived from source | See below |
| `{print_texture_description}` | Print texture | `Risograph printed texture with slight ink misregistration` |
| `{vinyl_color_and_material_description}` | Vinyl pressing description | `Translucent cherry red vinyl with cream marble swirl` |
| `{label_color}` | Center label background | `cream` |
| `{label_text_color}` | Center label text | `cherry red` |
| `{current_time}` | Player current time | `1:42` |
| `{total_time}` | Player total time | `3:58` |

## Cover Visual Description Guidance

Write 2-4 sentences covering:
1. The primary anchor (source-derived subject/shape/symbol)
2. Visual treatments (color reconstruction, soft focus, bloom, collage, etc. — choose 2-4 coherent ones)
3. Composition and negative space
4. How the source elements are transformed (not reproduced literally)

Example:
> A single bent golden candle stem with a small glowing orange flame rising from a soft hazy field of warm cream and deep cherry red. The flame blooms with soft diffused warm light. An abstracted soft geometric cheesecake-slice shape sits low within the cover, partially obscured by warm haze. Large negative space around the candle.
