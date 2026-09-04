# Examples

## Example 1 — Otaru Canal

### Input
Scenic image:
- Otaru Canal
- stone warehouses
- blue roofs
- canal water
- small boat

Bookmark reference:
- slim vertical metal souvenir bookmark
- blue cord
- enamel / cutout construction

Location:
`OTARU CANAL`

Country / region:
`HOKKAIDO, JAPAN`

### Scenic extraction
Primary motifs:
- blue warehouse roof
- stone warehouse wall
- canal water
- small boat

Primary palette:
- mist blue
- roof blue
- deep canal blue
- stone brown
- brushed silver

### Bookmark translation
Use:
- brushed metal outer frame
- blue enamel roof
- simplified stone warehouse pattern
- canal reflection lines
- one small boat
- deep blue braided cord

The bookmark should not contain a photographic crop.

### Expected composition
Left:
- refined Otaru Canal scene

Right:
- premium Otaru Canal metal bookmark

Overall:
- pale-blue Japanese editorial travel poster


---

## Example 2 — Kyoto Shrine

### Input
Scenic image:
- vermilion torii gates
- stone path
- green foliage

Location:
`FUSHIMI INARI`

Country / region:
`KYOTO, JAPAN`

### Palette
- pale blue background
- muted vermilion
- moss green
- warm ivory
- antique gold

### Bookmark
- antique-gold metal frame
- vermilion enamel torii
- small green foliage accents
- dark red or muted gold cord

Avoid creating a full photographic scene inside the bookmark.


---

## Example 3 — Mount Fuji

### Input
Scenic image:
- Mount Fuji
- pale sky
- lake
- cherry blossoms

Location:
`MOUNT FUJI`

Country / region:
`JAPAN`

### Palette
- mist blue
- snow white
- muted sakura pink
- lake blue
- champagne gold

### Bookmark
- slim metal cutout
- Fuji silhouette
- small sakura enamel detail
- reflective lake line
- soft blue or dusty pink cord


---

## Example 4 — Jiufen

### Input
Scenic image:
- hillside old street
- red lanterns
- layered buildings
- mist

Location:
`JIUFEN`

Country / region:
`TAIWAN`

### Palette
- pale blue-gray
- brick red
- warm amber
- stone gray
- antique brass

### Bookmark
- warm brushed-brass structure
- simplified hillside building layers
- tiny red enamel lanterns
- mist-line engraving
- deep burgundy cord


---

# Prompt example

```text
Create a 3:4 vertical Japanese-style travel souvenir poster.

LOCATION NAME:
OTARU CANAL

COUNTRY / REGION:
HOKKAIDO, JAPAN

MUST-PRESERVE SCENIC FEATURES:
blue-roof warehouse, canal, stone building, small boat

BOOKMARK MATERIAL:
brushed metal with enamel details

Use the uploaded scenic image as Image A.
Use the uploaded metal bookmark photo as Image B style reference.

Left side: preserve the scenic identity of Otaru Canal.
Right side: create one newly designed premium metal bookmark based on the same Otaru scenery.

Use a pale mist-blue editorial background, restrained Japanese decorative motifs, and elegant typography.
```

## Example 5 — Moss Stream with a Real Bookmark Reference

### Input
Scenic image:
- clear shallow woodland stream
- small cascading waterfall
- moss-covered rocks
- bare slender trees
- scattered snow
- wooden footbridge at the far left

Product reference:
- one slim rectangular metal bookmark selected from a photo showing three bookmarks
- brushed silver frame
- blue braided cord
- openwork / enamel construction

Style / layout reference:
- pale-blue Japanese editorial poster
- left scenery / right bookmark split
- calm premium souvenir finish

Test labels:
`MOSS STREAM` and `HOKKAIDO, JAPAN`

### Stability parameters

- Canvas: `3:4`
- Split: `60% scenery / 40% bookmark`
- Products: `1 bookmark / 1 cord`
- Scenic facts preserved: `5`
- Japanese poetic phrase: `off`
- Extra text: `none`
- Bookmark treatment: `brushed silver + blue enamel + moss-green relief`

### Expected composition

Left: the supplied stream remains recognizable, with the cascades and mossy rocks as the anchor.

Right: one centered, manufacturable silver bookmark translates the stream into simplified water, rock, branch, and cascade motifs. The three-bookmark reference must not become three products in the output.
