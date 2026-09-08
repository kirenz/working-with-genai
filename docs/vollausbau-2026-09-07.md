# Vollausbau Working with GenAI

## Auftrag und Arbeitsgrenzen

Alle übrigen Lektionen sowie Folien und Selbstlernmaterialien für KI-Einsteiger ausarbeiten. Rösterei Morgenrot als gemeinsamer Fall, vorhandene Trainings Frech, VWA und SiMa.ai als Ausgangspunkt. Nutzer wünscht Fable 5.1 für die gemeinsame Ausarbeitung und ausdrücklich keine umfangreichen Tests; die Durchsicht erfolgt später gemeinsam.

Ausschließlich lokale Ausarbeitung. Kein Commit/Push, kein neuer Produktionsimport, keine Freischaltungen oder Nachrichten. Die vorhandenen produktiven Inhalte bleiben unverändert. Der einmalige Startpaket-Importer ist nicht für eine Aktualisierung des bereits genutzten Kurses einzusetzen.

## Umfang

Die Dateizuordnung steht in `docs/kursmanifest.json`. Die Kursübersicht verbindet Buch und Folien. Neben den Modulen ergänzen Lernweg, Werkzeugkompass, freiwillige Arbeitsagenten-Vertiefung, Portfolio und Lehrleitfaden die Durchführung.

Drei externe Fable-5.1-Arbeitspakete übernehmen Module 1–2, 3–4 und 5–6. Schreibbereiche wurden getrennt; gemeinsame Navigation, Gestaltung, Kursmanifest und Lehrdurchführung liegen bei Codex. Vorhandene Firmenmaterialien sind ausschließlich Quellen für die didaktische Anpassung. Betriebsdaten und Zugänge gehören nicht ins GenAI-Material.

Das Sitzungslimit wurde während dieser Ausarbeitung erreicht. Die drei CLI-Abschlüsse bestätigen `claude-fable-5-1` als Hauptmodell und nennen 23:10 Uhr (Europe/Berlin) als Freigabezeit. Die Fortsetzung wurde bis dahin pausiert. Zu diesem Zeitpunkt lagen alle Buchkapitel und Materialien vor. Ab 23:10 Uhr übernehmen getrennte Opus-5-Aufträge die noch fehlende Übertragung in Units und Folien; die fertigen Buchtexte bleiben dabei bestehen. Zusatzcredits oder API-Abrechnung wurden nicht aktiviert.

## Didaktische Entscheidungen

- Erster Erfolg vor einer längeren Einführung in Modelle und Produkte.
- Ein durchgehender Fall mit bekannten Personen; eigenes berufliches Vorhaben parallel im selben Portfolio.
- Geführte Kernaufträge mit vollständigem synthetischem Material; eigener Transfer erst danach.
- Unterschiedliche Tätigkeiten in der Selbstlernphase: auswählen, reparieren, Quellen zuordnen, begründen, vergleichen, ein Artefakt erstellen.
- Konstruiertes Vergleichsmaterial für fehlende Konten und Nutzungslimits; keine erfundenen Live-Ergebnisse.
- Moderner Arbeitsschwerpunkt: Kontext und Quellen, Recherche, wiederverwendbare Anweisungen, begrenzte Arbeitsagenten und ein geführter Automatisierungsschritt.
- Keine automatisch generierten Zusatzübungen, kein automatisches fachliches Urteil über Portfolio-Freitexte.
- Kein Pflicht-Abo und keine eigene kostenpflichtige API. n8n-Zugang und zentraler Modellschritt bleiben vorbereitungsbedürftig.

## Erzeugung und Grenzen

Keine Unitvalidatoren, automatisierten Tests oder Browserprüfung des Vollausbaus beauftragt. Die späteren Ansichtsdateien werden einmal erzeugt; ein erfolgreicher Build belegt keine didaktische Eignung, korrekte Quizbewertung oder funktionierende individuellen Konten.

Das Opus-Paket für Module 1–2 berichtet zusätzlich einen begrenzten eigenen Skriptcheck von Feldlängen, ID-Referenzen und Score-Bändern seiner neuen Units. Dies war kein Plattform-Testlauf oder Import; eine umfassende Validierung und die gemeinsame Durchsicht stehen weiterhin aus.

Das Opus-Paket für Module 5–6 berichtet lediglich JSON-Lesbarkeit und Fenced-Div-Balance seiner Decks. Bei der Integration wurde sein konkreter Hinweis auf die widersprüchlichen Angaben zu kostenlosen Claude Projects aufgenommen: Kapitel 6.1 formuliert den Zugang nun kontobedingt und behält die vollständige Startnachricht als Ersatzweg bei.

Offen bleiben gemeinsame Inhaltsdurchsicht, praktische Durchläufe der Übungen, finale Zeiteinteilung anhand der Gruppe, Prüfungsorganisation, n8n-Kurszugang, etwaige kurze Videoaufnahmen und ein gesonderter Release. Quellenstand und bekannte Widersprüche sind in `docs/quellen-und-wiederverwendung.md` dokumentiert.

## Abschluss der Autorenschaft

Alle drei Opus-Folgeaufträge endeten ohne Fehler; ihre CLI-Abschlüsse bestätigen `claude-opus-5` als tatsächliches Modell. Lokal vorhanden sind 18 reguläre Buchlektionen, ein zusätzlicher freiwilliger Arbeitsagenten-Pfad, 19 Foliensätze und 18 Plattform-Units. Dazu kommen Lernweg, Werkzeugkompass, Kursübersicht, Arbeitsmaterialien als ZIP, Portfolio und Lehrleitfaden. Die Zuordnung ist im Kursmanifest und in der Buchnavigation eingetragen.

Die Zeitangaben der Foliensätze sind Moderationsoptionen, keine zusätzliche verpflichtende Präsenzzeit. Die gemeinsame Durchsicht muss insbesondere die Arbeitsphasen in Modul 4 mit dem vorgesehenen Selbststudium abstimmen. Der Hauptpfad bleibt im 30-Stunden-Plan; die Durchführbarkeit der Planungswerte ist noch nicht praktisch erprobt.

## Lokale Ansichten erzeugt

Buch-HTML und alle 19 Reveal.js-Decks wurden erfolgreich erzeugt. Beim ersten Folienlauf zeigte sich eine Ausgabezuordnung außerhalb des Buchordners; deshalb wurde ein eigenständiges Folienprojekt unter `slides/_quarto.yml` eingerichtet. Die Kursübersicht und Rückverweise verwenden nun HTML-Ziele. Nach dieser konkreten Korrektur wurden nur die Kursübersicht und das Folienprojekt erneut erzeugt. Keine Unitvalidatoren, Plattformtests oder Browserdurchsicht angeschlossen.

Einstieg für die lokale Durchsicht: `_book/kursuebersicht.html`; der lokale HTTP-Server wird auf 127.0.0.1:4332 mit diesem Buchordner gestartet. Der Server ist eine Vorschau, keine Veröffentlichung.
