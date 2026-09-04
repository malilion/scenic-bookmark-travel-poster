---
name: scenic-bookmark-travel-poster
description: Create a 3:4 Japanese-style travel poster from an uploaded scenic photo, with the scenery on the left and a matching premium souvenir bookmark on the right. Use when the user wants a landmark/travel image transformed into a refined collectible bookmark concept, especially with pale-blue Japanese editorial styling.
---

# Scenic Bookmark Travel Poster

## Goal

Create one polished **3:4 vertical poster** that visually connects:

- **Left:** the user's scenic travel image
- **Right:** a matching souvenir bookmark designed from that scenery

The final image should look like a premium Japanese travel collectible campaign.

## Inputs

Required:
- Scenic image
- Location name in English
- Country / region in English

Optional:
- Bookmark reference image
- Material preference
- Color preference
- Poetic phrase
- Landmark feature that must be preserved

## Default interpretation

If the user only uploads one scenic image:
- infer a suitable premium bookmark style
- default to brushed metal / enamel unless the scene strongly suggests another material
- use a coordinated cord color derived from the scenic palette

If a bookmark reference image is provided:
- use it only for product form, material, proportions, hanging cord, and craftsmanship cues
- do not copy its exact artwork
- design a new bookmark based on the scenic image

## Stability controls

Apply these controls whenever more than one image is supplied:

1. Assign every image one role before generating:
   - **scenic source:** controls the destination, landscape, landmark features, and palette
   - **product reference:** controls only the physical bookmark form, material, cord, and construction
   - **style / layout reference:** controls only the poster grid, visual hierarchy, spacing, and finish
2. If the product reference shows multiple bookmarks, select the clearest single bookmark and generate exactly one product.
3. Preserve three to five concrete scenic facts in the prompt. For example: `moss-covered rocks`, `small cascades`, `bare trees`, `patches of snow`, and `wooden footbridge`.
4. Keep the output geometry fixed at an exact 3:4 portrait canvas and a 60/40 left-scenery/right-bookmark split unless the user explicitly requests another ratio. Treat 2:3, 4:5, and square outputs as failures.
5. Use one centered hero bookmark with one cord. Do not generate a product collection, flat-lay, or collage.
6. Treat text as a closed set. Use only caller-supplied labels. If the user has not supplied a confirmed location name, omit the location label instead of inventing one.
7. Disable the optional poetic Japanese phrase by default when exact text matters. Never add pseudo-text, unrelated branding, watermarks, or unrelated place names. Text or signage that is visibly part of the scenic source may remain when it is necessary to preserve a recognizable landmark.

Before finalizing, check the image against the role assignments and reject it if the canvas is not 3:4, the bookmark copies a reference photo, the scenery changes identity, more than one bookmark appears, or unrelated generated text is present. Source-native landmark signage is allowed; invented or decorative pseudo-text is not. If the canvas ratio is wrong, regenerate once with the ratio lock repeated verbatim before considering any pixel-level normalization.

## Composition

Use a split vertical poster:

- Left panel: approximately 55–65%
- Right panel: approximately 35–45%

### Left panel

Preserve the location's recognizability.

Extract and retain the most distinctive visual elements, such as:
- landmark silhouette
- roof shape
- canal / river / coast
- bridge
- temple / shrine
- street
- mountain
- vegetation
- skyline
- local architectural pattern

Simplify visual clutter where useful.

The result should feel:
- airy
- calm
- refined
- editorial
- premium
- travel-oriented

### Right panel

Create one hero bookmark.

The bookmark must:
- clearly refer to the same destination
- translate the location into simplified decorative artwork
- look manufacturable
- have convincing material and depth
- include a hanging cord when appropriate
- include location text
- remain visually dominant on the right

Possible bookmark treatments:
- brushed metal
- enamel inlay
- polished alloy
- engraved metal
- carved wood
- embossed material
- metal cutout
- layered relief

## Color system

Use this default balance:

- 55–65% pale blue / mist blue / paper blue
- 15–25% scenic-derived primary color
- 10–15% secondary scenic color
- 3–6% metallic or gold accents
- remaining area in ivory / charcoal / muted neutrals

### Color extraction logic

From the scenic image, identify:
1. Dominant environmental color
2. Secondary landmark color
3. Accent color
4. Neutral / stone / paper tone

Then soften the palette:
- slightly desaturate
- avoid neon tones
- avoid harsh pure black
- avoid bright yellow gold

Preferred metallic accents:
- antique gold
- champagne gold
- brushed silver
- warm brass

## Typography

Always include:
- location name
- country / region

Use English for destination labels unless the user requests another language.

Optional:
- one short poetic Japanese phrase
- one small seal-like decorative element

Typography should feel:
- elegant
- editorial
- restrained
- integrated with the layout

Do not overfill the image with text.

## Japanese decorative motifs

Use only when they support the destination and composition.

Possible motifs:
- seigaiha wave pattern
- cloud-line motifs
- maple leaves
- ginkgo leaves
- small birds
- thin gold linework
- paper texture
- subtle seal mark

Keep them secondary.

## Product realism

The bookmark should show believable:
- metal / wood texture
- thickness
- edge highlights
- engraved or enamel details
- shadow
- cord attachment
- craftsmanship

Avoid:
- flat sticker appearance
- plastic toy look
- impossible geometry
- excessive ornament
- direct photo pasted onto the bookmark

## Text accuracy

Use the exact user-provided location and country/region.

If typography generation is unreliable:
- prioritize clean readable English destination text
- minimize extra decorative text
- do not invent a location name, country/region, or unrelated place name
- when no confirmed location label is available, use no destination text rather than a guessed label
- allow source-native landmark signage only when it is visibly present in the scenic source and supports recognition

## Quality checklist

Before finalizing, confirm:

- [ ] 3:4 vertical composition
- [ ] scenery is on the left
- [ ] bookmark is on the right
- [ ] location remains recognizable
- [ ] bookmark is newly designed from the scenery
- [ ] bookmark looks like a real collectible product
- [ ] pale-blue Japanese visual system is coherent
- [ ] colors are derived from the scenic image
- [ ] location and country/region are present
- [ ] layout is not cluttered
- [ ] scenery and bookmark feel like one visual series

## Generation instruction

Use the master prompt in `prompt.md`.

When the user supplies both scenic and bookmark reference images, use the "Reference Bookmark Mode" prompt section.

When the user supplies only a scenic image, use the "Scenic-Only Mode" prompt section.
