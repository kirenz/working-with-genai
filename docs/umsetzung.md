# Vollausbau: aktuelle Arbeitsfassung

Stand 07.09.2026. Alle 18 Lektionen, zugehörige Folien und Units sowie die freiwillige Arbeitsagenten-Vertiefung lokal ausgearbeitet. Gemeinsame Durchsicht auf Nutzerwunsch noch offen. Kein neuer Commit, Push oder Produktionsimport. Der frühere Veröffentlichungsbericht unten beschreibt ausschließlich das damalige Startpaket. Der aktuelle Umfang und Erzeugungsstand stehen in `docs/vollausbau-2026-09-07.md`.

---

# Startpaket: Working with GenAI

## Aktueller Änderungsstand: Fallumstellung auf die Rösterei Morgenrot (07.09.2026)

**Nur lokal.** Der durchgehende Lehrfall ist von der eigens erfundenen Nordwerk Elektrowerkzeuge GmbH auf die Rösterei Morgenrot aus dem Business-Analytics-Kurs umgestellt. Übernommen sind Ausgangslage (kleine Rösterei im Direktvertrieb, Onlineshop und Kaffee-Abo, drei Sorten, Wachstum ohne Gewinn 2025), Sortiment mit Listenpreisen, die fünf handelnden Personen mit ihren Funktionen und die vorhandenen Bilder. Neu für diesen Kurs und im Material gekennzeichnet: die Arbeitsanlässe der fünf Personen, die Kundenanfrage an Sina Bergmann und die Abo-Regel zum Sortenwechsel (fünf Werktage vor dem Versand). Am Business-Analytics-Repo wurde nichts geändert.

Geänderte Dateien in diesem Repo: `index.qmd`, `prompting/arbeitsauftrag.qmd`, `material/lehrfall-fachinformationen.txt`, `material/kundenanfrage.txt`, `material/prompt-vorlage.txt`, `material/portfolio-vorlage.md`, `docs/kurskonzept-v2.md`, `README.md`, diese Datei. Neu hinzugekommen: `material/roesterei-morgenrot.md`, `docs/roesterei-morgenrot-fallbasis.md`, `images/`. In der Lernplattform: `apps/api/app/db/units/working-with-genai/02-01-arbeitsauftrag.unit.json` — Aufbau unverändert bei zwölf Blöcken, elf Lernschritten und drei Quizfragen; Block-, Option- und Item-IDs sind erhalten, der Inhalt ist umgestellt.

**Prüfungen ausgesetzt.** Auf ausdrücklichen Nutzerwunsch wurden zu dieser Änderung keine Tests, kein `quarto render`, keine Unit-Validierung, keine Browserprüfung und keine gesonderten Reviews ausgeführt. Sie sind auf später verschoben. Der Abschnitt „Prüfungen" weiter unten beschreibt den Stand vor der Fallumstellung und wird nicht rückwirkend umgeschrieben.

**Öffentlich weiterhin Nordwerk.** Buch auf GitHub Pages und Musterlektion auf kurse.kirenz.de zeigen unverändert den vorherigen Lehrfall. Es wurde nichts committet, gepusht, deployt oder importiert.

Offen: Render, Unit-Validierung, Durchsicht durch Jan, danach Entscheidung über Release und Plattformimport. Beim Import sind die vorhandenen IDs und Lernfortschritte der bereits veröffentlichten Musterlektion zu erhalten.

---

## Stand des Startpakets vor der Fallumstellung

Stand: 07.09.2026. Konzept v2 und Musterlektion 2.1 fertig ausgearbeitet. Die übrigen 17 Lektionen sind geplant, aber noch nicht erstellt. Die Veröffentlichung von Buch und Musterlektion sowie Commit und Push wurden am 07.09.2026 ausdrücklich freigegeben. Die nachfolgend dokumentierten Inhaltsprüfungen beziehen sich auf den lokalen Stand vor der Veröffentlichung.

## Ergebnis

- `docs/kurskonzept-v2.md`: sechs Module mit 18 Lektionen, 30 Stunden (4 + 20 + 6), Portfolio-Zuordnung und Meilensteine zu den realen Terminen.
- `prompting/arbeitsauftrag.qmd`: vollständiges Musterkapitel mit synthetischem Lehrfall, kopierbarem Prompt, konstruiertem Ergebnis, Prüfkriterien und eigener Variante.
- `material/`: Fachinformationen, Kundenanfrage, identischer Prompt und Portfolio-Vorlage mit den vier offiziellen Bestandteilen.
- `_quarto.yml`, `index.qmd`, `book-theme.scss`, `AGENTS.md`, `README.md`, `.gitignore`: lokale Buchgrundlage. Theme aus dem eigenen n8n-Grundlagen-Buch übernommen.
- Plattform-Unit: `/Users/jankirenz/code/hdm/lernplattform/apps/api/app/db/units/working-with-genai/02-01-arbeitsauftrag.unit.json`, zwölf Blöcke in elf Lernschritten, drei feste Quizfragen und eine Auftragskarte.

Ziel bleibt `kurse.kirenz.de`, Slug `working-with-genai`. Beim Anlegen `simulator_enabled=false` setzen. Dieser vorhandene Schalter deaktiviert KI-generierte Zusatzübungen; keine neue Plattformfunktion erforderlich. Der Kurs wird zunächst unlisted angelegt und über den direkten Link bereitgestellt.

## Ausarbeitung und Review

Opus 5 hat das Startpaket über die lokale Claude-Code-CLI erstellt. Fable 5.1 prüfte unabhängig einen Snapshot der Unit. Angefordert und in den Antwortmetadaten bestätigt: `claude-opus-5` und `claude-fable-5-1`, bestehendes Claude-Max-Login. Codex prüfte Buch, Konzept und Unit und integrierte die Befunde.

Die erste Opus-Sitzung konnte aufgrund fehlender Arbeitsverzeichnisfreigaben nur die Unit erstellen. Nach expliziter Einbindung des bereits autorisierten Buchverzeichnisses wurden die übrigen Dateien fertiggestellt.

Wesentliche Korrekturen:

- Risikofrage statt sicherer Vorhersage einer Halluzination; unbelegte Häufigkeitsbehauptungen entfernt.
- Allgemeines Modellwissen von den für diesen Fall zugelassenen Belegen getrennt.
- Keine starre Ein-Verb-Regel; klares Ergebnis als didaktische Hilfe.
- Drei dokumentierte Durchläufe einschließlich unveränderter Wiederholung. Unterschiede sind Beobachtungen, kein kausaler Wirksamkeitsnachweis. Fables weitergehende Empfehlung, größere Unterschiede als kausal zuzuschreiben, wurde ausdrücklich nicht übernommen.
- Konkreter Check der Garantiebedingung und aller zusätzlichen Aussagen.
- Eigene Übung mit synthetischen Angaben; bloße Namensersetzung ist keine Freigabe interner Unterlagen.
- Widget-Rückmeldung ausschließlich zu Auswahlentscheidungen; keine Einsatzfreigabe oder automatische fachliche Freitextbewertung. Bänder 0–4, 5 und 6 unterscheiden verbleibende Auswahlprobleme.
- Auftragskarte in Portfolio-Teil 2 integriert; Materialherkunft und tatsächliches Material unterschieden. Übernahme in die Arbeitsmappe ausdrücklich per Kopieren.
- Umlaute vereinheitlicht; derselbe vollständige Prompt steht in Unit, Buch und Download.

## Prüfungen

- `quarto render` mit Quarto 1.8.27: erfolgreich, zwei Buchseiten, keine Renderwarnungen.
- `uv run python scripts/validate_unit.py app/db/units/working-with-genai/02-01-arbeitsauftrag.unit.json` im Plattformverzeichnis `apps/api`: bestanden.
- Tatsächlicher Plattform-Scorer: richtige und falsche Antworten für Multiple Choice, Klassifikation und Fehlerdiagnose geprüft.
- Buch, Unit und Prompt-Download auf identischen Promptinhalt abgeglichen.
- Vier Materialdownloads, Konzeptdownload und Buchkapitel lokal mit HTTP 200 geprüft.
- Echte React-Kurskomponenten in einer isolierten Vorschau: Quizabgabe, Weiter/Zurück, wiederhergestellter richtiger Versuch nach Reload und Auftragskarte geprüft. Rückmeldung bei fünf Punkten bleibt neutral, erst sechs Punkte bestätigen passende Auswahlentscheidungen, ohne fachliche Freigabe.
- Buch bei 1280 und 390 Pixeln visuell geprüft. Mobile Buchseite und Kurs-Widget ohne horizontalen Seitenüberlauf. Screenshots unter `lernplattform/output/playwright/genai-*`.
- Inhaltsdateien und Unit auf Format-/Whitespaceprobleme geprüft.

Eine zu frühe UI-Testabfrage las das Feedback noch vor dem abgeschlossenen Rendern. Die Folgeprüfungen warten ausdrücklich auf die sichtbare Rückmeldung. Kein Plattformfehler daraus abgeleitet.

## Vorschau und Grenzen

Während dieser Sitzung:

- Buch: http://127.0.0.1:4332/prompting/arbeitsauftrag.html
- Interaktive Unit: http://127.0.0.1:4330/

Das Buch kann jederzeit mit `quarto render` gebaut und mit einem lokalen HTTP-Server aus `_book/` geöffnet werden. Die isolierte Unit-Vorschau unter `/tmp/genai-preview` ist ein temporäres Prüfwerkzeug mit echten Komponenten, normalisierten Pydantic-Payloads und dem echten Scorer, aber ohne reguläre Konten oder Kursdatenbank. Sie verwendet eine Ersatzschrift. Quizversuche leben nur im lokalen Vorschauprozess, Widget-Eingaben im Browser. Login, regulärer Lernfortschritt, Mentor und Produktionsbetrieb wurden nicht getestet. Ein Live-Durchlauf des Prompts im kostenlosen ChatGPT-Konto und eine Erprobung mit Einsteigern stehen aus. Die Beispielantwort ist ausdrücklich konstruiert.

Die lokalen Browser melden lediglich ein fehlendes Favicon; das ist kein Inhalts- oder Anwendungsfehler. Alte Vorschaufehler vom Start vor Fertigstellung der Unit betreffen nicht den fertigen Stand.

## Folgender Umfang

1. Den Auftakt mit Modul 1 und die übrigen Lektionen ausarbeiten; Buch und Unit zusammen prüfen.
2. Freiwilligen Codex-/Claude-Code-Pfad und die frühe Demo vorbereiten. Aktuelle Zugänge, Preise und Limits vor Kursbeginn verifizieren.
3. n8n-Kurszugänge und gegebenenfalls zentralen Modellzugang für die geführte Bauübung vorbereiten; keine persönlichen API-Kosten voraussetzen.
4. Bewertungsform und organisatorischen Abgabeweg vor Kursbeginn festlegen. Kurze individuelle Rückmeldungen vor den beiden Beratungen einplanen.
5. Wenige gezielte Screen-Demos ergänzen; Textpfad bleibt vollständig bearbeitbar.
6. Freigegebenen Release durchführen und Produktionsprüfungen separat in der Lernplattform dokumentieren.

## Veröffentlichungsziele

- Buch: https://kirenz.github.io/working-with-genai/
- Musterkapitel: https://kirenz.github.io/working-with-genai/prompting/arbeitsauftrag.html
- Kurs: https://kurse.kirenz.de/courses/working-with-genai

Die CI veröffentlicht das Buch bei Änderungen auf `main`. Der Plattformimport bleibt ein eigener, ausdrücklich freizugebender Vorgang.
