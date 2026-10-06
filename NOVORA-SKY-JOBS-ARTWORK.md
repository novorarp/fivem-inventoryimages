# Novora Sky-Jobs-Itembilder

Am 06.10.2026 wurden sieben fehlende Motive für die neuen Items von Sky DOJ, Sky Jobs Base und Sky Fire Job erzeugt. Das bereits vorhandene Bild `images/printer_paper.png` wurde geprüft und unverändert beibehalten.

Generierungsmodus: integriertes `image_gen.imagegen`, jeweils ein neues Bild pro Item, `transparent_background: true`, ohne Referenzbilder. Die PNG-Dateien wurden unverändert aus den Generierungsergebnissen übernommen.

Format: jeweils PNG, 1254 × 1254 Pixel, RGBA mit echtem Alpha-Kanal. Motive, vollständige Darstellung, Transparenz und Dateinamen wurden geprüft. Die SHA-256-Prüfsummen der Projektdateien stimmen mit den ursprünglichen Generierungsergebnissen überein.

| Item-ID | Motiv | Bild |
| --- | --- | --- |
| `doj_document` | Justizdokument | [doj_document.png](images/doj_document.png) |
| `job_document` | Behördendokument | [job_document.png](images/job_document.png) |
| `doj_law_book` | Gesetzbuch | [doj_law_book.png](images/doj_law_book.png) |
| `sky_briefcase` | Aktenkoffer | [sky_briefcase.png](images/sky_briefcase.png) |
| `sky_case_folder` | Aktenordner | [sky_case_folder.png](images/sky_case_folder.png) |
| `printer_ink` | Druckerpatrone | [printer_ink.png](images/printer_ink.png) |
| `fire_dividing_breeching` | Schlauchverteiler | [fire_dividing_breeching.png](images/fire_dividing_breeching.png) |

## Verwendung

Die Dateinamen entsprechen den Item-IDs beziehungsweise den vorhandenen `client.image`-Einträgen in `ox_inventory/data/items.lua`. Die Bilder werden über den bestehenden Inventory-CDN geladen.

```text
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/doj_document.png
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/job_document.png
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/doj_law_book.png
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/sky_briefcase.png
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/sky_case_folder.png
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/printer_ink.png
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/fire_dividing_breeching.png
https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/printer_paper.png
```

## Prüfsummen

| Datei | SHA-256 |
| --- | --- |
| `doj_document.png` | `f82e9c28e4b0e7ef93f65e23f95fa7cbd8046f9bb1f3ee8bc418c6d9e655c42e` |
| `job_document.png` | `2fae53e61ab43824cd5576e84e2a0705366dcd7765c14e76291caca1cf86914e` |
| `doj_law_book.png` | `742e32e86bd0414d609e6c6c97e541772a08b3add80a338941cdbbc72891716f` |
| `sky_briefcase.png` | `d8ce32d9445ff530ae1fa2326ba76a20de100e631cd190dbae14d54ebc4e90db` |
| `sky_case_folder.png` | `d241a40d1f2eb0fc04aab86679fd8d49ad925081a89f6703c6e82c77c2194168` |
| `printer_ink.png` | `a97bde9f405f871dbacbb0c608657d034017abbd1bc128806f22fa9bc8613b0f` |
| `fire_dividing_breeching.png` | `9f252092c26c1c17936a1f60b5d8f97f4b8c2b32be1970851448fbd84dd9bb1c` |
| `printer_paper.png` (Bestand) | `d538379ef655c980c52936225b5b7d72c55f1ef7de5803edf29d5bee194f404b` |

## Verwendete Prompts

### Justizdokument — doj_document.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game, square composition, instantly legible at 64–128 pixels.
Style: premium realistic 3D game asset with clean coherent geometry, subtle natural material texture, restrained wear and crisp edges. Match a set of isolated realistic inventory objects.
Composition: one centered object or tightly unified object stack, three-quarter view from slightly above, slightly diagonal for depth. The complete silhouette fits within approximately 75–80 percent of the square canvas with generous transparent padding on every side.
Lighting: soft studio key light from upper left, controlled reflections and clear edge highlights so the object remains readable on a dark inventory panel.
Background: genuine transparent alpha. No environment, floor, pedestal, surrounding cast shadow, glow cloud or colored background.
Constraints: no people, hands, loose unrelated objects, text, letters, numbers, brands, logos, watermark, border around the image, particles or baked checkerboard. Do not crop any part of the subject.
Subject: A formal legal document represented by two neatly aligned sheets of thick warm ivory paper. The top sheet has a tiny balanced-scales pictogram embossed in gold near its header, subtle gray abstract horizontal rules that suggest a printed legal layout without any letters, and a prominent deep burgundy wax seal near the lower corner. A narrow dark red ribbon lies against the paper underneath the seal. Flat paper with one gently lifted corner, elegant and unmistakably a physical justice document. The seal, ribbon and sheets form one compact object.
```

### Behördendokument — job_document.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game, square composition, instantly legible at 64–128 pixels.
Style: premium realistic 3D game asset with clean coherent geometry, subtle natural material texture, restrained wear and crisp edges. Match a set of isolated realistic inventory objects.
Composition: one centered object or tightly unified object stack, three-quarter view from slightly above, slightly diagonal for depth. The complete silhouette fits within approximately 75–80 percent of the square canvas with generous transparent padding on every side.
Lighting: soft studio key light from upper left, controlled reflections and clear edge highlights so the object remains readable on a dark inventory panel.
Background: genuine transparent alpha. No environment, floor, pedestal, surrounding cast shadow, glow cloud or colored background.
Constraints: no people, hands, loose unrelated objects, text, letters, numbers, brands, logos, watermark, border around the image, particles or baked checkerboard. Do not crop any part of the subject.
Subject: A single official employment or registry certificate on crisp light cream paper, with a restrained thin warm orange ornamental line near its edge, an abstract round blue-gray stamp near the bottom and a small silver paper clip on the upper corner. A clear hierarchy of short gray horizontal rules suggests printed form fields, but there are no actual letters, words or numbers. Mostly white paper and orange accents; no wax seal and no ribbon. A slightly curled lower corner gives the sheet realistic thickness. One compact physical certificate.
```

### Gesetzbuch — doj_law_book.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game, square composition, instantly legible at 64–128 pixels.
Style: premium realistic 3D game asset with clean coherent geometry, subtle natural material texture, restrained wear and crisp edges. Match a set of isolated realistic inventory objects.
Composition: one centered object or tightly unified object stack, three-quarter view from slightly above, slightly diagonal for depth. The complete silhouette fits within approximately 75–80 percent of the square canvas with generous transparent padding on every side.
Lighting: soft studio key light from upper left, controlled reflections and clear edge highlights so the object remains readable on a dark inventory panel.
Background: genuine transparent alpha. No environment, floor, pedestal, surrounding cast shadow, glow cloud or colored background.
Constraints: no people, hands, loose unrelated objects, text, letters, numbers, brands, logos, watermark, border around the image, particles or baked checkerboard. Do not crop any part of the subject.
Subject: One substantial closed legal reference book with dark burgundy leather covers, a sturdy spine, subtly gilded cream page edges and a simple embossed gold balance-scales pictogram centered on the front cover. No title, writing or lettering anywhere. A thin deep red bookmark ribbon barely emerges between the pages. Visibly a single closed hardcover law book, with the front cover and page block both clearly visible in a diagonal three-quarter view.
```

### Aktenkoffer — sky_briefcase.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game, square composition, instantly legible at 64–128 pixels.
Style: premium realistic 3D game asset with clean coherent geometry, subtle natural material texture, restrained wear and crisp edges. Match a set of isolated realistic inventory objects.
Composition: one centered object or tightly unified object stack, three-quarter view from slightly above, slightly diagonal for depth. The complete silhouette fits within approximately 75–80 percent of the square canvas with generous transparent padding on every side.
Lighting: soft studio key light from upper left, controlled reflections and clear edge highlights so the object remains readable on a dark inventory panel.
Background: genuine transparent alpha. No environment, floor, pedestal, surrounding cast shadow, glow cloud or colored background.
Constraints: no people, hands, loose unrelated objects, text, letters, numbers, brands, logos, watermark, border around the image, particles or baked checkerboard. Do not crop any part of the subject.
Subject: One closed compact charcoal-black leather lawyer's briefcase, a traditional hard-sided rectangular case with rounded corners, a sturdy arched carry handle, two understated brushed brass clasps, narrow edge piping and subtle leather grain. Warm hardware highlights, crisp clean silhouette and realistic depth. Front and top edge visible together, the handle completely visible. No labels, monograms, badges, accessories or contents.
```

### Aktenordner — sky_case_folder.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game, square composition, instantly legible at 64–128 pixels.
Style: premium realistic 3D game asset with clean coherent geometry, subtle natural material texture, restrained wear and crisp edges. Match a set of isolated realistic inventory objects.
Composition: one centered object or tightly unified object stack, three-quarter view from slightly above, slightly diagonal for depth. The complete silhouette fits within approximately 75–80 percent of the square canvas with generous transparent padding on every side.
Lighting: soft studio key light from upper left, controlled reflections and clear edge highlights so the object remains readable on a dark inventory panel.
Background: genuine transparent alpha. No environment, floor, pedestal, surrounding cast shadow, glow cloud or colored background.
Constraints: no people, hands, loose unrelated objects, text, letters, numbers, brands, logos, watermark, border around the image, particles or baked checkerboard. Do not crop any part of the subject.
Subject: One slim warm ochre kraft-paper case file folder, slightly open so a few neatly stacked cream documents are visible inside. An obvious index tab on the upper edge and one small dark metal binder clip make it recognizable as an organized case folder. The front is plain kraft card with only two short subtle gray abstract rules, no writing. Clean readable folder silhouette, visible folded spine and paper layers, modest natural cardboard texture. No bookbinding, no wax seal, no additional loose papers.
```

### Druckerpatrone — printer_ink.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game, square composition, instantly legible at 64–128 pixels.
Style: premium realistic 3D game asset with clean coherent geometry, subtle natural material texture, restrained wear and crisp edges. Match a set of isolated realistic inventory objects.
Composition: one centered object or tightly unified object stack, three-quarter view from slightly above, slightly diagonal for depth. The complete silhouette fits within approximately 75–80 percent of the square canvas with generous transparent padding on every side.
Lighting: soft studio key light from upper left, controlled reflections and clear edge highlights so the object remains readable on a dark inventory panel.
Background: genuine transparent alpha. No environment, floor, pedestal, surrounding cast shadow, glow cloud or colored background.
Constraints: no people, hands, loose unrelated objects, text, letters, numbers, brands, logos, watermark, border around the image, particles or baked checkerboard. Do not crop any part of the subject.
Subject: One generic compact black plastic printer ink cartridge, with a stepped rectangular body, a small exposed strip of copper contacts on one side and a narrow muted cyan-magenta-yellow color indicator on its top label. No lettering or numbers on the label. Slightly satin plastic, rounded molded edges, a clearly recognizable cartridge silhouette and restrained highlights. Show its front, side contacts and top in a clean three-quarter view. No printer, packaging, spills or loose parts.
```

### Schlauchverteiler — fire_dividing_breeching.png

```text
Use case: stylized-concept.
Asset type: a single transparent PNG inventory item icon for a FiveM roleplay game, square composition, instantly legible at 64–128 pixels.
Style: premium realistic 3D game asset with clean coherent geometry, subtle natural material texture, restrained wear and crisp edges. Match a set of isolated realistic inventory objects.
Composition: one centered object or tightly unified object stack, three-quarter view from slightly above, slightly diagonal for depth. The complete silhouette fits within approximately 75–80 percent of the square canvas with generous transparent padding on every side.
Lighting: soft studio key light from upper left, controlled reflections and clear edge highlights so the object remains readable on a dark inventory panel.
Background: genuine transparent alpha. No environment, floor, pedestal, surrounding cast shadow, glow cloud or colored background.
Constraints: no people, hands, loose unrelated objects, text, letters, numbers, brands, logos, watermark, border around the image, particles or baked checkerboard. Do not crop any part of the subject.
Subject: One compact professional firefighting three-way hose dividing breeching manifold. A red-painted cast-metal body branches from ONE large rear inlet into exactly THREE forward hose outlets: one central outlet and one angled side outlet on each side. The inlet and three outlets have sturdy silver aluminum Storz-style coupling rims, and three black short valve levers sit on the red body. The camera is above and in front at a three-quarter angle so the three forward outlets and the large rear inlet are distinguishable. Realistic clean firefighting equipment, restrained wear, strong red-and-silver silhouette. No hoses connected, no water, no extra outlets, no labels and no detached parts.
```
