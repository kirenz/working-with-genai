# Working with GenAI

Vollständig ausgearbeitete Kursquellen für das Microcredential: sechs Module, 18 Lektionen, 30 Stunden. Durchgehender Fall ist die Rösterei Morgenrot mit den aus Business Analytics übernommenen Personen und Bildern.

## Zum Durchgehen

- `index.qmd`: Buchstart mit Fall und Team.
- `lernweg.qmd`: Termine, Arbeitsrhythmus und Zwischenstände.
- `kursuebersicht.qmd`: alle Kapitel und ihre Folien.
- `werkzeugkompass.qmd`: Orientierung zwischen Chat, Recherche, Projekten und Arbeitsagenten.
- `praxis/codex-claude-code.qmd`: frühe Demo und freiwilliger Praxispfad.
- `material/`: komplette synthetische Übungsunterlagen, Prompts und Arbeitsblätter, unterteilt nach Modulen.
- `slides/`: ein Reveal.js-Deck pro Lektion plus Arbeitsagenten-Demo, mit Sprecherhinweisen.
- `docs/lehrleitfaden.md`: Auftakt, Beratungen, Recap und Vorbereitung.

Die 18 Plattform-Units liegen in `hdm/lernplattform/apps/api/app/db/units/working-with-genai`. Ihre Zuordnung zu Buch, Folien und geplanten Lektionen steht in `docs/kursmanifest.json`. Die bestehende veröffentlichte Lektion behält ihren Slug `arbeitsauftrag`.

## Arbeitsweise

Buch zuerst, daraus Folien und interaktive Lernschritte. Buch in Wir-Form, deutsche Folien und Plattformtexte indirekt oder mit Sie. Materialien und eigene Fälle bleiben synthetisch. Die Musterantworten sind als konstruiert gekennzeichnet; es werden keine Live-Modellläufe behauptet.

Der Pflichtpfad erfordert keinen Zusatzkauf, keine eigene API und keine Installation. Funktionsabhängige Übungen haben einen Text- oder Kursbeispiel-Fallback. Für n8n werden Kursinstanz und zentrales Modell-Credential organisatorisch vorbereitet; diese Einrichtung ist noch nicht erfolgt.

## Bauen und ansehen

```sh
quarto render
quarto render slides
```

Die HTML-Dateien liegen unter `_book/`. Die Kursübersicht verbindet Kapitel und Folien. Ein Browser über einen lokalen HTTP-Server zeigt sie mit den zugehörigen Ressourcen an.

## Gemeinsame Durchsicht steht aus

Die Buchausarbeitung erfolgte in drei getrennten Fable-5.1-Arbeitspaketen über die lokale Claude-Code-CLI. Nach einer Sitzungspause übernahm Opus 5 die verbleibende Übertragung in Units und Folien; Codex integrierte die Ergebnisse. Nutzerwunsch: keine umfangreichen Prüfungen. Daher keine Unitvalidatoren, umfassenden Testläufe oder Browserprüfung des Vollausbaus. Begrenzte Feld- und Referenzprüfungen durch die Arbeitsagenten sind im Übergabebericht festgehalten. Ein Erzeugungslauf für die Ansichtsdateien ist keine didaktische oder technische Abnahme.

Quellen und Wiederverwendung: `docs/quellen-und-wiederverwendung.md` sowie die Modulnotizen unter `docs/authoring/`. Die Inhalte nutzen didaktische Bausteine aus Frech, VWA und SiMa.ai; deren betriebliche Daten und Zugänge werden nicht mitgenommen.

## Veröffentlichung zur gemeinsamen Durchsicht

Die Veröffentlichung dieser Arbeitsfassung wurde am 08.09.2026 beauftragt. Buch und Folien erscheinen auf GitHub Pages; die interaktiven Lektionen auf der kommerziellen Instanz. Der Kurs bleibt über seinen direkten Link zugänglich und wird nicht neu im Katalog gelistet. Die gemeinsame didaktische Durchsicht steht weiterhin aus. Kursimporte erhalten bestehende IDs, Quizversuche und Lernfortschritte; der einmalige Startpaket-Importer ist für diese Aktualisierung nicht geeignet.

- [Interaktiver Kurs](https://kurse.kirenz.de/courses/working-with-genai)
- [Buch und Folien](https://kirenz.github.io/working-with-genai/kursuebersicht.html)

Ziel bleibt `kurse.kirenz.de`, Kurs-Slug `working-with-genai`, `simulator_enabled=false`. Keine KI-generierten Zusatzübungen.

© Jan Kirenz, 2026.
