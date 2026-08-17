# Photo Random Paint

Recompose a supplied photograph as a restrained editorial print and add tactile impasto paint dots whose color is extracted from the photograph's strongest existing visual anchor. Use when the user asks for reference-style paint circles, color-anchor dots, photo cropping and layout with painted dots, or wants a photo treated like an inset magazine image with thick handmade color marks.

## What It Does

- Recomposes the photo into a vertical editorial layout with an inset photo, warm paper margin, and generous whitespace
- Samples the strongest subject-linked color anchor from the photograph itself (never from a reference image)
- Adds 6–9 irregular, raised impasto paint dots with 3–4 size levels in the anchor color
- Builds an asymmetric dot rhythm: large edge anchors, medium compositional bridges, small accents
- Renders thick acrylic/oil impasto with palette-knife ridges, uneven handmade edges, and contact shadows
- Keeps the face and defining details clear — dots may cross the photo edge into the margin but never obscure the subject

## Installation

### Claude Code

```bash
# Clone the repo
git clone https://github.com/sosotsai/photo-random-paint.git

# Symlink into your skills directory (macOS/Linux)
ln -s "$(pwd)/photo-random-paint" ~/.claude/skills/photo-random-paint
```

### Codex (OpenAI)

Copy the folder into `~/.codex/skills/`:

```bash
git clone https://github.com/sosotsai/photo-random-paint.git
cp -r photo-random-paint ~/.codex/skills/photo-random-paint
```

Then ask your assistant to use the `photo-random-paint` skill on any photograph.

## Usage

1. Supply a photograph
2. Ask to recompose it with paint dots (the dot color is chosen automatically from the photo's strongest color anchor)
3. Review the result — identity and composition are always preserved

## Files

- `SKILL.md` — the skill definition and workflow
- `assets/icon.svg` — skill icon

## License

MIT
