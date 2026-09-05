# vinyl-wallpaper-generator

Turn a photo, memory, sentence, emotion, story, object, or place into **two matching fictional-vinyl-themed mobile wallpapers** — a cover-art version and a single-record version with tonearm.

Built as an agent Skill (SKILL.md convention) — drop it into any skills directory and the agent will use it automatically when relevant.

## What it does

Given a source photo or a text idea, the skill:

1. **Analyzes the source** — extracts a primary visual anchor, supporting color/texture motifs, material cues, emotional tension, and privacy concerns (faces, names, plates).
2. **Builds a fictional release** — invents an artist name, album title, label, catalog number, sonic character, and design history. Artist names are web-search-verified to avoid collisions with real musicians.
3. **Designs the visual system** — palette, typography, print texture, and vinyl pressing color.
4. **Generates a tracklist** — varied track titles for Side A and Side B.
5. **Outputs two 9:19.6 wallpapers** in parallel.

## Output

Two images, both **9:19.6 portrait** (940 × 2048):

| Wallpaper | Description |
|---|---|
| **Cover version** | Album cover art centered in the lower half, sitting just above the player bar. |
| **Record version** | One vinyl record centered in the lower half with a tonearm; stylus rests on the **outer groove** (far from center label). |

Both share:
- Light gradient background (pale start → a desaturated tint of the subject's dominant color)
- 1–2 hairline decorative curves (no music notes)
- No status bar, notch, or any system UI
- Minimalist bottom player UI (progress bar + exactly three control icons)

## Installation

Clone into your agent's skills directory:

```bash
git clone https://github.com/Irisnotiris/vinyl-wallpaper-generator.git ~/.your-skills-dir/vinyl-wallpaper-generator
```

Or copy the folder into any directory the agent scans for skills. Keep `SKILL.md` at the root.

## Usage

Invoke naturally — the skill triggers on requests like:

- *"用 vinyl-wallpaper-generator 把这张照片做成壁纸"*
- *"Turn this memory into two vinyl wallpapers"*
- *"把'我们活着如同独自做梦'做成两张黑胶手机壁纸"*

The agent will handle the full workflow automatically and deliver both wallpapers plus the release concept, tracklist, and design notes.

## Repository structure

```
vinyl-wallpaper-generator/
├── SKILL.md                          # Main skill document (workflow + design specs)
├── README.md
├── LICENSE
└── references/
    └── prompt_templates.md           # Complete image-generation prompt templates with placeholders
```

## License

MIT
