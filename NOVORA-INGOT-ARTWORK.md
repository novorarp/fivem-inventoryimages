# Novora Barren-Itembilder

Die vier Motive wurden am 05.10.2026 mit dem integrierten OpenAI-Imagegen-Tool für die bestehenden Barren-Items in `ox_inventory/data/items.lua` erzeugt. Jedes Metall besitzt ein eigenes Motiv mit einheitlicher Perspektive und deutlich unterscheidbarer Oberfläche.

Generierungsmodus: `image_gen.imagegen`, jeweils ein neues Bild pro Item, `transparent_background: true`, ohne Referenzbilder. Die generierten PNG-Dateien wurden unverändert übernommen.

Format: jeweils PNG, 1254 × 1254 Pixel, RGBA mit echtem Alpha-Kanal. Transparenz, vollständige Darstellung und Dateinamen wurden geprüft. Die SHA-256-Prüfsummen der Projektdateien stimmen mit den jeweiligen Generierungsergebnissen überein.

| Item-ID | Deutsches Label | Bild |
| --- | --- | --- |
| `silver_ingot` | Silberbarren | [silver_ingot.png](images/silver_ingot.png) |
| `iron_ingot` | Eisenbarren | [iron_ingot.png](images/iron_ingot.png) |
| `copper_ingot` | Kupferbarren | [copper_ingot.png](images/copper_ingot.png) |
| `gold_ingot` | Goldbarren | [gold_ingot.png](images/gold_ingot.png) |

## Verwendung

Die Dateinamen entsprechen exakt den englischen Item-IDs. `ox_inventory` lädt die Bilder über die bestehende Bildadresse; in den Itemdefinitionen ist kein zusätzlicher `client.image`-Eintrag erforderlich:

```text
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/<itemname>.png
```

## Verwendete Prompts

### Silberbarren — silver_ingot.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game. Square composition, designed to remain immediately legible at 64–128 pixels.
Subject and composition: exactly one solid cast metal ingot, a classic long trapezoidal bullion bar with a slightly smaller rectangular top, sloped sides, and softly beveled edges. Three-quarter view from above. Its long axis runs diagonally from lower left to upper right, with its front short end at lower left and a long side visible on the lower right. Center the entire object with even transparent padding; it occupies approximately 80 percent of the square canvas. Do not crop any part.
Style: premium realistic 3D game inventory asset, clean readable silhouette, restrained fine metal grain, believable weight and thickness. No pedestal, no decorative elements.
Lighting: soft studio key light from upper left, controlled metal reflections, darker side face for volume, crisp readable bevels, balanced exposure. The object must read well on both light and dark inventory panels.
Background: genuine transparent alpha, with no floor, no environment, no background color, and no surrounding shadow or glow cloud.
Constraints: one bar only, no text, no letters, no numbers, no stamps, no inscriptions, no logos, no watermark, no frame, no particles, no checkerboard baked into the pixels.
Material: bright cool-white silver, subtly polished and brushed, luminous pale silver top with neutral cool gray sides. Clearly a SILVER bullion ingot, brighter and more polished than iron, with no golden or copper tint.
```

### Eisenbarren — iron_ingot.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game. Square composition, designed to remain immediately legible at 64–128 pixels.
Subject and composition: exactly one solid cast metal ingot, a classic long trapezoidal bullion bar with a slightly smaller rectangular top, sloped sides, and softly beveled edges. Three-quarter view from above. Its long axis runs diagonally from lower left to upper right, with its front short end at lower left and a long side visible on the lower right. Center the entire object with even transparent padding; it occupies approximately 80 percent of the square canvas. Do not crop any part.
Style: premium realistic 3D game inventory asset, clean readable silhouette, restrained fine metal grain, believable weight and thickness. No pedestal, no decorative elements.
Lighting: soft studio key light from upper left, controlled metal reflections, darker side face for volume, crisp readable bevels, balanced exposure. The object must read well on both light and dark inventory panels.
Background: genuine transparent alpha, with no floor, no environment, no background color, and no surrounding shadow or glow cloud.
Constraints: one bar only, no text, no letters, no numbers, no stamps, no inscriptions, no logos, no watermark, no frame, no particles, no checkerboard baked into the pixels.
Material: dark charcoal-gray iron, mostly matte cast metal with subtle fine grain and muted steel highlights. Clearly an IRON ingot, substantially darker and less reflective than silver. Neutral gray only, not black, not gold, no red rust.
```

### Kupferbarren — copper_ingot.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game. Square composition, designed to remain immediately legible at 64–128 pixels.
Subject and composition: exactly one solid cast metal ingot, a classic long trapezoidal bullion bar with a slightly smaller rectangular top, sloped sides, and softly beveled edges. Three-quarter view from above. Its long axis runs diagonally from lower left to upper right, with its front short end at lower left and a long side visible on the lower right. Center the entire object with even transparent padding; it occupies approximately 80 percent of the square canvas. Do not crop any part.
Style: premium realistic 3D game inventory asset, clean readable silhouette, restrained fine metal grain, believable weight and thickness. No pedestal, no decorative elements.
Lighting: soft studio key light from upper left, controlled metal reflections, darker side face for volume, crisp readable bevels, balanced exposure. The object must read well on both light and dark inventory panels.
Background: genuine transparent alpha, with no floor, no environment, no background color, and no surrounding shadow or glow cloud.
Constraints: one bar only, no text, no letters, no numbers, no stamps, no inscriptions, no logos, no watermark, no frame, no particles, no checkerboard baked into the pixels.
Material: warm reddish-orange copper, satin metallic finish with rich reddish-brown shadowed sides and clean pale copper edge highlights. Clearly a COPPER ingot, recognizably redder and browner than gold. No verdigris, no green corrosion.
```

### Goldbarren — gold_ingot.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game. Square composition, designed to remain immediately legible at 64–128 pixels.
Subject and composition: exactly one solid cast metal ingot, a classic long trapezoidal bullion bar with a slightly smaller rectangular top, sloped sides, and softly beveled edges. Three-quarter view from above. Its long axis runs diagonally from lower left to upper right, with its front short end at lower left and a long side visible on the lower right. Center the entire object with even transparent padding; it occupies approximately 80 percent of the square canvas. Do not crop any part.
Style: premium realistic 3D game inventory asset, clean readable silhouette, restrained fine metal grain, believable weight and thickness. No pedestal, no decorative elements.
Lighting: soft studio key light from upper left, controlled metal reflections, darker side face for volume, crisp readable bevels, balanced exposure. The object must read well on both light and dark inventory panels.
Background: genuine transparent alpha, with no floor, no environment, no background color, and no surrounding shadow or glow cloud.
Constraints: one bar only, no text, no letters, no numbers, no stamps, no inscriptions, no logos, no watermark, no frame, no particles, no checkerboard baked into the pixels.
Material: rich yellow-gold bullion, warm polished satin metallic finish, clean luminous golden upper face, deeper amber-gold side faces. Clearly a GOLD ingot, more yellow than copper. Restrained luxurious highlights, not orange painted plastic.
```
