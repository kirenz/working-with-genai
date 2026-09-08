# Folien für Working with GenAI

Buch zuerst. Ein Deck pro Lektion, in derselben Verzeichnisstruktur wie das zugehörige Buchkapitel. Inhalte aus dem fertigen Kapitel didaktisch verdichten; keine bloße Absatzkopie. Ergänzungen zuerst im Buch festhalten. Sprecherhinweise machen die Folien für die Durchführung nutzbar.

- Reveal.js-Quellen, Konfiguration aus `_quarto.yml`. Deck-Frontmatter: title, subtitle (Modul und Lektion), book-source (relativer Buchpfad). Keine neuen Plugins voraussetzen.
- Die Länge folgt dem Lernziel. Eine kurze Grundlagen- oder Orientierungslektion darf ein kurzes Deck bekommen; 7–10 Folien sind keine Pflicht. Eine Aussage oder Aufgabe je Folie, verständliche Titel. Für Grundlagen eignen sich Erklärung und kommentiertes Beispiel; für Praxis unter anderem ein sichtbares Ergebnis, Gegenüberstellung, geführter Auftrag und anschließende Auswertung. Keine Arbeitsphase oder Portfolio-Folie ohne entsprechenden Zweck.
- Sichtbarer Text indirekt/unpersönlich; bei nötiger Ansprache Sie. Sprecherhinweise ebenfalls indirekt, mit konkreter Moderation, Zeit und erwarteten Antworten. Keine Wir/Du-Anrede außerhalb von kopierbaren Prompts.
- Zu jeder inhaltlichen Folie `::: {.notes}` mit vollständigen Hinweisen, nicht nur Stichworten. Bei Live-Demo Schritte und Auffangweg bei fehlendem Konto nennen. Keine noch nicht vorhandenen Videos verlinken.
- Quelllinks konkret dort, wo produkt- oder rechtsbezogene Aussagen vorkommen; keine erfundenen Zitate. Beispielantworten als konstruiert kennzeichnen.
- Diagramme als einfache Mermaid-Flows oder native Tabellen/Spalten. Bestehende Bilder unter ../../images/ verwenden; keine Bildplatzhalter und keine neuen Personenporträts.
- Vorhandene Klassen: .stage, .kicker, .two-col, .card, .accent, .small, .sources. Zudem Quarto .columns/.column, .fragment und .notes. Keine neuen CSS-Abhängigkeiten erfinden.
- Übungen ohne Zusatzkauf; Varianten als optional markieren. Lernstoff darf anspruchsvoll sein, Bedienung bleibt geführt.
- Nutzer hat die ausführliche gemeinsame Durchsicht auf später verschoben. Bei einer beauftragten Veröffentlichung genügen gezielte Inhalts- und Zuordnungsprüfungen, ein Renderlauf und die notwendigen Veröffentlichungskontrollen. Die Freigabe muss den jeweiligen Veröffentlichungsumfang abdecken.
