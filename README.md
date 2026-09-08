# Working with GenAI

Vollständig ausgearbeitete Kursquellen für das Microcredential: sechs Module mit 31 Pflichtlektionen sowie eine freiwillige Vertiefung, 30 Stunden. Durchgehender Lehrfall ist die Rösterei Morgenrot. Grundlagen und Anwendungen sind einzeln über die Navigation erreichbar.

## Zum Durchgehen

- `index.qmd`: Buchstart mit Fall und Team.
- `lernweg.qmd`: Termine, Arbeitsrhythmus und Zwischenstände.
- `kursuebersicht.qmd`: alle Kapitel und ihre Folien.
- `werkzeugkompass.qmd`: Orientierung zwischen Chat, Recherche, Projekten und Arbeitsagenten.
- `praxis/codex-claude-code.qmd`: frühe Demo und freiwilliger Praxispfad.
- `material/`: komplette synthetische Übungsunterlagen, Prompts und Arbeitsblätter, unterteilt nach Modulen.
- `slides/`: ein Reveal.js-Deck pro Lektion plus Arbeitsagenten-Demo, mit Sprecherhinweisen.
- `docs/lehrleitfaden.md`: Auftakt, Beratungen, Recap und Vorbereitung.

Die 32 Plattform-Units liegen in `hdm/lernplattform/apps/api/app/db/units/working-with-genai`. Ihre Zuordnung zu Buch, Folien und Lektionen steht in `docs/kursmanifest.json`. Die 18 bereits veröffentlichten Lektionen behalten ihre Slugs und Datenbankkennungen.

## Arbeitsweise

Buch zuerst, daraus Folien und interaktive Lernschritte. Buch in Wir-Form oder neutral, deutsche Folien und Plattformtexte ohne direkte Leseransprache. Materialien und eigene Fälle bleiben synthetisch. Die Musterantworten sind als konstruiert gekennzeichnet; es werden keine Live-Modellläufe behauptet.

Der Pflichtpfad erfordert keinen Zusatzkauf, keine eigene API und keine Installation. Funktionsabhängige Übungen haben einen Text- oder Kursbeispiel-Fallback. Für n8n werden Kursinstanz und zentrales Modell-Credential organisatorisch vorbereitet; diese Einrichtung ist noch nicht erfolgt.

## Bauen und ansehen

```sh
quarto render
quarto render slides
```

Die HTML-Dateien liegen unter `_book/`. Die Kursübersicht verbindet Kapitel und Folien. Ein Browser über einen lokalen HTTP-Server zeigt sie mit den zugehörigen Ressourcen an.

## Gemeinsame Durchsicht steht aus

Die v3-Entwürfe wurden mit Fable 5.1 und Opus 5 über das vorhandene Claude-Max-Login ausgearbeitet. Nach Erreichen des Sitzungslimits beauftragte der Nutzer Codex ausdrücklich mit der Fertigstellung und erlaubte OpenAI-Subagenten. Codex führt die Materialien zusammen, korrigiert konkrete fachliche Befunde und veröffentlicht den abgestimmten Umfang.

Der Nutzer hat die ausführliche gemeinsame Durchsicht auf später verschoben. Zur Veröffentlichung gehören deshalb gezielte Inhalts-, Zuordnungs- und Unitprüfungen, der Buch-/Folien-Build und die notwendigen Sicherungen des Produktionsimports. Diese Prüfungen ersetzen keine vollständige didaktische Abnahme.

Quellen und Wiederverwendung: `docs/quellen-und-wiederverwendung.md` sowie die Modulnotizen unter `docs/authoring/`. Die Inhalte nutzen didaktische Bausteine aus Frech, VWA und SiMa.ai; deren betriebliche Daten und Zugänge werden nicht mitgenommen.

## Veröffentlichung zur gemeinsamen Durchsicht

Die Veröffentlichung dieser Arbeitsfassung wurde am 08.09.2026 beauftragt. Buch und Folien erscheinen auf GitHub Pages; die interaktiven Lektionen auf der kommerziellen Instanz. Der Kurs ist seit dem 08.09.2026 auch im öffentlichen Kurskatalog sichtbar. Die gemeinsame didaktische Durchsicht steht weiterhin aus. Kursimporte erhalten bestehende IDs, Quizversuche und Lernfortschritte; der einmalige Startpaket-Importer ist für diese Aktualisierung nicht geeignet.

- [Interaktiver Kurs](https://kurse.kirenz.de/courses/working-with-genai)
- [Buch und Folien](https://kirenz.github.io/working-with-genai/kursuebersicht.html)

Ziel bleibt `kurse.kirenz.de`, Kurs-Slug `working-with-genai`, `simulator_enabled=false`. Keine KI-generierten Zusatzübungen.

© Jan Kirenz, 2026.
