# Novora Waffenteile-Itembilder

Die drei Motive wurden am 06.10.2026 mit dem integrierten OpenAI-Imagegen-Tool für die bestehenden Crafting-Items in `ox_inventory/data/items.lua` erzeugt. Lauf, Griff und leeres Magazin werden als einzelne, freigestellte Komponenten dargestellt.

Generierungsmodus: `image_gen.imagegen`, jeweils ein neues Bild pro Item, `transparent_background: true`, ohne Referenzbilder. Die PNG-Dateien wurden unverändert aus den Generierungsergebnissen übernommen.

Format: jeweils PNG, 1254 × 1254 Pixel, RGBA mit echtem Alpha-Kanal. Transparenz, vollständige Darstellung und exakte Dateinamen wurden geprüft. Die SHA-256-Prüfsummen der Projektdateien stimmen mit den ursprünglichen Generierungsergebnissen überein.

| Item-ID | Deutsches Label | Bild |
| --- | --- | --- |
| `barrel` | Lauf | [barrel.png](images/barrel.png) |
| `grip` | Griff | [grip.png](images/grip.png) |
| `magazine` | Magazin | [magazine.png](images/magazine.png) |

## Verwendung

Die Dateinamen entsprechen den Item-IDs. Das Inventar kann die Bilder über die bestehende CDN-Adresse laden; zusätzliche Bildzuweisungen in den Itemdefinitionen sind nicht nötig.

```text
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/barrel.png
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/grip.png
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/magazine.png
```

## Verwendete Prompts

### Lauf — barrel.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for Novora FiveM roleplay. Square composition, designed to be clearly readable at 64–128 pixels.
Style: premium realistic 3D game inventory asset, clean geometry, believable material texture, crisp silhouette, restrained surface wear. An isolated game crafting component, not a technical drawing.
Composition: a three-quarter view, centered with comfortable transparent padding on every side. Fully visible, no cropped edges. The object occupies approximately 78 percent of the square canvas.
Lighting: soft studio lighting from upper left, controlled highlights along edges, enough contrast for a dark inventory UI.
Background: genuine transparent alpha, no colored background, no floor, no environment, no shadow cloud or glow.
Constraints: exactly one separate component, no complete firearm, no hands, no ammunition, no diagrams, no measurements, no text, no labels, no numbers, no logos, no watermark, no frame, no particles, no baked checkerboard.
Subject: one generic detached firearm barrel represented as a simple game crafting item. A dark brushed gunmetal steel cylindrical tube with a slightly wider base section and a visible dark circular opening at its front tip. Diagonally arranged from lower left to upper right, front tip at lower left. Subtle silver-gray edge highlights define the cylindrical form. Compact readable proportions, a clean sturdy silhouette, visually recognizable as a weapon barrel rather than an industrial pipe. No extra attachments, no suppressor, no additional loose parts, no cutaway or internal detail.
```

### Griff — grip.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for Novora FiveM roleplay. Square composition, designed to be clearly readable at 64–128 pixels.
Style: premium realistic 3D game inventory asset, clean geometry, believable material texture, crisp silhouette, restrained surface wear. An isolated game crafting component, not a technical drawing.
Composition: a three-quarter view, centered with comfortable transparent padding on every side. Fully visible, no cropped edges. The object occupies approximately 78 percent of the square canvas.
Lighting: soft studio lighting from upper left, controlled highlights along edges, enough contrast for a dark inventory UI.
Background: genuine transparent alpha, no colored background, no floor, no environment, no shadow cloud or glow.
Constraints: exactly one separate component, no complete firearm, no hands, no ammunition, no diagrams, no measurements, no text, no labels, no numbers, no logos, no watermark, no frame, no particles, no baked checkerboard.
Subject: one generic detached pistol-style weapon handgrip represented as a simple game crafting item. A compact standalone ergonomic grip with a gently angled profile, rounded back, subtle finger contour and finely stippled charcoal-black polymer surface. Three-quarter view exposes the front and a side, mounting end toward upper right, base toward lower left. Soft graphite-gray highlights clearly separate the edges from a dark UI. Show only the handle itself, no receiver, trigger, trigger guard, magazine, rail or other parts. Clean robust silhouette, believable molded rubber and polymer texture.
```

### Magazin — magazine.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for Novora FiveM roleplay. Square composition, designed to be clearly readable at 64–128 pixels.
Style: premium realistic 3D game inventory asset, clean geometry, believable material texture, crisp silhouette, restrained surface wear. An isolated game crafting component, not a technical drawing.
Composition: a three-quarter view, centered with comfortable transparent padding on every side. Fully visible, no cropped edges. The object occupies approximately 78 percent of the square canvas.
Lighting: soft studio lighting from upper left, controlled highlights along edges, enough contrast for a dark inventory UI.
Background: genuine transparent alpha, no colored background, no floor, no environment, no shadow cloud or glow.
Constraints: exactly one separate component, no complete firearm, no hands, no ammunition, no diagrams, no measurements, no text, no labels, no numbers, no logos, no watermark, no frame, no particles, no baked checkerboard.
Subject: one EMPTY detachable pistol-style firearm magazine represented as a simple game crafting item. A dark graphite-gray satin steel rectangular magazine body, subtly tapered at the top, with a small black polymer base plate and restrained stamped side indentations. The top opening is clearly empty: no cartridges or bullets anywhere. Three-quarter view exposing a broad side and the narrow front edge, long axis diagonally from lower left to upper right, base plate at lower left and open top at upper right. Soft steel-gray highlights reveal its shape against a dark UI. Clean compact silhouette and modest surface wear. No complete gun, no separate loose pieces, no letters, numbers or serial markings.
```
