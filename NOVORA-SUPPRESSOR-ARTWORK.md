# Novora Schalldämpfer-Itembilder

Die beiden Motive wurden am 06.10.2026 mit dem integrierten OpenAI-Imagegen-Tool für die Komponenten `at_suppressor_light` und `at_suppressor_heavy` in `ox_inventory/data/weapons.lua` erzeugt. Die leichte Variante besitzt eine schlanke, glatte Form, die schwere eine breitere Form mit Ringen.

Generierungsmodus: `image_gen.imagegen`, jeweils ein neues Bild pro Item, `transparent_background: true`, ohne Referenzbilder. Die PNG-Dateien wurden unverändert aus den Generierungsergebnissen übernommen.

Format: jeweils PNG, 1254 × 1254 Pixel, RGBA mit echtem Alpha-Kanal. Transparenz, vollständige Darstellung und Dateinamen wurden geprüft. Die SHA-256-Prüfsummen der Projektdateien stimmen mit den ursprünglichen Generierungsergebnissen überein.

| Item-ID | Motiv | Bild |
| --- | --- | --- |
| `at_suppressor_light` | Leichter Schalldämpfer | [at_suppressor_light.png](images/at_suppressor_light.png) |
| `at_suppressor_heavy` | Schwerer Schalldämpfer | [at_suppressor_heavy.png](images/at_suppressor_heavy.png) |

## Verwendung

`ox_inventory/data/weapons.lua` verweist im jeweiligen `client.image` auf die passende neue PNG-Datei. Dadurch zeigen beide Komponenten ihre eigenen Motive. Für bestehende Installationen die aktualisierte `data/weapons.lua` übernehmen und die Resource neu laden.

CDN-Adressen:

```text
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/at_suppressor_light.png
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/at_suppressor_heavy.png
```

## Verwendete Prompts

### Leichter Schalldämpfer — at_suppressor_light.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay video game. Square composition, instantly legible at 64–128 pixels.
Style: premium realistic 3D game asset matching an inventory set of dark metal weapon components. A fictional external game prop, not a diagram or technical illustration. Clean coherent geometry, restrained fine surface texture, modest wear, crisp readable silhouette.
Composition: exactly one isolated object in three-quarter view from above, diagonally oriented from lower left to upper right. Front circular end toward lower left, rear mounting end toward upper right. The entire object is centered with generous transparent padding on all sides, occupying approximately 75–80 percent of the canvas. No clipped edges.
Lighting: soft studio key light from upper left, controlled graphite and silver-gray reflections along the surface and rim. Readable on a dark inventory panel.
Background: genuine transparent alpha, no environment, no floor, no pedestal, no colored background, no surrounding shadow or glow cloud.
Constraints: external appearance only, no cutaway, no interior detail, no dimensions, no assembly instructions, no complete firearm, no other objects, no ammunition, no hands, no text, no letters, no numbers, no logos, no watermark, no frame, no particles, no baked checkerboard.
Subject: one compact, lightweight pistol-style suppressor as a fictional weapon attachment icon. A slim, short, straight cylindrical tube with a smooth satin dark gunmetal finish, subtle narrow end collars, and a simple round front face with a small dark opening. Minimal clean design. Emphasize a light and narrow silhouette with soft steel-gray rim highlights. The rear end is understated with no exposed internal mechanism. No extra attachments or loose parts.
```

### Schwerer Schalldämpfer — at_suppressor_heavy.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay video game. Square composition, instantly legible at 64–128 pixels.
Style: premium realistic 3D game asset matching an inventory set of dark metal weapon components. A fictional external game prop, not a diagram or technical illustration. Clean coherent geometry, restrained fine surface texture, modest wear, crisp readable silhouette.
Composition: exactly one isolated object in three-quarter view from above, diagonally oriented from lower left to upper right. Front circular end toward lower left, rear mounting end toward upper right. The entire object is centered with generous transparent padding on all sides, occupying approximately 75–80 percent of the canvas. No clipped edges.
Lighting: soft studio key light from upper left, controlled graphite and silver-gray reflections along the surface and rim. Readable on a dark inventory panel.
Background: genuine transparent alpha, no environment, no floor, no pedestal, no colored background, no surrounding shadow or glow cloud.
Constraints: external appearance only, no cutaway, no interior detail, no dimensions, no assembly instructions, no complete firearm, no other objects, no ammunition, no hands, no text, no letters, no numbers, no logos, no watermark, no frame, no particles, no baked checkerboard.
Subject: one heavy tactical rifle-style suppressor as a fictional weapon attachment icon. A robust, visibly broader and longer cylindrical body in dark charcoal-gray matte metal, with a few broad shallow circumferential bands and a slightly thicker rear collar to make it visually distinct from a slim smooth pistol suppressor. Simple round front face with a small dark opening, subdued brushed steel-gray highlights, sturdy clearly defined silhouette. Restrained surface texture, not heavily distressed. No exposed internal mechanism, no extra attachments or loose parts.
```
