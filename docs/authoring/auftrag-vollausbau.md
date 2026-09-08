# Vollausbau: gemeinsamer Arbeitsvertrag

Nutzerauftrag 07.09.2026: alle übrigen Lektionen, Buch UND Folien UND interessante Selbstlernphase selbständig mit Fable 5.1 ausarbeiten. Bestehende eigene Kurse Frech, VWA und SiMa.ai als didaktische Quellen nutzen. Umfang vollständig lokal fertigstellen, kein Commit/Push/Deploy. Keine Tests, Render, Validatoren, Browserchecks oder Review-Schleifen; Nutzer geht alles später gemeinsam durch. Produktionsstand nicht verändern. Nicht mit „Plan“ oder Gerüsten abschließen.

## Kanonischer Rahmen

`docs/kurskonzept-v2.md`, `material/roesterei-morgenrot.md`, `docs/roesterei-morgenrot-fallbasis.md` und `AGENTS.md`. 6 Module, 18 Lektionen, 30 Stunden (4 Präsenz +20 online/selbst +6 Prüfung). Portfolio wächst: 1 Canvas, 2 Prompt-/Context-Pipeline, 3 Qualität/Compliance, 4 Transfer. Kostenfreies Chatkonto als Hauptpfad, keine Pflicht-API/Installation; Funktion nicht verfügbar → vollständiger Weg per Copy/Paste. Claude/Gemini vergleichend, Copilot kurz einordnen. Kein Modellranking oder unbelegtes Sparversprechen. Früh Codex/Claude-Code-Demo, später freiwillige Vertiefung. n8n selbst geführt bauen auf vorbereiteter Kursinstanz, kein automatischer Versand, kein eigenes API-Abo, keine Prüfpflicht. Simulator bleibt false.

Rösterei und Personen/Sortiment wie vorhanden. Neue Zusatzmaterialien als synthetische GenAI-Erweiterung benennen. Keine echten Daten aus Firmenkursen kopieren (auch keine Kundenlisten, Meetingprotokolle, Logins, private Links oder Screenshots mit Kundendaten). Nur didaktische Muster, eigene generische Texte und klar synthetische Beispiele übertragen. Quelle und Übernahme jeweils in eigener Autorennotiz nennen.

## Verbindliche Dateimatrix

| Nr | Buchpfad (.qmd) / Folienpfad unter slides/ | Unit-Datei (.unit.json) |
|---|---|---|
|1.1|start/erster-chat|01-01-erster-chat|
|1.2|start/grenzen-daten|01-02-grenzen-daten|
|1.3|start/anwendungsfall|01-03-anwendungsfall|
|2.1|prompting/arbeitsauftrag (bestehend)|02-01-arbeitsauftrag (bestehend, IDs bewahren)|
|2.2|prompting/beispiele-format|02-02-beispiele-format|
|2.3|prompting/iterieren|02-03-iterieren|
|3.1|kontext/material-auswaehlen|03-01-material-auswaehlen|
|3.2|kontext/regeln-quellen|03-02-regeln-quellen|
|3.3|kontext/material-finden|03-03-material-finden|
|4.1|qualitaet/aussagen-pruefen|04-01-aussagen-pruefen|
|4.2|qualitaet/testfaelle|04-02-testfaelle|
|4.3|qualitaet/toolvergleich|04-03-toolvergleich|
|5.1|verantwortung/datenschutz|05-01-datenschutz|
|5.2|verantwortung/urheberrecht|05-02-urheberrecht|
|5.3|verantwortung/ki-kompetenz|05-03-ki-kompetenz|
|6.1|transfer/wiederverwenden|06-01-wiederverwenden|
|6.2|transfer/miniworkflow|06-02-miniworkflow|
|6.3|transfer/transferplan|06-03-transferplan|

Units: /Users/jankirenz/code/hdm/lernplattform/apps/api/app/db/units/working-with-genai/. source.url = https://kirenz.github.io/working-with-genai/<Buchpfad>.html. source.chapter = Modul N · Titel. Kein neuer Programmcode nötig. Schreibbefugnis je Agent strikt auf seine Zeilen, zugehörige material/mNN/ und slides/Module sowie eigene Autorennotiz beschränken. Root pflegt gemeinsame Navigation, index, README, Konzeptstatus, Kursmanifest und Lehrleitfaden. Diese gemeinsamen Dateien nicht bearbeiten.

## Ausarbeitungsniveau

Pro neuem Buchkapitel etwa 900–1500 Wörter als Orientierung, keine Textlänge um ihrer selbst willen. Eine Handlung und sichtbares Ergebnis, konkreter Anlass aus Morgenrot, Lernziel und Zeit, vollständiges Material/Download, copy-ready Prompt, geführte Schritte, konstruiertes Sollbeispiel, begründete Rückmeldung, eine eigene Variante, kurzer Portfolioeintrag. Kursmaterial vollständig nutzbar ohne Video. Keine leeren TODO-Kapitel. Schwieriges neben dem Schritt erklären, keine Prompt-Pattern-Liste oder Technikvorlesung.

Abwechslung durch begründete Entscheidung, Sortieraufgabe, Reparaturauftrag, Quellenpuzzle, Aktennotiz, Mini-Fall, Vorher/Nachher, Erklär-es-einer-Kollegin. Nicht jede Lektion künstlich dieselbe Risikosituation. Formative Selbstlernaufgaben redaktionell vorgeben; Nutzer verbietet die KI-Funktion zum Generieren eigener Zusatzaufgaben. Eigene berufliche Fälle und selbst konstruierte Testfälle bleiben legitime Lernziele.

Units etwa 7–11 Schritte, 2–3 feste Quizfragen plus echter Toolauftrag und Transfer/Portfolio. Nicht nur Buch-Link und Quiz. Verwende tatsächliche Schemas in app/schemas/lesson_block.py und quiz.py (bei abweichendem Pfad suchen), Beispiel vorhandene Musterunit und n8n-grundlagen-uc. Kein Schema erfinden. Abwechslung über vorhandene Fragetypen; komplexes Widget nur wenn wirklich passend und mit bekanntem Schema, keine neue UI. Keine Quizlösung in der direkt vorangehenden Erklärung verraten. Solutions für freie Übungen erst nach Bearbeitung enthüllen. Freitext wird nicht automatisch fachlich bewertet.

Folien nach Buch schreiben, pro Lektion 7–10 inhaltliche Folien mit Speaker-Notes. Keine 20-Zeilen-Prompts winzig auf Folien: kurz sinnvoll zeigen, Vollprompt im Buch verlinken, Demo-Auftrag in Notizen. Kopierbares Material nicht ausschließlich in Notizen. `slides/AGENTS.md` gilt. Root stellt Theme und Metadaten bereit.

## Materialvorbilder (nur lesen)

- /Users/jankirenz/code/presentation/training-frech/uebungen.qmd und handout/_uebungen/: niedrige Einstiegshürde, Vormachen → Mitmachen → eigenes Prüfen, kontrollierte Beispieldaten.
- /Users/jankirenz/code/consulting/vwa-ki-strategie/buch/: Nutzen, Kontext, Quellen, Projekte und praktische Vorlagen.
- /Users/jankirenz/code/consulting/vwa-ki-strategie/IT/: Arbeitsaufträge, enge Aktionsrechte, Freigaben, Piloteinführung. Kein IT-Detailniveau in den Pflichtkurs übertragen.
- /Users/jankirenz/code/consulting/sima-ai/reference/ und Plattformunits claude-sima, gemini-workspace, ai-sima. Claude-Projekte/Dateiarbeit/Skills/CLAUDE.md und Recherche didaktisch übernehmen, nicht die Enterprise-Anbindungen voraussetzen.
- /Users/jankirenz/code/kurse/n8n-grundlagen sowie Units n8n-grundlagen-uc für geführte Handlungsschritte und Formate.

## Quellenstand für aktuelle Inhalte

Root hat am 07.09.2026 offizielle Seiten abgerufen. Details bei Bedarf gezielt über WebFetch/WebSearch selbst öffnen, keine ungeprüften Preise/Limits/Schaltflächen erfinden. In eigener Autorennotiz konkrete Quellen, Abrufdatum, getragene Aussage und Unsicherheit nennen; im Buch kurze passende Primärlinks. Maximal kurze Paraphrasen, keine übernommenen langen Dokumentationsabsätze.

- https://help.openai.com/en/articles/10169521 (Projects): wiederverwendbarer Kontext und Anweisungen; Zugriff/Tools folgen Konto und Workspace. Kein Freigabenachweis für vertrauliche Daten.
- https://help.openai.com/en/articles/10500283 (Deep research): mehrstufige Recherche mit Quellen; verfügbarer Umfang kontobedingt; normale Suche oder bereitgestellte Quellen als Ausweichweg.
- https://support.claude.com/en/articles/9519177-how-can-i-create-and-manage-projects: Claude Projects, Anweisungen und Wissensmaterial.
- https://support.google.com/gemini/answer/15235603: Gems mit wiederverwendbaren Anweisungen und Material; Funktionsumfang accountabhängig.
- https://code.claude.com/docs/en/overview und /en/skills: Claude Code kann Dateien bearbeiten und Werkzeuge benutzen, Skills für wiederkehrende Aufgaben. Aufgabe, Bereich und Aktionsgrenzen vorgeben.
- https://developers.openai.com/codex/app/ leitet inzwischen auf https://learn.chatgpt.com/docs/app um. Produktbezeichnung und verfügbare Wege sind im Wandel: Codex im Kurs wie gewünscht zeigen, keine alten Produktnamen/Featuregrenzen als sichere Neuigkeit behaupten. Für Einsteiger nach Handlung unterscheiden: Chat antwortet, Arbeitsagent kann Dateien/Werkzeuge bearbeiten. Agententeil freiwillig.
- https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.chainllm/ und https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.set/: Basic LLM Chain und Edit Fields. Zentral vorbereitete Modell-Credentials sind organisatorische Voraussetzung, noch nicht tatsächlich eingerichtet; Ersatzweg mit manuell eingefügtem konstruiertem Modellergebnis.
- https://digital-strategy.ec.europa.eu/en/faqs/ai-literacy-questions-answers: aktuelle FAQ enthält geänderten Art.4 nach Digital Omnibus. Maßnahmen zur Förderung von KI-Kompetenz kontextbezogen; ausdrücklich KEINE Garantie eines bestimmten individuellen Niveaus. Seitenkopf enthält ältere Formulierung, Detailantworten aktualisiert. Keine pauschale alte Aussage über vorgeschriebenes Zertifikat oder festen Schulungsumfang übernehmen, keine ungesicherte Rechtschronologie. Autorennotiz benennt Versionsunterschied. Für aktuelle Fristen und Einzelpflichten weiterführend geltenden Text öffnen, sonst Rechtsdetail weglassen.
- https://www.gesetze-im-internet.de/urhg/__2.html und /__51.html: persönliche geistige Schöpfung, Zitatrecht zweckgebunden; „Quelle nennen genügt“ ist falsch. Lizenz/Übernahmerechte/Schutzfähigkeit getrennt behandeln.
- https://www.datenschutzkonferenz-online.de/media/oh/20240506_DSK_Orientierungshilfe_KI_und_Datenschutz.pdf und Orientierungshilfen-Index: Freigabe/Zweck/Datenminimierung/accountbezogene Verarbeitung; pseudonymisiert ist nicht automatisch anonym. Orientierung statt juristisches Gutachten.

Abschlussbericht: konkret erstellte Dateien, didaktische Entscheidungen, wiederverwendete Vorlagen, offene Betriebsabhängigkeiten. Keine ausgeführten Tests behaupten. Keine neuen Subagenten starten; Fable 5.1 ist angefordert.
