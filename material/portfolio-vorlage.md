# Arbeitsmappe — Vorlage für das Praxisportfolio

Kursmaterial „Working with GenAI" (HdM-Microcredential, Kickoff 18.09.2026, Recap 08.10.2026)

Diese Datei ist die Arbeitsmappe. Sie wird nicht am Ende geschrieben, sondern wächst vom ersten Kurstag an mit. Jede Lektion liefert einen Baustein; am Recap-Termin ist die Mappe das Prüfungsdokument.

**So wird sie benutzt:** Datei kopieren, umbenennen (`portfolio-<name>.md` oder als Textdokument), und die Platzhalter in spitzen Klammern durch eigene Inhalte ersetzen. Format ist freigestellt — Markdown, Word, Folien. Entscheidend ist, dass die vier Teile erkennbar sind.

> **Datenregel:** Keine echten Namen, Adressen, Kunden- oder Vertragsnummern in der Mappe. Für die Übungen vollständig erfundene Angaben verwenden. Allein Namen und Nummern zu ersetzen genügt bei vertraulichen Inhalten nicht. Was im Alltag zulässig ist, entscheidet die Regelung der eigenen Organisation.

---

## Teil 1 — Use-Case-Canvas

Der Anwendungsfall, an dem im ganzen Kurs gearbeitet wird. Ein Fall, nicht drei.

**Problem.** <Welche Aufgabe kostet heute Zeit oder Qualität? Was passiert konkret, wenn sie schlecht läuft?>

**Zielgruppe.** <Wer bekommt das Ergebnis: Kundschaft, Fachabteilung, Leitung, Öffentlichkeit?>

**Nutzenversprechen.** <Was ist nach der Umsetzung besser? Wenn möglich mit einer Größenordnung: Zeit pro Vorgang, Häufigkeit pro Woche, Zahl der Beteiligten.>

**Häufigkeit und Umfang.** <Wie oft fällt der Fall an? Wie lang ist ein typischer Vorgang?>

**Datenbedarf.** <Welche Angaben braucht eine korrekte Antwort, und wo liegen sie heute?>

**Abgrenzung.** <Was gehört ausdrücklich nicht dazu? Welche Entscheidung bleibt in jedem Fall bei einem Menschen?>

---

## Teil 2 — Prompt- und Context-Pipeline

Die dokumentierte Bauweise: Was geht in welcher Form an das Modell, und woher stammen die Fakten?

### Auftragskarte aus Modul 2

Diese Auftragskarte entsteht in der Musterlektion und gehört zu Teil 2. Sie ist eine Planungshilfe; das tatsächliche Material und die vollständigen Prompts werden darunter ergänzt.

| Feld | Eintrag |
|---|---|
| **Der Fall** — welcher wiederkehrende Schreibanlass? | <z. B. Anfragen zu Lieferzeiten von Ersatzteilen, mehrmals pro Woche> |
| **Aufgabe** — gewünschtes Ergebnis | <z. B. Entwirf eine Antwort-Mail auf die folgende Anfrage.> |
| **Materialherkunft** — woher kommen die Fakten? | <z. B. Auszug aus der Konditionsübersicht, als Text in den Prompt eingefügt> |
| **Format** — Textsorte, Länge, Aufbau | <z. B. E-Mail, höchstens 150 Wörter, am Ende eine Liste „Offen"> |
| **Grenzen** — was passiert bei einer fehlenden Angabe? | <z. B. nicht beantworten, sondern unter „Offen" auflisten> |
| **Prüfung vor dem Versand** — wie geht der Entwurf hinaus? | <z. B. gegen das Material lesen, korrigieren, selbst versenden> |

---



**Der Arbeitsauftrag im Wortlaut.** <Den fertigen Prompt vollständig einfügen, mit den vier Teilen Aufgabe, Material, Format, Grenzen.>

**Gespeicherte Anweisungen, soweit verwendet.** <Was ist dauerhaft hinterlegt, etwa als Projekt-Anweisung oder System-Prompt, statt bei jedem Durchlauf neu eingetippt zu werden?>

**Kontextquellen.**

| Quelle | Woher | Wie eingebunden | Wie aktuell gehalten |
|---|---|---|---|
| <z. B. Konditionsübersicht> | <z. B. Intranet-Seite, PDF> | <z. B. relevanter Abschnitt in den Prompt kopiert> | <z. B. bei jeder Preisänderung> |

**Übungsmaterial im Wortlaut.** <Die freigegebenen beziehungsweise synthetischen Ausgangstexte einfügen oder beilegen; Herkunft allein genügt nicht.>

**Entwicklungsschritte.** <Zwei bis vier Durchläufe, jeweils: welcher Prompt wurde verwendet, was wurde verändert und was wurde beobachtet? Mindestens eine unveränderte Wiederholung festhalten. Wenige Durchläufe erlauben keine sichere Ursachenzuordnung.>

---

## Teil 3 — Qualitäts- und Compliance-Check

**Testfälle.** Mindestens fünf, darunter ein Fall mit einer Lücke im Material und ein Fall, der außerhalb des vorgesehenen Bereichs liegt.

| # | Eingabe (kurz) | Erwartetes Ergebnis | Tatsächliches Ergebnis | Bestanden? |
|---|---|---|---|---|
| 1 | <Standardfall> | <...> | <...> | <ja/nein> |
| 2 | <Fall mit fehlender Angabe> | <steht unter „Offen"> | <...> | <ja/nein> |
| 3 | <Fall außerhalb des Bereichs> | <wird abgelehnt oder ausgewiesen> | <...> | <ja/nein> |
| 4 | <...> | <...> | <...> | <ja/nein> |
| 5 | <...> | <...> | <...> | <ja/nein> |

**Prüfkriterien.** <Woran wird „gut" festgemacht? Belegbarkeit jeder Aussage, Vollständigkeit, Form, Ton.>

**Übertragbarkeit.** <Derselbe Auftrag in einem zweiten Werkzeug: Was war anders, was blieb gleich? Kein Ranking, sondern eine Beobachtung am eigenen Fall.>

**Risiko-Orientierung.** Keine Konformitätserklärung, sondern eine geordnete Einschätzung mit den offenen Punkten:

| Feld | Einschätzung | Wer klärt das verbindlich? |
|---|---|---|
| Personenbezogene Daten im Prozess | <welche, in welchem Schritt, wie ersetzt> | <z. B. Datenschutzbeauftragte> |
| Genutztes Konto / Vertragslage | <privat, geschäftlich, welche Vereinbarung besteht> | <z. B. IT, Einkauf> |
| Rechte an Eingaben und Ergebnissen | <fremde Inhalte im Material? Weiterverwendung des Ergebnisses?> | <z. B. Rechtsabteilung> |
| Transparenz gegenüber Empfängern | <wird der KI-Einsatz kenntlich gemacht, und wo?> | <z. B. Führungskraft> |
| Verbleibende Risiken | <was bleibt offen, und wie wird damit umgegangen?> | <...> |

---

## Teil 4 — Transferplan

**Erste 30 Tage.** <Welche zwei bis drei Schritte werden konkret umgesetzt? Mit Datum und verantwortlicher Rolle.>

**Beteiligte.** <Wer muss zustimmen, wer muss informiert werden, wer nutzt es mit?>

**Woran wird der Erfolg gemessen?** <Eine Kennzahl oder Beobachtung, die nach vier Wochen prüfbar ist.>

**Was den Plan scheitern lassen könnte.** <Ehrlich: fehlende Freigabe, fehlende Zeit, unklare Datenlage, Widerstand im Team.>

**Wann wird nachgesteuert?** <Fester Termin für einen Rückblick.>

---

## Termine und Ablauf

| Wann | Was |
|---|---|
| 18.09.2026, 13:00–17:00 (Präsenz) | Kickoff. Teil 1 und die Auftragskarte in Teil 2 entstehen im Termin. |
| 23.09.2026, Vorabend | Zwischenstand einreichen: Teil 1 und der Prompt aus Teil 2. |
| 24.09.2026, 17:30–18:30 (online) | Beratungstermin. Besprechung der kurzen individuellen Rückmeldung zum eingereichten Stand. |
| 29.09.2026, Vorabend | Zwischenstand einreichen: Teil 2 vollständig, Testfälle aus Teil 3 begonnen. |
| 30.09.2026, 17:30–18:30 (online, optional) | Zweiter Beratungstermin. |
| 08.10.2026, 17:30–19:00 (online) | Recap, Abgabe der Mappe, Kurzpräsentation. |

**Kurzpräsentation:** 5 Minuten als Planwert, entlang der vier Teile. Keine gestaltete Foliensammlung nötig; die Mappe selbst darf gezeigt werden.

**Bewertungsgrundlage** laut Modulbeschreibung: fachlicher Nutzen, Qualität der Ergebnisse, sichere Umsetzung und Nachvollziehbarkeit des Transferplans. Die genaue Bewertungsform (Pass/Fail oder Note) ist mit der HdM-Weiterbildung noch zu bestätigen und wird vor dem Kickoff nachgetragen.

**Rückmeldung im Kurs:** Freitexte werden nicht automatisch fachlich bewertet. Die Lernplattform gibt Rückmeldung zu Auswahlaufgaben; inhaltliche Rückmeldung kommt vom Lehrenden vor und in den Beratungsterminen.
