# n8n-Kursvorbereitung für Lektion 6.2

Organisatorische Vorbereitung des Miniworkflows, Stand 07.09.2026. Diese Notiz fasst zusammen, was vor dem Kurs vorliegen muss, damit Lektion 6.2 wie im Buchkapitel `transfer/miniworkflow.qmd` beschrieben durchführbar ist. Sie beschreibt **keinen erledigten Aufbau**: Zum Zeitpunkt dieser Notiz ist die Kursinstanz mit ihrer zentralen Modell-Credential **nicht eingerichtet**. Alle Angaben sind Vorbereitungsaufgaben, keine Zustandsmeldungen.

## Was die Lektion voraussetzt

| Voraussetzung | Wer stellt sie bereit | Stand |
|---|---|---|
| Erreichbare n8n-Kursinstanz mit Zugang für alle Teilnehmenden | Lehrende | offen |
| Ein dort hinterlegtes Chat-Model mit einer Kurs-Credential | Lehrende | offen |
| Adresse der Instanz und Name des Chat-Model-Knotens in den Kursinformationen | Lehrende | offen |
| Kein eigener API-Schlüssel, kein bezahltes Konto, keine Installation bei den Teilnehmenden | — | so festgelegt |

Die Teilnehmenden tragen die Adresse der Instanz einmal in das Profilfeld der Plattform-Unit 06-02 ein; danach führen die Aktionslinks der Unit dorthin. Im Repo steht keine Adresse.

## Was vor dem Kurs zu klären ist

Diese Punkte hängen von der konkreten Instanz und ihrer Version ab. Sie werden vor dem Kurs an der laufenden Instanz nachgesehen, nicht aus der Dokumentation angenommen:

1. **Zugang.** Wie melden sich die Teilnehmenden an, und legt jede Person eigene Workflows an? Die Lektion sieht vor, dass jeder Workflow das eigene Kürzel im Namen trägt, damit die Workflows der Kursgruppe unterscheidbar bleiben.
2. **Modellzugang.** Welcher Chat-Model-Knoten steht zur Verfügung, und unter welchem Namen erscheint er im Auswahlmenü? Die Kursinformationen nennen ihn wörtlich, damit im Kurs nicht gesucht wird.
3. **Credential.** Ist die hinterlegte Credential für die Konten der Teilnehmenden auswählbar, oder sehen sie nur ihre eigenen? Falls sie nicht auswählbar ist, ist die Lektion ohne Modellschritt zu planen und der Ersatzweg der reguläre Weg. Ob und wie eine Credential geteilt werden kann, hängt von Betriebsart und Lizenzstufe der Instanz ab und wird an der Instanz geprüft.
4. **Kontingent.** Welche Nutzungsgrenze hängt an der Credential, und trägt sie eine Kursgruppe, die den Knoten mehrfach ausführt? Ein erschöpftes Kontingent während der Übung ist der wahrscheinlichste Störfall.
5. **Beschriftungen.** Die Lektion nennt **Trigger manually**, **Edit Fields (Set)** mit **Manual Mapping** und **Fields to Set**, **Basic LLM Chain** mit **Define below**, den Modi **Fixed** und **Expression**, den Anschluss **Model** sowie **Execute step**, **Execute workflow** und **Activate**. Diese Bezeichnungen folgen der n8n-Dokumentation zu [Edit Fields (Set)](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.set/) und [Basic LLM Chain](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.chainllm/) (Abruf 07.09.2026). Einzelne Schaltflächen können in der Version der Instanz anders heißen; Abweichungen werden vor dem Kurs notiert und in den Kursinformationen ergänzt, statt sie im Material zu raten.
6. **Aufräumen.** Wann werden Kurs-Workflows und Ausführungen gelöscht, und wer macht das? Auch bei rein synthetischen Daten gehört das in die Kursinformationen.

Zu Versionsnummern, Plänen und Funktionsumfang der Instanz macht diese Notiz bewusst keine Angaben. Was gilt, wird an der eingerichteten Instanz nachgesehen.

## Daten in dieser Übung

Alle Werte sind konstruiert: die Statusanfrage von „K. Weber“, die Versandinformationen von Lager und Versand und der konstruierte Entwurf für den Ersatzweg. Die Sendungsnummer bleibt ein Platzhalter, weil sie im Alltag eine Kennung wäre, die nicht in einen Modellschritt gehört.

Beide Feldwerte stehen fest im Knoten `Anfrage und Material`. Das ist eine didaktische Entscheidung und keine Vereinfachung aus Bequemlichkeit: So fließen keine echten Daten, und der Knoten steht trotzdem für die beiden Zulieferungen, die im Alltag auseinanderfallen. Eine Anbindung an ein echtes Postfach ist nicht Teil des Kurses.

## Was der Workflow nicht enthält

- **Keinen Versandknoten.** Kein Send Email, kein Gmail, kein Outlook.
- **Keinen Auslöser auf ein Postfach.** Der Ablauf startet per Klick.
- **Keine Aktivierung.** Der Workflow wird gespeichert und bleibt inaktiv; getestet wird mit *Execute step* am Knoten oder *Execute workflow*.

Das ist keine Vorsicht für den Kursbetrieb, sondern die Verantwortungslage aus Modul 5: Der Entwurf wird von einer Person geprüft und selbst versendet. Wer im Betrieb einen automatischen Versand erwägt, beginnt bei der Risiko-Tabelle, nicht beim Knoten.

## Ersatzweg, wenn der Modellzugang fehlt

Der Ersatzweg steht im Buchkapitel als Schritt 5 und in der Plattform-Unit als eigener Auftrag. Er ist vollständig und führt zum selben Ausgabefeld:

1. Knoten `Entwurf` entfernen oder abklemmen; die ersten beiden Knoten bleiben unverändert.
2. Zweiten **Edit Fields (Set)** anhängen, Name `Entwurf (manuell)`.
3. Ein Feld `text`, Typ String, Modus Fixed. Wert: entweder der konstruierte Entwurf aus `material/m06/entwurf-konstruiert.txt` oder ein selbst im kostenlosen Chatkonto erzeugter und geprüfter Entwurf. Dabei werden die beiden Ausdrücke im Prompt von Hand durch Material und Anfrage ersetzt.
4. *Execute step*; das Output-Panel zeigt das Feld `text`.
5. Speichern, nicht aktivieren.

Was der Ersatzweg offenlässt, wird im Kurs benannt: die Frage, wie zuverlässig ein Modell die Grenzen einhält, wenn Material und Anfrage über Ausdrücke hineinkommen. Sie wird als offener Punkt notiert, falls der Modellzugang später bereitsteht.

## Zeitliche Einordnung

Die Lektion gehört in die asynchrone Phase; das zugehörige Deck rechnet mit rund 15 Minuten Arbeitsphase für den Aufbau. Prüfungsrelevant ist nicht der Workflow, sondern die begründete Entscheidung über Automatisierung in Portfolio-Teil 4. Wer den Workflow nicht baut, bearbeitet die Entscheidung mit dem Ersatzweg und verliert nichts.

## Prüfliste vor dem Kurs

- [ ] Instanz erreichbar, Zugänge verteilt
- [ ] Chat-Model-Knoten vorhanden, Name in den Kursinformationen wörtlich genannt
- [ ] Kurs-Credential hinterlegt und aus den Teilnehmendenkonten auswählbar
- [ ] Kontingent für eine Kursgruppe geprüft
- [ ] Abweichende Beschriftungen notiert und in den Kursinformationen ergänzt
- [ ] Der Aufbau aus dem Kapitel einmal selbst durchgespielt, einschließlich Ersatzweg
- [ ] Regel bekannt gegeben: kein Versandknoten, keine Aktivierung, eigenes Kürzel im Workflownamen
- [ ] Aufräumtermin und Zuständigkeit festgelegt
