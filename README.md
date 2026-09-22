# 🖼️ Novara Inventory Images

## Kleidungsitems für ox_inventory

Die 14 neuen `images/clothing_*.png` decken Kopfbedeckung, Maske, Brille, Ohrringe, Oberteil, Unterhemd, Arme/Handschuhe, Hose, Schuhe, Tasche, Kette, Weste, Uhr und Armband ab. Herkunft und Generierung stehen in [NOVARA-CLOTHING-ARTWORK.md](NOVARA-CLOTHING-ARTWORK.md).

Das Inventar lädt `https://raw.githubusercontent.com/novorarp/fivem-inventoryimages/main/images/<itemname>.png`. Für bestehende ox-IDs gilt der exakte Name einschließlich Groß-/Kleinschreibung und Bindestrichen: `WEAPON_PISTOL.png`, `ammo-9.png`. Diese Kompatibilitätsfälle sind Ausnahmen von der allgemeinen Namenskonvention unten. Neue Kleidungs-IDs verwenden `clothing_<category>`.

Das Inventar lädt die Bilder im Spiel über die CDN-URL dieses Repositories. Die lokale Browser-Vorschau verwendet gebündelte Kopien derselben Assets.

> Die zentrale Bildbibliothek für Inventory-Items von **Novara**.

Dieses Repository sammelt und verwaltet die Grafiken, die für Items in unseren Inventar-Systemen verwendet werden. Eine einheitliche Benennung sorgt dafür, dass jedes Bild zuverlässig über seine Item-ID gefunden werden kann.

## 📁 Aufbau

```text
novara_inventoryimages/
├── images/
│   ├── apple.png
│   ├── first_aid_kit.png
│   ├── items_to_download.json
│   └── sources.json
└── README.md
```

| Datei / Ordner | Beschreibung |
| --- | --- |
| `images/` | Enthält alle Inventory-Bilder und die zugehörigen Metadaten. |
| `images/items_to_download.json` | Liste von Items, für die Bilder vorbereitet oder beschafft werden sollen. |
| `images/sources.json` | Dokumentiert Bildquelle, Lizenz und Attribution, sofern vorhanden. |

## 🚨 Verbindliche Namensregeln

Der Dateiname eines Bildes muss immer der **englischen Item-ID beziehungsweise dem englischen Item-Namen** entsprechen.

### ✅ Erlaubt

- ausschließlich englische Begriffe
- nur Kleinbuchstaben (`a-z`)
- Zahlen (`0-9`), falls sie Teil der Item-ID sind
- Unterstriche (`_`) als einzige Worttrenner
- die Dateiendung `.png` in Kleinbuchstaben
- exakt ein Bild pro Item-ID

### ❌ Nicht erlaubt

- deutsche oder anderssprachige Bezeichnungen
- Leerzeichen
- Bindestriche (`-`) oder andere Worttrenner
- Großbuchstaben
- Umlaute, Sonderzeichen oder Akzente
- zusätzliche Zusätze, die nicht zur Item-ID gehören

Die gültige Form lässt sich so zusammenfassen:

```regex
^[a-z0-9]+(?:_[a-z0-9]+)*\.png$
```

## 📝 Beispiele

| Item-ID / englischer Name | ✅ Richtiger Dateiname | ❌ Falscher Dateiname |
| --- | --- | --- |
| `apple` | `apple.png` | `Apfel.png` |
| `water_bottle` | `water_bottle.png` | `water bottle.png` |
| `first_aid_kit` | `first_aid_kit.png` | `first-aid-kit.png` |
| `weapon_pistol` | `weapon_pistol.png` | `WEAPON_PISTOL.PNG` |
| `radio_2` | `radio_2.png` | `Radio 2.png` |

> **Merksatz:** Wenn die Item-ID `first_aid_kit` lautet, muss das Bild `first_aid_kit.png` heißen.

Falls nur ein englischer Anzeigename vorhanden ist, wird dieser in `snake_case` umgewandelt:

```text
First Aid Kit  →  first_aid_kit.png
Water Bottle   →  water_bottle.png
Access Card    →  access_card.png
```

Wenn Item-ID und Anzeigename voneinander abweichen, hat die **Item-ID Vorrang**, da sie vom Inventory technisch für die Bildzuordnung verwendet wird.

## 🎨 Anforderungen an Bilder

- Format: **PNG**
- ein quadratisches Seitenverhältnis wird empfohlen
- ein transparenter Hintergrund wird empfohlen
- das Item sollte mittig, vollständig und gut erkennbar dargestellt sein
- unnötige Ränder, Wasserzeichen und eingebettete Texte vermeiden
- Bilder vor dem Hinzufügen sinnvoll komprimieren, ohne sichtbaren Qualitätsverlust

## ➕ Neues Bild hinzufügen

1. Englische Item-ID im verwendeten Inventory prüfen.
2. Bild als PNG vorbereiten.
3. Dateinamen exakt aus der Item-ID übernehmen.
4. Leerzeichen und andere Trenner durch Unterstriche ersetzen.
5. Datei in `images/` ablegen.
6. Falls erforderlich, Quelle und Lizenz in `images/sources.json` dokumentieren.
7. Prüfen, ob das Bild im Inventory korrekt geladen und dargestellt wird.

Beispiel für einen Eintrag in `sources.json`:

```json
{
  "id": "first_aid_kit",
  "title": "First Aid Kit",
  "file": "first_aid_kit.png",
  "source": "https://example.com/source",
  "license": "License name",
  "attribution": "Creator name"
}
```

Dabei müssen `id` und `file` zusammenpassen:

```text
id:   first_aid_kit
file: first_aid_kit.png
```

## 🔍 Checkliste vor dem Commit

- [ ] Ist die Item-ID beziehungsweise der Item-Name englisch?
- [ ] Entspricht der Dateiname exakt der Item-ID?
- [ ] Ist der Dateiname vollständig kleingeschrieben?
- [ ] Werden ausschließlich Unterstriche als Worttrenner verwendet?
- [ ] Enthält der Dateiname keine Leerzeichen, Bindestriche oder Sonderzeichen?
- [ ] Ist die Dateiendung `.png` kleingeschrieben?
- [ ] Ist das Motiv sauber freigestellt, zentriert und gut erkennbar?
- [ ] Wurden Quelle und Lizenz dokumentiert, sofern dies erforderlich ist?
- [ ] Wurde die Darstellung im Inventory getestet?

## 🧹 Umgang mit bestehenden Altdateien

Im Bilderbestand können noch ältere Dateien vorhanden sein, deren Namen nicht diesen Regeln entsprechen. Sie gelten **nicht als Vorlage** für neue Bilder.

Neue oder überarbeitete Assets müssen immer die Regeln dieser README erfüllen. Bestehende Dateien dürfen nur zusammen mit allen dazugehörigen Item-Verweisen umbenannt werden, damit keine Bilder im Inventory fehlen.

## ⚖️ Bildrechte

Füge nur Bilder hinzu, die verwendet und weitergegeben werden dürfen. Bei externen Quellen müssen Lizenz, Urheber und Quelle korrekt in `images/sources.json` eingetragen werden. Bilder mit unklaren Nutzungsrechten gehören nicht in das Repository.

---

💙 **Einheitliche Namen bedeuten weniger Fehler, leichteres Suchen und ein saubereres Inventory.**
