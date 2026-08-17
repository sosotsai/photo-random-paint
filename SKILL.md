---
name: photo-random-paint
description: Recompose a supplied photograph as a restrained editorial print and add tactile impasto paint dots whose color is extracted from the photograph's strongest existing visual anchor. Use when the user asks for reference-style paint circles, color-anchor dots, photo cropping and layout with painted dots, or wants a photo treated like an inset magazine image with thick handmade color marks.
---

# Photo Random Paint

Transform one supplied photograph into an editorial image with an inset photo, paper margin, and raised handmade paint dots. Use image generation/editing; preserve the source photograph rather than recreating it.

## Workflow

1. Inspect the photograph and any style reference before editing.
2. Identify the subject, movement or gaze direction, important negative space, structural lines, and strongest existing color anchor.
3. State the selected anchor color briefly before generation when useful. Do not ask for confirmation unless two candidates are genuinely equal and would create materially different results.
4. Recompose the photo into a vertical editorial layout unless the user specifies another ratio.
5. Add irregular, raised impasto paint dots using the anchor color.
6. Inspect the result. Correct color choice, subject drift, overly perfect circles, weak texture, or mechanical placement with one targeted edit.

## Choose the Anchor Color

Select a color already present in the photograph; never default to the color in a reference image.

Use this priority order:

1. A distinctive saturated color on the primary subject, especially clothing or an accessory.
2. A small but semantically important colored object that already attracts the eye.
3. A recurring environmental accent that supports the subject.
4. If the photograph is nearly monochrome, choose a restrained tint sampled from its warmest or coolest meaningful area instead of inventing an unrelated bright color.

Prefer a color that is visually distinctive, belongs to the subject, survives repetition, and does not compete with skin tones. Sample its perceived hue rather than forcing an exact flat digital value. Preserve tiny highlight and shadow shifts created by thick paint.

Do not:

- copy the reference image's dot color automatically;
- introduce a second unrelated accent palette;
- choose black, white, skin tone, or a large neutral background merely because it occupies the most pixels;
- increase saturation so far that the dots no longer feel connected to the source anchor.

If two strong anchors exist, choose the one closest to the primary subject. Use multiple colors only when the user explicitly requests them.

## Compose the Photograph

- Preserve the real person, face, anatomy, clothing, objects, spatial perspective, motion blur, grain, and photographic mood.
- Crop to strengthen the original subject rather than replace or redraw it.
- Use an inset rectangular photograph on warm off-white or context-appropriate paper with generous margins when the reference calls for it.
- Let the subject's motion, gaze, and open space determine placement.
- Keep key anatomy and the main silhouette readable. Never place a dot over the face or defining subject detail.
- Allow selected dots to cross the photograph edge into the paper margin so the two layers feel integrated.
- Avoid rigid symmetry and template-like even spacing.

## Design the Paint Dots

- Usually use 6–9 dots with 3–4 size levels; adapt to the amount of negative space.
- Build an asymmetric rhythm: large edge anchors, medium compositional bridges, and small accents that guide the eye.
- Render opaque acrylic or oil impasto with palette-knife ridges, uneven handmade edges, slight thickness, and believable contact shadows.
- Keep forms circular enough to read as dots but never perfect vector circles.
- Use dots only unless the user asks for strokes or other marks.

Avoid bubbles, glossy spheres, flat stickers, clean vector shapes, repeated identical discs, clip-art shadows, excessive overlap, text, logos, and watermarks.

## Image Editing Prompt Pattern

Use the original as the edit target and any additional image as style reference only. Include these invariants:

```text
Use case: compositing / style-transfer
Input roles: source photograph = exact edit target; reference = layout and paint-texture language only.
Primary request: recompose the source as a restrained editorial print and add 6–9 tactile impasto paint dots.
Anchor color: sample the strongest existing subject-linked color from the source photograph: <describe selected element and perceived color>. Repeat only this color, with natural ridge highlights and shadows.
Composition: preserve subject identity, anatomy, pose, clothing, meaningful objects, perspective, motion, grain, and mood. Use motion/gaze/negative space to place varied dots; selected dots may cross the photo edge; do not obscure the face or defining details.
Paint texture: opaque thick acrylic/oil, palette-knife ridges, irregular handmade circular edges, subtle contact shadows.
Avoid: copying the reference color, new objects, subject reconstruction, perfect circles, bubbles, glossy spheres, flat stickers, symmetric spacing, text, logos, watermarks.
```

If the user requests only a color correction, edit only the dots' color and explicitly preserve their number, position, size, shape, texture, layout, and the complete photograph.
