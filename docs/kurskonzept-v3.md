# Working with GenAI: Grundlagen, Anwendung und eigene Use Cases

Konzeptstand vom 08.09.2026, gemeinsam mit Claude Fable 5.1 diskutiert und durch Codex integriert. Der Nutzer hat anschließend die vollständige Umsetzung und Veröffentlichung beauftragt. Die folgende Darstellung dokumentiert die Entscheidungen für v3; die konkrete Zuordnung der ausgearbeiteten Quellen steht in `kursmanifest.json`.

Diese Fassung ersetzt für die weitere Ausarbeitung die Festlegung auf drei Lektionen je Modul und das einheitliche Übungsmuster aus v2. Der organisatorische Rahmen bleibt bestehen: sechs Module, 1 ECTS, 30 Stunden, vier Portfolio-Teile und die vorgesehenen Termine.

## Ziel und Zuschnitt

Der Kurs vermittelt, wie generative KI bei beruflichen Aufgaben sinnvoll eingesetzt wird. Dazu gehören das Verstehen grundlegender Konzepte, das Finden geeigneter Anwendungsfälle, die Formulierung von Aufträgen, die Arbeit mit Informationen und die Beurteilung von Ergebnissen. Die Zielgruppe benötigt weder KI-Vorwissen noch Programmierkenntnisse. Vertrieb und Marketing sind zwei von mehreren Anwendungsbereichen.

Grundlagen erhalten eigene, auffindbare Einträge in der Seitenleiste. Die Titel nennen das gesuchte Thema ausdrücklich, etwa Prompting, Halluzinationen oder Kontextfenster. Ein Thema bekommt eine eigene Lektion, wenn es ein eigenständiges Lernziel trägt und später gezielt nachgeschlagen werden soll. Kleine Erläuterungen zu einem einzelnen Arbeitsschritt bleiben bei diesem Schritt.

Die Rösterei Morgenrot verbindet die Anwendungen. Kurze zusätzliche Beispiele aus anderen Arbeitsbereichen zeigen den Transfer, etwa Besprechungsnotizen strukturieren, Tabellen vergleichen oder Ideen entwickeln. Nicht jede Seite verlangt einen neuen Chat, eine eigene Variante und einen Portfolio-Eintrag.

## Was wir vom SiMa.ai-Kurs übernehmen

Maßgebliches Vorbild ist die Plattformgliederung in `hdm/lernplattform/apps/api/app/db/seed_claude_sima.py`, insbesondere die Abschnitte „Claude in chat“ und „Projects“. Die älteren Referenzseiten im SiMa.ai-Workshop sind nicht die maßgebliche aktuelle Kursnavigation.

Der Seed dokumentiert zwei passende Entscheidungen: „Lead research“ wurde aus „Writing good prompts“ herausgelöst, damit die Anwendung wiedergefunden werden kann. Zwei Einstiegsübungen mit demselben Zweck wurden zusammengeführt. Die Units `07-chat-good-prompts.unit.json` und `10-projects-first-project.unit.json` zeigen außerdem, dass eine Lektion unterschiedlich umfangreich sein darf.

Übernommen werden diese Regeln für den Zuschnitt. Die Ausrichtung auf Vertrieb und Marketing sowie produktspezifische Einrichtungsschritte werden nicht zum Curriculum dieses Grundlagenkurses. Die SiMa.ai-Quellen und der parallel überarbeitete Claude-Kurs bleiben unverändert.

## Die geplante Seitenleiste

31 Pflichtlektionen in sechs Modulen sowie eine freiwillige Vertiefung. Die Zahl ergibt sich aus den Themen; sie ist keine Vorgabe für spätere Ergänzungen. Die Typen in den Tabellen dienen der Redaktion und sind keine zusätzlichen Navigationsebenen.

### 1. Generative KI verstehen und Anwendungsfälle finden

| Nr. | Sichtbarer Titel | Schwerpunkt |
|---|---|---|
| 1.1 | Willkommen und Orientierung | Kursziel, Arbeitsweise, Morgenrot und Portfolio kennenlernen. |
| 1.2 | Wie generative KI arbeitet | Sprachmodell, Trainingswissen, mitgegebener Kontext und Werkzeugabruf verständlich einordnen; unterschiedliche Antworten auf gleiche Aufträge erklären. |
| 1.3 | ChatGPT, Claude und Gemini im Überblick | Werkzeuge für Aufgaben einordnen; früher Einblick in Work, Cowork, Codex und Claude Code. |
| 1.4 | Vom Briefing zum Entwurf | Einen vorgegebenen Auftrag bearbeiten, das Ergebnis überarbeiten und gegen die Angaben prüfen. |
| 1.5 | Welche Daten dürfen ins KI-Werkzeug? | Übungsdaten, betriebliche Angaben und offene Freigaben unterscheiden. |
| 1.6 | Halluzinationen und Unsicherheit | Plausibilität, Quellenstütze und sachliche Richtigkeit unterscheiden; unbelegte Produktangaben untersuchen. |
| 1.7 | Use Cases im Arbeitsalltag finden | Tätigkeiten und Engpässe erfassen, Arbeitsschritte zerlegen und mögliche Unterstützung ableiten. |
| 1.8 | Use Cases bewerten und priorisieren | Nutzen, Machbarkeit, Aufwand und Risiken vergleichen; KI und andere Lösungswege abwägen. |
| 1.9 | Den Pilotfall im Use-Case-Canvas festhalten | Einen begrenzten Fall mit Ausgangslage, Erfolgskriterium, Datenbedarf und Zuständigkeit beschreiben. |

Vor der ersten Eingabe gilt bereits die kurze Regel, ausschließlich das bereitgestellte erfundene Material zu verwenden. Die ausführliche Datenlektion vertieft diese Orientierung. Die Agentendemo findet früh im Auftakt statt; eigene Installation oder Nutzung bleibt freiwillig.

### 2. Prompting und Zusammenarbeit im Dialog

| Nr. | Sichtbarer Titel | Schwerpunkt |
|---|---|---|
| 2.1 | Prompting: Task, Context, Format und Check | Die vier Teile und ihren jeweiligen Beitrag an kurzen kommentierten Beispielen verstehen. |
| 2.2 | Einen Arbeitsauftrag für eine Kundenanfrage formulieren | Die vier Teile auf Sinas Anfrage anwenden und den Entwurf prüfen. |
| 2.3 | Mit Beispielen und Format steuern | Ergebnisform vorgeben, Beispiele nutzen und unerwünschte Übernahmen erkennen. |
| 2.4 | Im Dialog weiterarbeiten | Rückfragen, gezielte Überarbeitung und Vergleich von Varianten einsetzen. |

Die vier Teile bilden die gemeinsame Arbeitsweise dieses Kurses. Sie werden nicht als universell vorgeschriebener Standard dargestellt. Der Check im Prompt und die anschließende menschliche Prüfung bleiben zwei unterschiedliche Schritte.

### 3. Kontext, Dokumente und Recherche

| Nr. | Sichtbarer Titel | Schwerpunkt |
|---|---|---|
| 3.1 | Chatverlauf und Kontextfenster | Verstehen, welche Informationen im aktuellen Auftrag berücksichtigt werden können; Token nur so weit erklären, wie sie zum Verständnis der Begrenzung beitragen. |
| 3.2 | Passende Materialien auswählen | Relevanz, Version und Verwendungszweck von Dokumenten prüfen. |
| 3.3 | Prompt Injection: Anweisungen in Dokumenten | Fremde Aufforderungen in Material erkennen und von eigenen Arbeitsaufträgen unterscheiden. |
| 3.4 | Regeln und Quellen in einer Kontextmappe festhalten | Eine versionierte, vom Werkzeug unabhängige Arbeitsgrundlage erstellen. |
| 3.5 | Fundstellen in langen Dokumenten nutzen | Passagen suchen, im Zusammenhang lesen und gezielt bereitstellen; Abruf und Antwort unterscheiden. |
| 3.6 | Websuche und Quellen prüfen | Den bereits vorhandenen Rechercheauftrag mit Quellen, Aktualität und offenen Fragen bearbeiten. |

Die Websuche erhält einen eigenen Menüpunkt, weil sie unter „Wenn das Material zu groß wird“ schwer auffindbar ist. Der bestehende Rechercheauftrag wird verlagert und nicht als zusätzliche Übung verdoppelt. RAG wird als Prinzip des Suchens relevanter Passagen eingeordnet; eine Architekturlektion ist nicht vorgesehen.

### 4. Ergebnisse beurteilen und verbessern

| Nr. | Sichtbarer Titel | Schwerpunkt |
|---|---|---|
| 4.1 | Was ein gutes KI-Ergebnis ausmacht | Kriterien für Auskünfte, Zusammenfassungen, Ideen und Tabellenvergleiche unterscheiden. |
| 4.2 | Aussagen, Zahlen und Quellen prüfen | Eine Zusammenfassung prüfen und reparieren; Rechenwege, Einheiten und Bezugsgrößen anhand eines kurzen Beispiels nachvollziehen. |
| 4.3 | Mit Testfällen die Qualität prüfen | Typische Fälle, Grenzfälle und fehlende Angaben am eigenen Vorhaben untersuchen. |
| 4.4 | Einen Auftrag auf andere KI-Werkzeuge übertragen | Beobachten, was bei einem Werkzeugwechsel erhalten bleibt und erneut geprüft werden muss. |

Ein Ergebnis wird nicht allein nach der Belegbarkeit einzelner Sätze beurteilt. Je nach Aufgabe zählen beispielsweise Vollständigkeit, Brauchbarkeit, Vielfalt, nachvollziehbare Berechnungen oder die Passung zu einer Entscheidung. Enthält eine Idee Sachbehauptungen, müssen diese ebenfalls geprüft werden. Ein Anbieter-Ranking ist nicht vorgesehen.

### 5. Daten, Rechte und Verantwortung

| Nr. | Sichtbarer Titel | Schwerpunkt |
|---|---|---|
| 5.1 | Datenschutz im Arbeitsalltag | Datenbedarf und Freigaben des eigenen Vorhabens klären; frühe Datenregeln anwenden statt wiederholen. |
| 5.2 | Urheberrecht und geistiges Eigentum | Rechtefragen bei Material und Ergebnissen erkennen und Zuständigkeiten festhalten. |
| 5.3 | Verzerrungen und unfaire Ergebnisse | Wertungen und einseitige Darstellungen untersuchen; besondere Aufmerksamkeit bei Aussagen über Personen. |
| 5.4 | Verantwortung und KI-Kompetenz im Betrieb | Nutzung, menschliche Entscheidung und verbindliche Klärung im Risiko-Überblick zusammenführen. |

Rechts- und produktbezogene Einzelangaben werden bei der Ausarbeitung anhand aktueller Primärquellen geprüft. Diese Gliederung legt Lernziele fest und trifft keine neuen Rechtsaussagen.

### 6. Wiederverwenden und Arbeitsabläufe gestalten

| Nr. | Sichtbarer Titel | Schwerpunkt |
|---|---|---|
| 6.1 | Chat, Projekt, Agent oder Workflow? | Nach Aufgabe, Kontrolle, Wiederholbarkeit und Datenzugang auswählen; keine aufsteigende Stufenleiter. |
| 6.2 | Aufträge und Kontext wiederverwenden | Ein geprüftes Startpaket vorbereiten und in einer geeigneten Arbeitsumgebung einsetzen. |
| 6.3 | Einen einfachen Workflow mit n8n aufbauen | Einen begrenzten Ablauf auf der Kursinstanz geführt erproben; Ersatzweg bei fehlendem Modellzugang. |
| 6.4 | Transferplan und Kurzpräsentation | Einen nächsten betrieblichen Schritt, Erfolgskriterien und Zuständigkeiten festhalten; Portfolio vorstellen. |

Die n8n-Anwendung ist eine geführte Kurserfahrung. Eine funktionsfähige Automatisierung ist keine Voraussetzung für das Portfolio. Ergebnisse bleiben vor einer menschlichen Freigabe Entwürfe.

### Freiwillige Vertiefung, ab Kursbeginn sichtbar

**Codex und Claude Code: eine Aufgabe mit Dateien.** Die bestehende Praxisquelle wird weiterverwendet. Eigene Erprobung ersetzt einen Teil der persönlichen Transferzeit und setzt keinen zusätzlichen Pflichtaufwand voraus. Es entsteht keine neue Sektion mit weiteren Pflichtmodulen.

## Use Cases systematisch ermitteln

Die bisherige Lektion `start/anwendungsfall.qmd` enthält sechs Morgenrot-Kandidaten, fünf Eignungskriterien, die Sammlung von zwei bis drei eigenen Schreib- oder Prüfanlässen sowie einen Canvas. Das bietet eine Grundlage für die Auswahl. Eine angeleitete Suche entlang realer Tätigkeiten und ein Vergleich von Nutzen und Umsetzungsaufwand fehlen bisher. Die Beschränkung auf feste Fakten und satzweise prüfbare Texte ist für den gesamten Kurs zu eng.

Die drei neuen Menüpunkte entwickeln daraus einen zusammenhängenden Arbeitsgang:

1. **Finden:** Eine typische Arbeitswoche oder einen Vorgang betrachten. Zeitaufwand, wiederkehrende Rückfragen, Medienwechsel, Wartezeiten und Qualitätsprobleme notieren. Einen Vorgang in Eingaben, Arbeitsschritte, Ergebnis und Empfänger zerlegen. Festhalten, was heute daran nicht gut funktioniert. Daraus zwei bis drei konkrete Kandidaten ableiten, etwa Informationen vergleichen, Material strukturieren, Entwürfe erstellen oder Entscheidungen vorbereiten. Ein kurzes Interview mit KI kann dabei helfen; ein manuelles Arbeitsblatt bietet denselben Weg. Die KI fragt nach und ordnet Angaben. Sie erfindet weder Zeitersparnisse noch benötigte Werkzeugfunktionen; Zeitwerte stammen aus Beobachtungen oder werden als noch zu prüfende Annahmen der Person gekennzeichnet.
2. **Bewerten:** Zuerst offene Freigaben und ungeeignete Entscheidungsdelegation erkennen. Anschließend erwarteten Nutzen, Datenverfügbarkeit, Aufwand einschließlich Prüfung und erreichbare Ergebnisqualität vergleichen. Für eine exakt regelgebundene Aufgabe auch eine Vorlage, Tabellenfunktion oder gewöhnliche Automatisierung erwägen. Bewertungen mit einem kurzen Satz begründen. Unbekannte Größen werden als Annahmen festgehalten. Ein hoher Nutzen verrechnet keine ungeklärte Voraussetzung.
3. **Pilot festhalten:** Einen kleinen Ausschnitt auswählen. Den heutigen Ablauf und ein beobachtbares Erfolgskriterium festhalten, etwa Bearbeitungszeit einschließlich Nacharbeit, Zahl notwendiger Rückfragen oder Vollständigkeit einer Übergabe. Benennen, was die KI übernimmt und welche Entscheidung bei einer Person bleibt. Der bestehende Canvas ist weiterhin Portfolio-Teil 1; die Kandidatenliste und Priorisierungsbegründung sind dessen Arbeitsgrundlage.

Es gibt keine zusätzliche gewichtete Punkteskala und keinen zweiten Canvas. Die bisherigen Felder tragen Ausgangslage, Nutzen, Häufigkeit, Datenbedarf und Abgrenzung. Der Vergleich der Kandidaten wird als kleine vorbereitende Tabelle geführt. Eignung für einen ersten Kurspiloten und langfristiges Potenzial eines Vorhabens werden ausdrücklich unterschieden. Die Entdeckung bleibt breit, der Pilot wird klein und mit einem zur Aufgabe passenden Bewertungsmaßstab zugeschnitten. Prüfbarkeit bedeutet bei einer Ideenaufgabe etwas anderes als bei einer Auskunft nach Aktenlage.

## Lektionen gestalten

Grundlagenlektionen erklären einen Begriff oder Zusammenhang in verständlichem Fließtext und an einem kurzen Beispiel. Sie brauchen weder eine vollständige Morgenrot-Aufgabe noch einen neuen Portfolio-Eintrag. Eine Beobachtung oder unbewertete Vermutung kann den Einstieg bilden. Bewertete Wissensfragen folgen nach den benötigten Erklärungen.

Praxislektionen enthalten einen begrenzten Auftrag, geeignete Materialien, eine eigene Durchführung und erklärendes Feedback. Pro Modul wird ein zusammenhängender Beitrag zum eigenen Vorhaben bearbeitet; zusätzliche eigene Varianten sind Vertiefungen. Die Auswahl interaktiver Formate folgt dem Lernziel. Quizfragen, Diagramme und Callouts sind keine Pflichtausstattung jeder Seite.

Jede Lektion erhält ein Buchkapitel, eine verständliche Plattform-Unit und passende Folien. Das Buch bleibt die Quelle für die Ausarbeitung. Die Plattform vermittelt die Kernerklärung selbst; der Buch-Tab ist keine Voraussetzung zum Verständnis. Kurze Grundlagen dürfen kurze Decks bekommen. Die Folien sind eine alternative Darstellung, keine zusätzliche Pflichtlektüre.

## Abgrenzung zu Werkzeugkursen

Working with GenAI vermittelt die übertragbaren Konzepte und die Auswahl passender Arbeitsweisen. Kurse zu ChatGPT, Claude und Gemini übernehmen ausführliche Bedienung, Kontoeinstellungen und produktspezifische Vertiefungen. Die Werkzeugkurse müssen unabhängig nutzbar bleiben und dürfen benötigte Begriffe knapp erklären.

Die erste praktische Aufgabe enthält die unmittelbar benötigten Bedienschritte. Vertiefungsverweise führen auf eine passende Lektion statt auf einen kompletten Kurs als Voraussetzung. Nur vorhandene, geprüfte Ziele werden verlinkt. Die parallele Überarbeitung des Claude-Kurses ist nicht Teil dieses Auftrags.

## Zeitbudget und Meilensteine

Die folgenden Zeiten sind Planungsbudgets. Sie sind noch keine gemessenen Bearbeitungszeiten der neu zugeschnittenen Lektionen. Mehr Menüpunkte verteilen den Lernstoff; sie erzeugen keine zusätzlichen Stunden.

| Bestandteil | Stunden |
|---|---:|
| Präsenzauftakt | 4,0 |
| Online-Termine einschließlich Recap | 3,5 |
| Onboarding | 0,5 |
| Angeleitete asynchrone Lektionen und Übungen | 9,0 |
| Eigene Erprobung | 7,0 |
| Prüfungsdokumentation und Präsentationsvorbereitung | 6,0 |
| Gesamt | 30,0 |

### Präsenzauftakt am 18.09., 13 bis 17 Uhr

| Beginn | Minuten | Schwerpunkt |
|---|---:|---|
| 13:00 | 10 | Willkommen und Arbeitsweise |
| 13:10 | 15 | Wie generative KI arbeitet, mit einem kurzen kommentierten Beispiel |
| 13:25 | 10 | Werkzeuge einordnen |
| 13:35 | 25 | Vom Briefing zum Entwurf |
| 14:00 | 15 | Demo: Arbeit mit Dateien in Codex und Claude Code |
| 14:15 | 15 | Datenregeln für die eigene Arbeit |
| 14:30 | 20 | Halluzinationen und Unsicherheit am Beispiel |
| 14:50 | 15 | Pause |
| 15:05 | 25 | Use Cases systematisch finden; vorläufigen Kandidaten benennen |
| 15:30 | 15 | Task, Context, Format und Check |
| 15:45 | 35 | Einen Arbeitsauftrag für die Kundenanfrage bearbeiten |
| 16:20 | 25 | Beispiele und Format, gemeinsame Einführung |
| 16:45 | 15 | Arbeitsmappe, offene Fragen und Weiterarbeit |

Die Priorisierung der eigenen Kandidaten und der Canvas werden im Selbststudium abgeschlossen. Eine eigene Variante im Auftakt nutzt gegebenenfalls den vorläufigen Kandidaten; dessen Auswahl ist noch keine endgültige Entscheidung. Damit muss Modul 1 nicht mehr vollständig in den Auftakt passen. Die kurze Einführung vor der ersten Übung ersetzt keinen langen Theorievortrag und ist auch ohne Live-Termin als Lektion verständlich.

### Verteilung der neun angeleiteten Selbstlernstunden

| Modul | Minuten | Verwendung |
|---|---:|---|
| 1, verbleibender Anteil | 35 | Kandidaten bewerten und ersten Canvas festhalten |
| 2, verbleibender Anteil | 65 | Beispiele vertiefen und im Dialog weiterarbeiten |
| 3 | 120 | Kontext verstehen, Materialien und Fundstellen bearbeiten, Websuche |
| 4 | 105 | Ergebnisqualität, Quellenprüfung, Testfälle und Werkzeugübertragung |
| 5 | 90 | Daten, Rechte, Verzerrungen und Zuständigkeiten |
| 6 | 125 | Wiederverwendung, geführter Workflow und Transferentscheidung |
| Gesamt | 540 | 9 Stunden |

Raum entsteht durch das Aufteilen vorhandener Erklärungen, eine eigene Transferaufgabe pro Modul und das Kürzen doppelter Daten- und Prüfhinweise. Live bearbeitete Aufgaben werden nicht erneut als asynchrone Pflicht angesetzt. Die sieben Stunden eigene Erprobung gelten für die Weiterentwicklung des Vorhabens, nicht nochmals für die hier eingerechnete erste Canvas-Fassung. Die sechs Prüfungsstunden dienen der abschließenden Dokumentation und Präsentationsvorbereitung; der Recap zählt ausschließlich zu den Online-Terminen.

Bis zum 23.09. liegen Kandidatenvergleich, Canvas und erster Arbeitsauftrag aus Modul 1 und 2 vor. Beratung: 24.09. Bis zum 29.09. folgen Kontextquellen und erste Testfälle aus Modul 3 und 4. Beratung: 30.09. Die Inhalte aus Modul 5 und 6 sowie das Portfolio werden bis zum Recap am 08.10. abgeschlossen. Kurze individuelle Rückmeldung vor den Beratungen bleibt vorgesehen.

## Zuordnung und Umsetzung

Das aktuelle `docs/kursmanifest.json` beschreibt vorhandene Quellen. Es wird erst bei der Ausarbeitung schrittweise erweitert. Es werden keine leeren Kapitel in die Buchnavigation oder auf die Plattform eingehängt. Die Nummern oben sind redaktionelle Zielpositionen und keine neuen Datenbankkennungen.

| Bestehender Lektions-Slug | Geplanter Platz und Umgang |
|---|---|
| `willkommen` | 1.1, Orientierung verdichten; ausführlichen Werkzeugüberblick auf eigene Seite auslagern. |
| `erster-chat` | 1.4, Titel „Vom Briefing zum Entwurf“ erhalten. |
| `grenzen-daten` | 1.6, Mechanismus und Datenregeln auf eigene Grundlagen verteilen. Datenkarten sind ein gesonderter Zuordnungsfall vor späterer Veröffentlichung. |
| `anwendungsfall` | 1.9, vorhandenen Canvas und Kennungen erhalten; systematisches Finden und Priorisieren auf zwei eigene Seiten davor. |
| `arbeitsauftrag` | 2.2, die vier Teile auf einer eigenen Grundlagenlektion davor erklären. |
| `beispiele-format` | 2.3, gemeinsame Einführung und vertiefende Anwendung. |
| `iterieren` | 2.4, Titel auf Zusammenarbeit im Dialog ausrichten. |
| `material-auswaehlen` | 3.2, Dokumentauswahl; Prompt Injection in 3.3 erklären. Vor benötigter Kenntnis keine bewertete Frage dazu stellen. |
| `regeln-quellen` | 3.4, Schwerpunkt auf der werkzeugunabhängigen Kontextmappe. |
| `material-finden` | 3.5, Kontextfenster nach 3.1 und Rechercheauftrag nach 3.6 auslagern. |
| `aussagen-pruefen` | 4.2, Qualitätskriterien durch neue Grundlage 4.1 vorbereiten. |
| `testfaelle` | 4.3, bestehende Anwendung fortführen. |
| `toolvergleich` | 4.4, beobachtete Übertragbarkeit statt Anbieter-Ranking. |
| `datenschutz` | 5.1, auf eigene Datenentscheidung konzentrieren. |
| `urheberrecht` | 5.2, bestehende Aufgabe fortführen und fachlich aktualisieren. |
| `ki-kompetenz` | 5.4, Risiko-Überblick und Zuständigkeiten; neue Grundlage zu Verzerrungen in 5.3. |
| `wiederverwenden` | 6.2, Startpaket fortführen; Auswahl der Arbeitsweise als Grundlage 6.1 davor. |
| `miniworkflow` | 6.3, geführte Anwendung und Ersatzweg erhalten. |
| `transferplan` | 6.4, vier Portfolio-Teile und Kurzpräsentation zusammenführen. |

Die freiwillige Buchquelle `praxis/codex-claude-code.qmd` bleibt erhalten und bekommt bei der Ausarbeitung eine eigenständig auffindbare Plattform-Zuordnung. Der bestehende Werkzeugkompass liefert Material für 1.3; das parallele Nachschlageangebot darf keine abweichenden Angaben entwickeln.

### Bestehende Lernstände bei der späteren Veröffentlichung

Eine lokale Textänderung erfordert keinen sofortigen Datenbankimport. Die Quellen können gemeinsam überarbeitet und anschließend konsistent veröffentlicht werden. Ein zwischenzeitlicher Produktivstand mit neuem Buch und alten Units ist kein vorgeschriebener Umsetzungsschritt.

Der produktive Kurs besteht bereits. Aus dem zukünftigen Kickoff-Datum darf kein leerer Lernstand abgeleitet werden. Vor einem später beauftragten Import werden die tatsächlich vorhandenen Kennungen und Lernstände erhoben. Der ersetzende Standardimport `app.db.import_unit` ist für diese Umstrukturierung nicht der vorgesehene Weg.

Bestehende Lektionen behalten ihre Slugs und Identität. Quizfragen und Versuche werden erhalten. Ein veränderter Fragetext darf die Bedeutung eines bereits gewerteten Versuchs nicht stillschweigend verändern. Neue Grundlagen bekommen neue Kennungen. Das Herauslösen von Blöcken wird ausdrücklich zugeordnet. Insbesondere beim Datenkarten-Widget und beim Canvas ist die vollständige Speicherzuordnung zu prüfen; derselbe Storage-Key allein ist kein Nachweis für erhaltene Eingaben.

Die neue Lektion zu Datenregeln kann lokal vollständig vorbereitet werden. Ein Verschieben des bestehenden Datenkarten-Widgets erfolgt erst mit einer belegten Zuordnung seiner Daten; andernfalls bleibt es zunächst an seinem bisherigen Ort. Diese Umsetzungseinzelheit ändert das Ziel einer eigenen auffindbaren Datenlektion nicht.

### Reihenfolge der Ausarbeitung

Zuerst werden Modul 1 und die Prompting-Grundlage ausgearbeitet, einschließlich der drei Use-Case-Lektionen und ihrer Arbeitsblätter. Danach folgen Kontext und Qualität, anschließend Verantwortung und Transfer. Jeweils Buch, Material, Unit und Folien zusammenführen. Interne Anleitung und Lernweg werden danach auf die tatsächliche Navigation und Zeitverteilung abgestimmt.

Für diesen Konzeptstand genügen Zuordnungs-, Zahlen- und Textkontrolle. Umfangreiche Render-, Test- und Browserprüfungen bleiben wie besprochen der späteren gemeinsamen Durchsicht vorbehalten. Die ursprüngliche Konzeptphase umfasste keinen Release; die nachfolgende ausdrückliche Freigabe vom 08.09.2026 umfasst Umsetzung und Veröffentlichung.

## Umsetzungsstand vom 8. September 2026

Die 31 Pflichtlektionen und die freiwillige Vertiefung sind in Buch, Plattform-Units und Folien ausgearbeitet. Grundlagen und Use-Case-Ermittlung erhalten eigene Einträge in der Navigation. Die Zuordnung steht in `docs/kursmanifest.json`. Schemavalidierung und Renderläufe für Buch und alle 32 Decks sind abgeschlossen. Die ausführliche gemeinsame inhaltliche Durchsicht folgt nach der Veröffentlichung.
