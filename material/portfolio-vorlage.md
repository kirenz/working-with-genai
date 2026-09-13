# Arbeitsmappe: Vorlage für das Praxisportfolio

Kursmaterial „Working with GenAI" (HdM-Microcredential, Kickoff 18.09.2026, Recap 08.10.2026)

Diese Datei ist die Arbeitsmappe. Sie wird nicht am Ende geschrieben, sondern wächst vom ersten Kurstag an mit. Die Arbeit am eigenen Vorhaben liefert pro Modul einen Beitrag; am Recap-Termin ist die Mappe das Prüfungsdokument.

**So wird sie benutzt:** Datei kopieren, umbenennen (`portfolio-<name>.md` oder als Textdokument), und die Platzhalter in spitzen Klammern durch eigene Inhalte ersetzen. Format ist freigestellt: Markdown, Word, Folien. Entscheidend ist, dass die vier Teile erkennbar sind.

> **Datenregel:** Keine echten Namen, Adressen, Kunden- oder Vertragsnummern in der Mappe. Für die Übungen vollständig erfundene Angaben verwenden. Allein Namen und Nummern zu ersetzen genügt bei vertraulichen Inhalten nicht. Was im Alltag zulässig ist, entscheidet die Regelung der eigenen Organisation.

---

## Teil 1: Use-Case-Canvas

Vor dem Canvas stehen zwei bis drei Kandidaten aus dem Tätigkeitsinventar. Offene Voraussetzungen werden kenntlich gemacht. Vor der Erprobung muss geklärt sein, dass die benötigten Daten und Werkzeuge verwendet werden dürfen. Die Auswahlbegründung gehört zu diesem ersten Portfolio-Teil.

| Kandidat und heutiges Problem | Erwarteter Nutzen | Aufwand einschließlich Prüfung | Daten und offene Voraussetzungen | Entscheidung mit Begründung |
|---|---|---|---|---|
| <Aufgabe 1> | <Beobachtung oder Annahme> | <Beobachtung oder Annahme> | <Was ist vorhanden, was fehlt?> | <Pilot / zuerst klären / anderer Lösungsweg> |
| <Aufgabe 2> | <…> | <…> | <…> | <…> |
| <Aufgabe 3, falls vorhanden> | <…> | <…> | <…> | <…> |

Für den gewählten Pilotfall werden die folgenden sechs Felder ausgefüllt.

**Problem.** <Welche Aufgabe kostet heute Zeit oder Qualität? Was passiert konkret, wenn sie schlecht läuft?>

**Zielgruppe.** <Wer bekommt das Ergebnis: Kundschaft, Fachabteilung, Leitung, Öffentlichkeit?>

**Nutzenversprechen (zunächst eine Annahme).** <Was ist nach der Umsetzung besser? Die erwartete Veränderung zunächst als Annahme kennzeichnen: Zeit pro Vorgang einschließlich Nacharbeit, Qualität, Häufigkeit pro Woche, Zahl der Beteiligten.>

**Häufigkeit und Umfang.** <Wie oft fällt der Fall an? Wie lang ist ein typischer Vorgang?>

**Datenbedarf.** <Welche Informationen benötigt die Aufgabe, wo liegen sie und dürfen sie im vorgesehenen Werkzeug verwendet werden?>

**Abgrenzung.** <Was gehört ausdrücklich nicht dazu? Welche Entscheidung bleibt bei einem Menschen, und welche Rolle verantwortet Prüfung und nächsten Schritt?>

---

## Teil 2: Prompt- und Context-Pipeline

Dokumentiert wird, welchen Auftrag das Modell erhält, welche Informationen bereitgestellt werden und wie das Ergebnis beurteilt wird.

### Auftragskarte aus Modul 2

Diese Auftragskarte entsteht in der Musterlektion am Lehrfall Rösterei Morgenrot und gehört zu Teil 2. Sie ist eine Planungshilfe; das tatsächliche Material und die vollständigen Prompts werden darunter ergänzt. Der eigene Fall ersetzt dabei den Lehrfall, die Bauweise bleibt dieselbe.

| Feld | Eintrag |
|---|---|
| **Der Fall**: welche berufliche Aufgabe? | <z. B. Anfragen zu Abo-Änderungen und Lieferterminen, mehrmals pro Woche> |
| **Task**: gewünschtes Ergebnis | <z. B. Entwirf eine Antwort-Mail auf die folgende Anfrage.> |
| **Context**: welche Informationen und Rahmenbedingungen sind erforderlich? | <z. B. Rolle im Kundenservice; Auszug aus der Konditionsübersicht, als Text in den Prompt eingefügt> |
| **Format**: Ergebnisform, Umfang, Aufbau | <z. B. E-Mail, höchstens 150 Wörter, am Ende eine Liste „Offen"> |
| **Check**: was soll das Modell kennzeichnen, wenn eine Angabe fehlt? | <z. B. nicht beantworten, sondern unter „Offen" auflisten> |
| **Prüfung vor der Verwendung**: wie wird das Ergebnis beurteilt und freigegeben? Diese Prüfung machen wir selbst; der Check im Prompt ersetzt sie nicht. | <z. B. gegen den Context lesen, korrigieren, selbst versenden> |

---



**Der Arbeitsauftrag im Wortlaut.** <Den fertigen Prompt vollständig einfügen, mit den vier Teilen TASK, CONTEXT, FORMAT, CHECK.>

**Gespeicherte Anweisungen, soweit verwendet.** <Was ist dauerhaft hinterlegt, etwa als Projekt-Anweisung oder System-Prompt, statt bei jedem Durchlauf neu eingetippt zu werden?>

**Kontextquellen.**

| Quelle | Woher | Wie eingebunden | Wie aktuell gehalten |
|---|---|---|---|
| <z. B. Konditionsübersicht> | <z. B. Intranet-Seite, PDF> | <z. B. relevanter Abschnitt in den Prompt kopiert> | <z. B. bei jeder Preisänderung> |

**Übungsmaterial im Wortlaut.** <Die freigegebenen beziehungsweise synthetischen Ausgangstexte einfügen oder beilegen; Herkunft allein genügt nicht.>

**Entwicklungsschritte.** <Zwei bis vier Durchläufe, jeweils: welcher Prompt wurde verwendet, was wurde verändert und was wurde beobachtet? Mindestens eine unveränderte Wiederholung festhalten. Wenige Durchläufe erlauben keine sichere Ursachenzuordnung.>

---

## Teil 3: Qualitäts- und Compliance-Check

**Testfälle.** Mindestens fünf: ein typischer Fall, fehlende Angaben, eine Bedingung, widersprüchliche Vorgaben und eine Aufgabe außerhalb des vorgesehenen Bereichs. Die konkreten Fälle und Erwartungen richten sich nach dem Vorhaben. Bei einer Ideenaufgabe können beispielsweise widersprüchliche Ziele, eine fehlende Zielgruppe oder eine feste Budgetgrenze geprüft werden. Die Tabelle zeigt Beispiele für Auskunftsaufgaben.

| # | Eingabe (kurz) | Erwartetes Ergebnis | Tatsächliches Ergebnis | Bestanden? |
|---|---|---|---|---|
| 1 | <Standardfall> | <...> | <...> | <ja/nein> |
| 2 | <Fall mit fehlender Angabe> | <steht unter „Offen"> | <...> | <ja/nein> |
| 3 | <Fall mit Bedingung> | <Zusage bleibt an die Bedingung geknüpft> | <...> | <ja/nein> |
| 4 | <Fall außerhalb des Bereichs> | <wird abgelehnt oder ausgewiesen> | <...> | <ja/nein> |
| 5 | <Widerspruch zwischen Quellen> | <Widerspruch benannt; keine unbegründete Auswahl> | <...> | <ja/nein> |

**Durchlauf dokumentieren.** <Datum, Werkzeug und sichtbare Modellbezeichnung, sofern angezeigt; neue oder fortgesetzte Unterhaltung; verwendete Materialversion. Bei einer konstruierten Kursantwort ausdrücklich „Kursbeispiel, kein eigener Modelllauf“ notieren. Nicht ausgeführte Fälle als offen markieren.>

**Prüfkriterien.** <Woran wird „gut" festgemacht? Je nach Aufgabe etwa sachliche Richtigkeit, Quellenstütze, Vollständigkeit, nachvollziehbare Berechnung, Vielfalt der Ideen, Form und Ton. Den Maßstab und den Prüfschritt konkret nennen.>

**Übertragbarkeit.** <Derselbe Auftrag in einem zweiten Werkzeug: Was war anders, was blieb gleich? Kein Ranking, sondern eine Beobachtung am eigenen Fall.>

**Risiko-Orientierung.** Keine Konformitätserklärung, sondern eine geordnete Einschätzung mit den offenen Punkten:

| Feld | Einschätzung | Wer klärt das verbindlich? |
|---|---|---|
| AI-Act-Einordnung | <Rolle, Art der Verwendung, sich daraus ergebende Pflicht oder deren Fehlen> | <z. B. Führungskraft; offene Rechtsfrage an die Rechtsberatung> |
| Personenbezogene Daten im Prozess | <welche, in welchem Schritt, wie ersetzt> | <z. B. Datenschutzbeauftragte> |
| Genutztes Konto / Vertragslage | <privat, geschäftlich, welche Vereinbarung besteht> | <z. B. IT, Einkauf> |
| Rechte an Eingaben und Ergebnissen | <fremde Inhalte im Material? Weiterverwendung des Ergebnisses?> | <z. B. Rechtsabteilung> |
| Transparenz gegenüber Empfängern | <wird der KI-Einsatz kenntlich gemacht, und wo?> | <z. B. Führungskraft> |
| Verbleibende Risiken | <was bleibt offen, und wie wird damit umgegangen?> | <...> |

---

## Teil 4: Transferplan

**Erste 30 Tage.** <Welche zwei bis drei Schritte werden konkret umgesetzt? Mit Datum und verantwortlicher Rolle.>

**Beteiligte.** <Wer muss zustimmen, wer muss informiert werden, wer nutzt es mit?>

**Woran wird der Erfolg gemessen?** <Eine Kennzahl oder Beobachtung, die nach vier Wochen prüfbar ist.>

**Was den Plan scheitern lassen könnte.** <Ehrlich: fehlende Freigabe, fehlende Zeit, unklare Datenlage, Widerstand im Team.>

**Wann wird nachgesteuert?** <Fester Termin für einen Rückblick.>

---

## Termine und Ablauf

| Wann | Was |
|---|---|
| 18.09.2026, 13:00–17:00 (Präsenz) | Kickoff. Kandidaten und ein vorläufiger Pilot werden erarbeitet. Auswahl, Canvas und erster eigener Auftrag werden bis zum 23.09. festgehalten. |
| 23.09.2026, Vorabend | Zwischenstand einreichen: Teil 1 und der Prompt aus Teil 2. |
| 24.09.2026, 17:30–18:30 (online) | Beratungstermin. Besprechung der kurzen individuellen Rückmeldung zum eingereichten Stand. |
| 29.09.2026, Vorabend | Zwischenstand einreichen: Teil 2 vollständig, Testfälle aus Teil 3 begonnen. |
| 30.09.2026, 17:30–18:30 (online, optional) | Zweiter Beratungstermin. |
| 08.10.2026, 17:30–19:00 (online) | Recap, Abgabe der Mappe, Kurzpräsentation. |

**Kurzpräsentation:** 5 Minuten als Planwert, entlang der vier Teile. Keine gestaltete Foliensammlung nötig; die Mappe selbst darf gezeigt werden.

**Bewertungsgrundlage** laut Modulbeschreibung: fachlicher Nutzen, Qualität der Ergebnisse, sichere Umsetzung und Nachvollziehbarkeit des Transferplans. Die genaue Bewertungsform (Pass/Fail oder Note) ist mit der HdM-Weiterbildung noch zu bestätigen und wird vor dem Kickoff nachgetragen.

**Rückmeldung im Kurs:** Freitexte werden nicht automatisch fachlich bewertet. Die Lernplattform gibt Rückmeldung zu Auswahlaufgaben; inhaltliche Rückmeldung kommt vom Lehrenden vor und in den Beratungsterminen.
