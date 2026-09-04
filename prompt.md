# Prompt Library

## Master Prompt

Create a 3:4 vertical Japanese-style travel souvenir poster.

Use the uploaded scenic image as the location reference. If a bookmark reference image is also provided, use it only as a guide for the bookmark's product form, material, proportions, hanging cord, and craftsmanship.

Create a refined split composition:

- LEFT: a beautiful poster-style interpretation of the scenic location
- RIGHT: one matching souvenir bookmark newly designed from that same location

### Overall direction

- elegant Japanese aesthetic
- pale blue / mist blue background
- light luxury
- calm and delicate
- premium collectible souvenir
- clean editorial layout
- subtle paper texture
- restrained decorative motifs

### Stability controls

Assign the uploaded images explicitly before interpreting them:

- **Image A — scenic source:** the only authority for the destination, scenery, landmark facts, and palette.
- **Image B — product reference:** the only authority for one bookmark's physical form, material, proportions, cord, and construction. If it contains several bookmarks, choose one and generate exactly one.
- **Image C — style/layout reference:** the only authority for split layout, spacing, typography hierarchy, background treatment, and finish. Do not copy its landmark artwork or text.

Use an exact 3:4 portrait canvas (for example, 1086×1448; never 2:3, 4:5, or square), a fixed 60% left / 40% right split, one centered hero bookmark, and one hanging cord. Preserve three to five observable facts from Image A. Keep typography to the exact labels supplied by the user; if a location is not confirmed, omit the location label. Do not invent text.

### Left side — scenery

Preserve the recognizability of the original location.

Identify and retain the most distinctive visual features from the uploaded photo, such as:
- landmark architecture
- roof shape
- water
- boats
- bridge
- mountain
- trees
- street geometry
- skyline
- local building details

Simplify visual clutter while keeping the place recognizable.

Use:
- soft natural light
- mild haze
- refined detail
- generous breathing room
- subtle Japanese decorative motifs only when useful

Do not let decorative elements overpower the location.

### Right side — bookmark

Design ONE premium souvenir bookmark inspired by the same destination.

The bookmark must:
- look like a real collectible product
- translate the scenery into simplified decorative artwork
- NOT use a direct photo crop
- preserve key scene motifs
- include believable material, depth, edges, and shadows
- include a hanging cord if appropriate
- include the destination name and country / region

Possible construction:
- brushed metal frame
- enamel inlay
- engraved metal
- polished alloy
- metal cutout
- carved wood
- embossed layered relief

If a bookmark reference image is provided:
- reference its proportions and product character
- reference its cord / hanging structure
- reference its craftsmanship and material cues
- DO NOT copy its exact artwork

### Color rules

Build the palette from the scenic photo.

Extract:
1. dominant color
2. secondary landmark color
3. accent color
4. neutral tone

Then soften and refine them.

Default visual balance:
- 55–65% pale blue / mist blue
- 15–25% scenic-derived primary color
- 10–15% secondary scenic color
- 3–6% metallic / gold accent
- remaining area in ivory or muted neutral tones

Avoid:
- neon colors
- overly saturated colors
- harsh pure black
- bright yellow gold
- cheap-looking glossy plastic

### Typography

Use elegant Japanese-inspired editorial typography.

Include:
- [LOCATION NAME]
- [COUNTRY / REGION]

Optional:
- one short poetic Japanese phrase

Keep typography restrained and readable.

### Final goal

Create a visually unified high-end travel poster where the scenic location on the left and the matching souvenir bookmark on the right clearly belong to the same destination and design system.

The result should feel suitable for a premium tourism campaign, collectible travel series, or sophisticated social-media post.

### Final rejection checks

Reject and regenerate if any of these occur: the canvas is not exact 3:4, more than one bookmark, a direct photo crop inside the bookmark, a changed or generic scenic subject, copied artwork from a reference image, an invented place name, pseudo-text, logo, watermark, or a layout that is not a clear left-scenery/right-bookmark split. Repeat the exact ratio instruction on the retry.


---

# Scenic-Only Mode

Use this when the user provides only a scenic image.

Create a premium bookmark design automatically based on the scene.

Default bookmark interpretation:
- refined brushed metal or enamel
- vertical slim proportions
- matching hanging cord
- scenic motifs simplified into layered decorative shapes

Use the scenic photo's own colors to define:
- bookmark enamel colors
- cord color
- engraved details
- metallic accents


---

# Reference Bookmark Mode

Use this when the user provides:
- Image A: scenic photo
- Image B: bookmark reference

Image A controls:
- destination
- scenery
- landmark elements
- palette inspiration

Image B controls only:
- bookmark product form
- proportions
- material direction
- cord style
- craftsmanship feeling

Do not copy Image B's original landmark artwork.

Create a new bookmark that belongs to Image A's destination.


---

# Variable Template

Replace the variables before generation:

LOCATION NAME:
[LOCATION NAME]

COUNTRY / REGION:
[COUNTRY / REGION]

OPTIONAL PHRASE:
[OPTIONAL PHRASE]

BOOKMARK MATERIAL:
[AUTO / METAL / ENAMEL / WOOD / OTHER]

MUST-PRESERVE SCENIC FEATURES:
[KEY FEATURES]

OPTIONAL COLOR DIRECTION:
[AUTO / USER PREFERENCE]

SCENIC SOURCE FACTS:
[3–5 facts visible in the scenic image]

PRODUCT REFERENCE CUES:
[single bookmark form, material, cord, and construction cues]

STYLE / LAYOUT REFERENCE CUES:
[split ratio, palette, typography hierarchy, and finish]
