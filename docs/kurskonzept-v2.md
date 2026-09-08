# Kurskonzept v2 — Working with GenAI

HdM-Microcredential „Generative KI in der Praxis: Produktivität steigern und Prozesse sicher optimieren"

| | |
|---|---|
| **Kurs-Slug** | `working-with-genai` |
| **Lehrender** | Jan Kirenz |
| **ECTS** | 1 (30 Stunden Gesamtaufwand) |
| **Laufzeit** | 18.09.2026 (Kickoff) bis 08.10.2026 (Recap und Abgabe) |
| **Zielplattform** | kurse.kirenz.de |
| **Stand** | v2, 07.09.2026 — Rahmen erhalten, lokaler Vollausbau ergänzt |

**Nachtrag vom 07.09.2026 (lokal):** Der durchgehende Lehrfall ist von der zuvor eigens erfundenen Nordwerk Elektrowerkzeuge GmbH auf die **Rösterei Morgenrot** umgestellt, den Fall aus dem Business-Analytics-Kurs. Ausgangslage, Sortiment und Personen werden von dort übernommen, die GenAI-Aufgaben sind neu. Betroffen sind Abschnitt 1 (Lehrfall), Abschnitt 6 (Modulzuschnitt) und Abschnitt 11 (Designentscheidungen). Modulzahl, Lektionszahl, Zeitbudget, Termine und Prüfungsleistung bleiben unverändert.

Version 2 konkretisiert die früheren Entwürfe (`inhalte.md`, `inhalte-3.md` im Notes-Projekt) für die Kursgestaltung. Die eingereichte Modulbeschreibung bleibt die organisatorische Referenz. Was dort als Modulbeschreibung für das HdM-Formular formuliert war, wird hier zu einem umsetzbaren Kursaufbau mit Modulen, Lektionen, Zeitbudget und Werkzeugentscheidungen.

---

## 1. Leitidee

Der Kurs beantwortet eine einzige Frage über sechs Module hinweg: **Wie kommen wir von einem Text, der gut klingt, zu einem Ergebnis, das wir vertreten können?**

Die Teilnehmenden lernen, nützliche Ergebnisse zu erzeugen, mit eigenen Informationen zu verbessern und nachvollziehbar zu prüfen. Der eigene berufliche Nutzen und die Qualität des Ergebnisses verbinden die Module.

Daraus folgen drei Festlegungen, die den ganzen Kurs prägen:

1. **Material vor Formulierung.** Für betriebliche Auskünfte werden relevante, freigegebene Informationen bereitgestellt. Allgemeines Modellwissen ersetzt keine aktuellen Fachinformationen.
2. **Lücken sichtbar machen statt schließen.** Ausgewählte Übungen enthalten Informationslücken. Andere üben Format, Auswahl, Wiederverwendung und Verbesserung, damit der Kurs unterschiedliche Erfolgserlebnisse bietet.
3. **Verantwortung bleibt bei der Person.** Kein Ergebnis geht automatisch heraus. Auch der Miniworkflow in Modul 6 endet bei einem Entwurf, nicht bei einer verschickten Nachricht.

### Durchgehender Lehrfall

Ein erfundenes Unternehmen begleitet den Kurs: die **Rösterei Morgenrot**, eine kleine Kaffeerösterei mit Direktvertrieb an Endkundinnen und Endkunden, eigenem Onlineshop, Kaffee-Abo und drei Sorten im Sortiment. Der Betrieb wächst, ein Gewinn bleibt 2025 trotzdem aus.

Der Fall ist aus dem Business-Analytics-Kurs übernommen, damit derselbe Betrieb zwei Kurse trägt und Teilnehmende, die beide besuchen, sich nicht zweimal in eine Firma einarbeiten. Übernommen werden Ausgangslage, Sortiment mit Listenpreisen und die fünf handelnden Personen mit ihren Funktionen. **Nicht übernommen** wird der Statistikteil: Hier geht es nicht um Auswertungen, sondern um Texte und Auskünfte, die belegbar sein müssen.

Der Einstieg liegt im Kundenservice bei Sina Bergmann. Eine Mail stellt drei Fragen, und sie liegen bewusst unterschiedlich: der reguläre Shop-Preis ist gedeckt, der Sortenwechsel im Abo nur unter einer Bedingung, das Ankunftsdatum der nächsten Lieferung gar nicht. Der Fall bleibt synthetisch, damit jede Aussage nachschlagbar ist und alle Daten unbedenklich in ein Chatfenster kopiert werden dürfen. Die Falldaten liegen unter `material/roesterei-morgenrot.md`, `material/lehrfall-fachinformationen.txt` und `material/kundenanfrage.txt`.

Zwei Ergänzungen sind eigens für diesen Kurs erfunden und im Material als solche gekennzeichnet: die Abo-Regel zum Sortenwechsel (fünf Werktage vor dem Versand) und die Zuspitzung der Anfrage auf drei unterschiedlich belegte Fragen. Preise und Personen stammen dagegen unverändert aus dem Fallmaterial.

Parallel dazu arbeitet jede teilnehmende Person ab Modul 1 an einem **eigenen wiederkehrenden Fall**. Der Lehrfall zeigt die Bauweise, der eigene Fall trägt das Portfolio.

---

## 2. Zielgruppe und Voraussetzungen

Fach- und Führungskräfte aus Verwaltung, Vertrieb, Marketing, Personal und Beratung, die generative KI im eigenen Arbeitsalltag einsetzen wollen. Programmierkenntnisse sind nicht erforderlich und werden an keiner Stelle des Pflichtpfads vorausgesetzt.

Vorausgesetzt wird:

- Ein Browser und ein **kostenloses Chatkonto** (ChatGPT). Kein kostenpflichtiges Abonnement für den Pflichtpfad.
- Ein wiederkehrender Schreib- oder Prüfanlass aus dem eigenen Arbeitsalltag, an dem gearbeitet werden kann.
- Bereitschaft, Ergebnisse gegen das eigene Fachmaterial zu prüfen, statt sie zu übernehmen.

Nicht vorausgesetzt: Vorerfahrung mit KI-Werkzeugen, ein Firmenzugang, eine API, eine Installation.

---

## 3. Didaktisches Muster

Jede Lektion folgt derselben Abfolge. Sie verbindet Beobachten, eigenes Handeln und Prüfen. Die Reihenfolge wird an das jeweilige Lernziel angepasst.

| Schritt | Was passiert | Warum |
|---|---|---|
| 1. Risiko erkennen | Vor jedem Werkzeugeinsatz benennen die Teilnehmenden, was schiefgehen kann | Eine eigene Einschätzung gibt der anschließenden Prüfung einen konkreten Bezug |
| 2. Erklärung | Die wenigen Bausteine kurz und am Fall, nicht als Theorieblock | Theorie steht neben dem Schritt, zu dem sie gehört |
| 3. Mitmachen | Ein vollständiger, kopierfertiger Auftrag, ohne Vorbereitung lauffähig | Erster Erfolg ohne Einrichtungshürde |
| 4. Eigene Variante | Derselbe Aufbau auf den eigenen Fall angewendet | Der Transfer passiert im Kurs, nicht danach |
| 5. Ergebnisprüfung | Abgleich Aussage für Aussage gegen das mitgegebene Material | Die Kernkompetenz des Kurses |
| 6. Portfolio | Der brauchbare Teil wandert in die Arbeitsmappe | Die Prüfungsleistung wächst mit, statt am Ende zu entstehen |

**Rückmeldung.** Auswahlaufgaben (Multiple Choice, Zuordnung, Fehlersuche) geben automatische Rückmeldung. Freitexte und Portfolio-Einträge werden **nicht** automatisch fachlich bewertet; die inhaltliche Rückmeldung kommt vom Lehrenden in den Beratungsterminen. Bewertete Quizfragen zeigen Lösungen erst nach einer richtigen Antwort oder nach dem dritten Versuch. Freie Übungen erhalten davon getrennt erklärendes Feedback.

---

## 4. Werkzeuge und Zugänge

### Pflichtpfad

**ChatGPT als Hauptwerkzeug**, kostenloses Chatkonto. Jede Pflichtübung ist so gebaut, dass sie in einem kostenlosen Konto läuft: keine Datei-Uploads als Bedingung, keine API, kein Abonnement. Wo eine Funktion nur in bezahlten Stufen verfügbar ist, wird das benannt und ein Weg ohne sie gezeigt.

**Claude und Gemini** kommen in Modul 4 als Vergleich dazu: derselbe Auftrag, zwei bis drei Werkzeuge, Beobachtung der Unterschiede am eigenen Fall. **Ausdrücklich ohne Ranking.** Der Kurs erklärt keinen Anbieter zum Sieger; er zeigt, wie ein Auftrag so gebaut wird, dass er übertragbar bleibt, und wie die Übertragbarkeit selbst geprüft wird.

**Microsoft Copilot** wird genannt, weil er in vielen Organisationen der einzige freigegebene Zugang ist. Es gibt aber **keine eigene Übungsschiene** dafür: Der Pflichtpfad bleibt zur Begrenzung des Lernumfangs bei den vereinbarten Werkzeugen.

**n8n** in Modul 6 auf einer **bereitgestellten Kursinstanz**. Die Teilnehmenden bauen den Miniworkflow angeleitet selbst — nicht per Import eines fertigen Workflows. Keine eigene Installation, kein eigener kostenpflichtiger API-Zugang.

### Freiwilliger Praxispfad (Codex, Claude Code)

Am Kickoff steht nach dem ersten Chat-Erfolg eine **Demo von 10 bis 15 Minuten**: Codex und Claude Code am Lehrfall Rösterei Morgenrot. Zweck ist die Einordnung, nicht die Schulung — sichtbar machen, was jenseits des Chatfensters möglich ist, wenn ein Werkzeug Dateien lesen und schreiben darf.

Daran schließt ein **freiwilliger Praxispfad** an, der ab Kursbeginn offensteht: eine erste Aufgabe plus Einrichtungshilfe. Festlegungen dazu:

- **Keine Installation und kein Abonnement sind Pflicht.** Wer den Pfad nicht geht, verliert nichts an der Prüfungsleistung.
- Wer ihn geht, **ersetzt damit einen Teil der persönlichen Transferzeit** (siehe Abschnitt 5). Der Pfad addiert keine Stunden zum 30-Stunden-Budget.
- Der freiwillige Pfad ist in `praxis/codex-claude-code.qmd` ausgearbeitet; die Durchführung der Demo wird vor Kursstart organisatorisch vorbereitet.

### Zugänge — offener Punkt

Vor Kursstart ist eine **Übersicht der Zugangs- und Abo-Optionen** zu erstellen: welche Funktionen im kostenlosen Konto verfügbar sind, was ein bezahlter Zugang zusätzlich bietet und was das kostet. Die Übersicht wird **erst nach Prüfung der Anbieterseiten** gefüllt; Preise und Funktionsumfänge ändern sich häufig und werden hier nicht aus dem Gedächtnis notiert. Bis dahin gilt für die Kursplanung nur die harte Zusage: **Der Pflichtpfad läuft vollständig im kostenlosen Konto.**

---

## 5. Zeitbudget — 30 Stunden

Der offizielle Rahmen aus der Modulbeschreibung: 4 Stunden Präsenz, 20 Stunden Online-Phase und Selbststudium, 6 Stunden Prüfungsleistung.

### Präsenz — 4 Stunden

| Termin | Dauer | Inhalt |
|---|---|---|
| Kickoff 18.09.2026, 13:00–17:00 (vor Ort) | 4,0 h | Modul 1 vollständig, dazu die erste Praxiseinheit aus Modul 2 |

### Online-Phase und Selbststudium — 20 Stunden

**Live online — 3,5 Stunden**

| Termin | Dauer | Rolle |
|---|---|---|
| 24.09.2026, 17:30–18:30 | 1,0 h | Beratungstermin: Rückmeldung zum eingereichten Zwischenstand |
| 30.09.2026, 17:30–18:30 (optional) | 1,0 h | Zweiter Beratungstermin |
| 08.10.2026, 17:30–19:00 | 1,5 h | Recap, Abgabe, Kurzpräsentationen |

**Asynchron — 16,5 Stunden**

| Anteil | Stunden | Inhalt |
|---|---|---|
| Onboarding | 0,5 | Plattform, Konto, Datenregeln, Arbeitsmappe anlegen |
| Angeleitete Lektionen und Praxis | 9,0 | Die Lektionen der Module 2 bis 6 mit den jeweiligen Durchläufen |
| Eigene Erprobung | 7,0 | Arbeit am eigenen Fall zwischen den Lektionen; hierauf entfällt auch der freiwillige Praxispfad, wenn er genutzt wird |

Als Planungsgröße rechnen die 9 Stunden mit im Mittel rund 35 bis 40 Minuten je noch asynchron bearbeiteter Lektion einschließlich eines eigenen Durchlaufs im Chatfenster. **Was im Kickoff live geübt wird, wird im Selbststudium nicht erneut angesetzt** — die Präsenzstunden und die asynchronen Stunden decken unterschiedliche Lektionen ab.

### Prüfungsleistung — 6 Stunden

Ausarbeitung und Dokumentation des Portfolios sowie Vorbereitung der Kurzpräsentation. **Der Recap-Termin selbst zählt in der Online-Phase und wird hier nicht ein zweites Mal angesetzt.**

### Summe

| Block | Stunden |
|---|---|
| Präsenz | 4,0 |
| Online live | 3,5 |
| Asynchron | 16,5 |
| Prüfungsleistung | 6,0 |
| **Gesamt** | **30,0** |

**Teilnahme ohne Prüfungsleistung** ist offiziell möglich. Als interner Planungswert bleiben ohne die sechs Stunden Prüfungsaufwand 24 Stunden; dies ist keine zusätzliche offizielle Kurskategorie. Das Portfolio bleibt in diesem Fall als Arbeitsergebnis empfohlen, wird aber nicht eingereicht.

**Zum Grundlagenpfad:** Der kompakte Einstieg für Teilnehmende ohne Vorerfahrung ist Teil dieser 30 Stunden (Onboarding, Live-Einstieg und die geführten Kernaufgaben der sechs Module). Es gibt **keinen separaten Grundlagenkurs** mit eigenem Stundenumfang.

---

## 6. Module und Lektionen

Sechs Module zu je drei Lektionen, 18 Lektionen insgesamt. Eine Lektion entspricht einem Buchkapitel und einer Unit auf der Lernplattform.

### Jedes Modul hat eine Ansprechperson im Fall

Damit der Fall trägt und nicht nur als Kulisse dient, bekommt jedes Modul eine Funktion aus der Rösterei, aus deren Arbeitsalltag die Beispiele gezogen werden. Die Zuordnung ist eine **Designentscheidung dieses Kurses**; sie steht so nicht im Fallmaterial. Die Personen bleiben über ihre Funktion beschrieben, nicht über Eigenschaften, und die Beispiele werden beim Schreiben der jeweiligen Lektion ausformuliert. Die sechs Module sind nun als lokale Buchkapitel, Folien und Units ausgearbeitet.

| Modul | Funktion im Fall | Anlass, aus dem die Beispiele stammen |
|---|---|---|
| 1 — Ankommen | Jonas Halder, Marketing | Textentwurf aus einem freigegebenen Briefing: schnelles Ergebnis bei geringem Risiko, danach die Grenze, dass Produktversprechen belegt sein müssen |
| 2 — Strukturierte Arbeitsaufträge | Sina Bergmann, Vertrieb und Kundenservice | Die Kundenanfrage zum Abo, an der die Musterlektion gebaut ist |
| 3 — Kontext bereitstellen | Marlene Bosch, Röstung und Produktion | Produktions- und Sortimentsangaben als wiederverwendbare Arbeitsgrundlage; Mengen und Termine werden dabei nicht ergänzt |
| 4 — Qualität prüfen | Petra Lindqvist, Verwaltung und Controlling | Eine Aufbereitung für die interne Besprechung gegen die Quelle abgleichen, offene Angaben festhalten, Testfälle bauen |
| 5 — Verantwortung und Risiko | Aylin Yılmaz, Geschäftsführung | Was wird freigegeben, was geht nach außen, wer klärt verbindlich |
| 6 — In den Alltag bringen | Ellen Ruppert, Lager und Versand | Wiederkehrende Statusanfragen; der Miniworkflow endet beim Entwurf |

Aylin Yılmaz führt den Betrieb und ist Adressatin der Empfehlungen; sie vergleicht Anwendungsfälle und entscheidet, welcher Ablauf als Nächstes erprobt wird. Diese Auswahlentscheidung trägt außer Modul 5 auch die Lektion 1.3. Die vier übrigen Funktionen des Einstiegsteams sind untereinander gleichrangig. Ellen Ruppert gehört nicht zu den fünf Personen des Einstiegs, kommt aber im Fallmaterial als Zuständige für Lager und Versand vor und wird in Modul 6 ohne weitere Einführung genannt. Die Arbeitsaufträge der fünf Personen sind in `material/roesterei-morgenrot.md` zusammengefasst; die interne Herleitung steht in `docs/roesterei-morgenrot-fallbasis.md`.

### Modul 1 — Ankommen: erster Erfolg und erste Grenzen

Der Einstieg produziert innerhalb weniger Minuten ein brauchbares Ergebnis und zeigt danach sofort, wo die Grenzen liegen. Läuft vollständig im Kickoff.

**Outcome:** Ein erstes eigenes Ergebnis erzeugt, die Grenzen eines Chatmodells benannt und einen eigenen Anwendungsfall ausgewählt.

- **1.1 Der erste Chat-Erfolg** — Eine echte kleine Aufgabe im Chatfenster, ohne Vorwissen, mit sichtbarem Ergebnis.
- **1.2 Grenzen und erste Datenregeln** — Woher die Antworten kommen und warum sie falsch sein können; anschließend die Frage, was ins Chatfenster gehört und was nicht.
- **1.3 Den eigenen Anwendungsfall wählen** — Kriterien für einen guten Kandidaten (wiederkehrend, feste Fakten, prüfbares Ergebnis); erster Eintrag im Use-Case-Canvas.

### Modul 2 — Strukturierte Arbeitsaufträge

Vom Zuruf zum Auftrag. Das Modul liefert die Bauweise, die den Rest des Kurses trägt.

**Outcome:** Einen Arbeitsauftrag aus vier Bausteinen bauen, das Ergebnis gegen das Material prüfen und gezielt in Durchläufen verbessern.

- **2.1 Vom Zuruf zum Arbeitsauftrag** — Aufgabe, Material, Format, Grenzen an der Kundenanfrage aus der Rösterei Morgenrot. *(Kapitel ausgearbeitet, Plattform-Unit vorhanden.)*
- **2.2 Mit Beispielen und Format steuern** — Ein Musterbeispiel im Prompt, Vorgaben zu Länge, Ton und Aufbau; wann ein Beispiel mehr hilft als eine Beschreibung.
- **2.3 Iterieren: eine Änderung pro Durchlauf** — Systematisch verbessern statt neu formulieren; die eigene Prompt-Fassung dokumentieren.

### Modul 3 — Kontext bereitstellen

Der Übergang vom einzelnen Prompt zur wiederverwendbaren Arbeitsgrundlage.

**Outcome:** Relevante Fachinformationen auswählen, als Kontext bereitstellen und prüfen, ob die Antwort durch diese Informationen gedeckt ist.

- **3.1 Welche Materialien wirklich relevant sind** — Auswählen statt alles mitschicken; woran zu viel Kontext erkennbar wird.
- **3.2 Regeln und Quellen dauerhaft hinterlegen** — Wiederkehrende Vorgaben einmal festlegen statt jedes Mal eintippen; Quellenangaben im Ergebnis einfordern.
- **3.3 Wenn das Material zu groß wird** — Relevante Textstellen heraussuchen und nur diese mitgeben. Genau das leistet der Ansatz, der unter dem Kürzel RAG läuft. **Behandelt wird das Prinzip des Heraussuchens, nicht die technische Architektur** — keine Vektordatenbanken, keine Embedding-Modelle, kein Systemdiagramm.

### Modul 4 — Qualität prüfen

Das Modul, das den Kurs von einer Prompting-Schulung unterscheidet.

**Outcome:** Ergebnisse gegen Quellen prüfen, eigene Testfälle bauen und die Übertragbarkeit des eigenen Auftrags einschätzen.

- **4.1 Aussagen gegen Quellen prüfen** — Der Abgleich Satz für Satz; typische Stellen, an denen Ungedecktes steht; Umgang mit Zahlen, Fristen und Zitaten.
- **4.2 Testfälle für den eigenen Fall** — Fünf Fälle bauen, darunter einer mit Lücke und einer außerhalb des Bereichs; Ergebnisse festhalten.
- **4.3 Übertragbarkeit: derselbe Auftrag in ChatGPT, Claude und Gemini** — Was gleich bleibt, was sich unterscheidet, welche Formulierungen robust sind. Beobachtung am eigenen Fall, **kein Ranking und keine Kaufempfehlung**.

### Modul 5 — Verantwortung und Risiko-Orientierung

**Outcome:** Die eigenen Risiken benennen, ordnen und die Stellen kennen, an denen eine verbindliche Klärung nötig ist.

- **5.1 Datenschutz im Arbeitsalltag** — Welche Daten in welches Konto dürfen; Platzhalter und Anonymisierung als Handwerk; wer in der eigenen Organisation entscheidet.
- **5.2 Urheberrecht und geistiges Eigentum** — Fremde Inhalte im Material, Rechte an Ergebnissen, Umgang mit Zitaten und Bildern.
- **5.3 AI Literacy und der eigene Risiko-Überblick** — Anforderungen des EU AI Act als Orientierung, Transparenz gegenüber Empfängern, Ausfüllen der Risiko-Tabelle im Portfolio.

> **Wichtige Abgrenzung:** Modul 5 vermittelt **Risiko-Orientierung, keine Konformitätsgarantie.** Der Kurs ersetzt weder eine Rechtsberatung noch eine Datenschutzfolgenabschätzung noch eine interne Freigabe. Das Portfolio benennt für jedes Risikofeld ausdrücklich, wer die verbindliche Klärung vornimmt.

### Modul 6 — In den Alltag bringen

**Outcome:** Die eigene Lösung wiederverwendbar machen, einen einfachen automatisierten Ablauf selbst bauen und den Transfer planen.

- **6.1 Projects und gespeicherte Anweisungen** — Den eigenen Auftrag als dauerhafte Arbeitsumgebung einrichten, statt ihn jedes Mal neu einzufügen.
- **6.2 Ein Miniworkflow, selbst gebaut** — Angeleitet auf der bereitgestellten n8n-Kursinstanz: Auslöser, ein Schritt mit Sprachmodell, Ergebnis als Entwurf. Kein Import eines fertigen Workflows, kein eigener kostenpflichtiger API-Zugang, **kein automatischer Versand**.
- **6.3 Transferplan und Kurzpräsentation** — Die ersten 30 Tage, Beteiligte, Erfolgsmaß, Risiken; Vorbereitung der fünfminütigen Präsentation.

---

### Zuordnung zu den vier Portfolio-Teilen

| Lektionen | Beitrag zum Portfolio |
|---|---|
| 1.1–1.3 | Teil 1: Ausgangsproblem, Grenzen und Use-Case-Canvas |
| 2.1–2.3 | Teil 2: Auftragskarte, vollständige Prompts und dokumentierte Varianten |
| 3.1–3.3 | Teil 2: Kontextmaterial, Herkunft, Regeln und Auswahl relevanter Textstellen |
| 4.1–4.3 | Teil 3: Prüfkriterien, Testfälle und beobachtete Übertragbarkeit |
| 5.1–5.3 | Teil 3: Daten-, Rechte- und Risiko-Check mit offenen Klärungspunkten |
| 6.1 | Teil 2: Wiederverwendung der geprüften Arbeitsgrundlage |
| 6.2 | Teil 4: begründete Entscheidung über mögliche Automatisierung; n8n ist keine Prüfungspflicht |
| 6.3 | Teil 4: Transferplan; Präsentation der vier Teile |

## 7. Ablauf und Meilensteine

| Bis wann | Was liegt vor | Module |
|---|---|---|
| 18.09.2026 (Kickoff) | Erster eigener Chat-Erfolg, gewählter Anwendungsfall, erste Auftragskarte | M1 vollständig, erste Praxis aus M2 |
| 23.09.2026 (Vorabend) | Zwischenstand eingereicht: Use-Case-Canvas und erster Arbeitsauftrag | M1, M2 |
| 24.09.2026 | Beratungstermin mit kurzer Rückmeldung des Lehrenden | — |
| 29.09.2026 (Vorabend) | Zwischenstand eingereicht: Kontextquellen dokumentiert, erste Testfälle | M3, M4 |
| 30.09.2026 | Zweiter Beratungstermin (optional) | — |
| 08.10.2026 | Portfolio vollständig, Kurzpräsentation | M5, M6 |

Die Arbeitsmappe wächst ab dem Kickoff mit. Der Lehrende gibt zu jedem rechtzeitig eingereichten Zwischenstand vor der Beratung eine kurze individuelle Rückmeldung mit zwei bis drei Punkten. Im Termin werden diese besprochen. Der Abgabeweg wird mit den organisatorischen Kursinformationen bekanntgegeben.

---

## 8. Prüfungsleistung

Praxisportfolio: Entwicklung und Dokumentation eines eigenen GenAI-Anwendungsfalls aus dem Berufsalltag, bestehend aus vier Teilen.

1. **Use-Case-Canvas** — Problemdefinition, Zielgruppe, Nutzenversprechen, Datenbedarf, Abgrenzung.
2. **Prompt- und Context-Pipeline** — Der dokumentierte Arbeitsauftrag, gespeicherte Anweisungen, genutzte Kontextquellen und die Entwicklungsschritte.
3. **Qualitäts- und Compliance-Check** — Testfälle mit Ergebnissen, Prüfkriterien, Beobachtung zur Übertragbarkeit und die Risiko-Tabelle mit den Zuständigkeiten für die verbindliche Klärung.
4. **Transferplan** — Erste 30 Tage, Beteiligte, Erfolgsmaß, Risiken, Termin für den Rückblick.

Abschluss: **Kurzpräsentation von 5 Minuten** (Planwert) im Recap-Termin.

Bewertungsgrundlage laut Modulbeschreibung: fachlicher Nutzen, Qualität der Ergebnisse, sichere Umsetzung und Nachvollziehbarkeit des Transferplans. Die Vorlage liegt unter `material/portfolio-vorlage.md`.

**Offen:** Die genaue Bewertungsform (Pass/Fail oder Note) steht in den Vorentwürfen unterschiedlich und ist mit der HdM-Weiterbildung vor Kursstart zu bestätigen.

---

## 9. Umsetzung auf der Lernplattform

Der Kurs läuft auf **kurse.kirenz.de**, nicht auf einer HdM-Instanz. Slug: `working-with-genai`.

- **Buch als kanonische Quelle.** Jede Lektion entsteht zuerst als Quarto-Kapitel in diesem Repo, danach als Plattform-Unit. Kein Inhalt existiert nur in einer Unit-JSON: Alle Lehrfalldaten, Prompts und Materialien stehen vollständig im Buch und zusätzlich als Download unter `material/`.
- **Simulator.** Für diesen Kurs wird der vorhandene Flag `simulator_enabled` bei der Kursanlage auf `false` gesetzt. Damit wird die KI-generierte Zusatzübung deaktiviert. Redaktionell erstellte Quizfragen und didaktische interaktive Simulationen bleiben möglich.
- **Veröffentlichung des Startpakets.** Freigegeben am 07.09.2026: das Buch und die ausgearbeitete Musterlektion 2.1 werden veröffentlicht. Der Kurs ist zunächst nur über den direkten Link erreichbar und erscheint nicht im öffentlichen Katalog. *Stand nach der Fallumstellung: Die veröffentlichte Fassung zeigt weiterhin den vorherigen Lehrfall. Die Umstellung auf die Rösterei Morgenrot liegt bisher nur lokal vor; ein erneuter Buch-Release und ein Plattformimport sind gesondert freizugeben.*
- **Medien.** Der Textpfad ist vollständig und selbsttragend: Jede Übung lässt sich ohne Video und ohne Screenshot durchführen. Screenshots und einige kurze Demo-Videos werden später ergänzt, wo eine Oberfläche sonst schwer zu treffen ist (Projects in Modul 6.1, n8n-Kursinstanz in Modul 6.2).

---

## 10. Offene Punkte

| Punkt | Was fehlt | Wann |
|---|---|---|
| Zugangs- und Abo-Übersicht | Funktionsumfang und Preise nach Prüfung der Anbieterseiten; im Konzept bewusst nicht aus dem Gedächtnis gefüllt | vor Kursstart |
| Freiwilliger Praxispfad | Erste Aufgabe und Einrichtungshilfe für Codex und Claude Code ausformulieren | vor Kursstart |
| Bewertungsform | Pass/Fail oder Note, Abstimmung mit HdM-Weiterbildung | vor Kursstart |
| n8n-Kursinstanz | Bereitstellung, Zugänge, Modellzugang für Modul 6.2 | vor Modul 6 |
| Kapitel 1.1 bis 6.3 | Von 18 Lektionen ist eine geschrieben. Die übrigen 17 liegen nur als Titel, Outcome und Anlass im Fall vor; Text, Prompts und Units fehlen | laufend |
| Screenshots und Demo-Videos | Wenige, gezielt an den Oberflächen-Stellen | nach den Kapiteln |

---

## 11. Quellen und ihre Rolle

Die Trennung ist bewusst: Was ist eine **Designentscheidung** dieses Kurses, und was ist eine **belegte Aussage**?

### Designentscheidungen dieses Kurses

Nicht belegt, sondern gewählt — und als solche im Buch gekennzeichnet:

- Die Vierteilung **Aufgabe, Material, Format, Grenzen** als Merkhilfe für den Aufbau eines Arbeitsauftrags.
- Die Weiterverwendung des synthetischen Falls **Rösterei Morgenrot** aus dem Business-Analytics-Kurs als durchgehender Lehrfall, ohne dessen Statistikteil.
- Die Abo-Regel zum Sortenwechsel (fünf Werktage vor dem Versand) und die Zuspitzung der Kundenanfrage auf drei unterschiedlich belegte Fragen: eigens für diesen Kurs erfunden und im Material gekennzeichnet.
- Die Zuordnung je einer Funktion aus dem Fall zu jedem Modul.
- Die sechsstufige Lektionsabfolge (Risiko erkennen bis Portfolio).
- Der Zuschnitt auf sechs Module zu je drei Lektionen.
- Die Behandlung von RAG als Prinzip des Heraussuchens ohne Architekturteil.

### Belegte Aussagen

- **OpenAI, „How do I prompt ChatGPT effectively?"** — <https://help.openai.com/en/articles/10032626-how-do-i-prompt-chatgpt-effectively>. Empfiehlt: klar formulieren, spezifisch werden, genug Kontext mitgeben, den Prompt iterativ verbessern. Trägt im Kurs die Bausteine *Aufgabe* und *Material* sowie das Iterationsprinzip in Lektion 2.3.
- **Anthropic, Prompt engineering overview** — <https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview>. Setzt vor die Prompt-Optimierung das Festlegen der Erfolgskriterien. Trägt im Kurs die Bausteine *Format* und *Grenzen* sowie den Testfall-Ansatz in Modul 4.

### Kursorganisatorische Grundlagen

- HdM-Weiterbildung, Angebotsseite zum Microcredential GenAI — <https://www.hdm-weiterbildung.de/angebote/kontaktstudium/microcredential-genai>. Quelle für Termine, 1 ECTS, Portfolio-Bestandteile und die Möglichkeit der Teilnahme ohne Prüfung. Die Stundenaufteilung 4 + 20 + 6 stammt aus den Notes-Entwürfen.
- Notes-Projekt `11_HdM_Micro_GenAI`, Dateien `inhalte.md` und `inhalte-3.md`. Quelle für Modultitel, Lernziele und die Vier-Teile-Struktur des Portfolios.

**Keine erfundene Forschung.** Wo im Kurs eine Aussage über das Verhalten von Sprachmodellen getroffen wird, wird sie als Mechanismus beschrieben („ein Chatmodell setzt Text fort, der zur Anfrage passt") und nicht als Häufigkeitsbehauptung („der häufigste Fehler ist …"). Häufigkeitsaussagen kommen im Kursmaterial nur vor, wenn eine Quelle sie trägt.

## Vollausbau vom 07.09.2026

Alle 18 Lektionen liegen als Buchkapitel, Folien und Plattform-Units vor. Hinzu kommen ein persönlicher Lernweg, ein Werkzeugkompass, die frühe Demo samt freiwilligem Codex-/Claude-Code-Pfad und vollständige modulbezogene Übungsmaterialien. Zuordnung in `docs/kursmanifest.json`, Lehrdurchführung in `docs/lehrleitfaden.md`. Tests und gemeinsame Inhaltsdurchsicht stehen aus; die lokale Ausarbeitung ist kein Produktionsrelease.

Die neun Stunden angeleitete asynchrone Arbeit verteilen sich als Planungswerte auf Modul 2 (80 Minuten Nacharbeit und Vertiefung), Modul 3 (120), Modul 4 (120), Modul 5 (90) und Modul 6 (130). Was live bearbeitet wurde, wird nicht erneut als eigenständige Pflichtleistung angesetzt. Der Lehrleitfaden trennt Präsenz, eigene Erprobung und Prüfungsdokumentation.
