# Prompt-Fassungen v1 bis v4: derselbe Auftrag, vier Stände

Kursmaterial „Working with GenAI", Modul 2, Lektion 2.4 „Im Dialog weiterarbeiten“. Zu jeder Fassung steht, was gegenüber der vorherigen geändert wurde. Ein Änderungsschwerpunkt je Schritt. Die Fassungen gehören zu **Portfolio-Teil 2** (Arbeitsauftrag im Wortlaut und Entwicklungsschritte).

Die Kundenanfrage ist in allen Fassungen vollständig enthalten. v1 ist bewusst unzureichend und dient nur als Vergleich. v2 bis v4 sind kopierbare vollständige Arbeitsaufträge. Die Änderungen betreffen jeweils einen Schwerpunkt; dieser kann mehrere zusammengehörige Zeilen umfassen.

---

## Fassung v1: der Zuruf

```text
Beantworte diese Kundenanfrage freundlich im Stil unseres Kundenservice.

Betreff: Abo im Oktober aussetzen

Guten Tag,

ich bin im Oktober drei Wochen unterwegs und möchte meine Abo-Lieferung in
dieser Zeit aussetzen. Geht das, und was muss ich dafür tun? Außerdem: Gibt
es Entkoffeiniert Sanft auch im Abo? Und ist Ihr Kaffee eigentlich Bio?

Beste Grüße
R. Novak

--------------------------------------------------------------------------
DREI FRAGEN, DREI ANTWORTLAGEN
--------------------------------------------------------------------------

1. Lieferung aussetzen ............. bedingt belegbar. Die Regel steht im
                                     Auszug (fünf Werktage vor dem Versand).
                                     Das Versanddatum der Oktober-Lieferung
                                     fehlt; ob die Frist zu halten ist,
                                     bleibt offen.
2. Entkoffeiniert Sanft im Abo ..... belegbar: alle drei Sorten sind im Abo
                                     wählbar.
3. Bio ............................. NICHT belegbar. Der Auszug sagt
                                     ausdrücklich, dass dem Kundenservice
                                     dazu keine freigegebenen Angaben
                                     vorliegen. Weder "ja" noch "nein" darf
                                     im Entwurf stehen.
```

Bewusst unzureichend: keine Fachinformationen, kein festgelegtes Format, kein Check. Konstruiertes Vergleichsergebnis siehe `durchlauf-1-entwurf.txt`.

---

## Fassung v2: Context und Check ergänzt

**Geändert:** Die Fachinformationen kommen als Context hinein, dazu die Check-Zeile „nur Context, Lücken unter Offen".

```text
TASK
Entwirf eine Antwort-Mail auf die unten stehende Kundenanfrage.

CONTEXT
Du unterstützt den Kundenservice der Rösterei Morgenrot. Gültig sind ausschließlich die folgenden Angaben.

Fachinformationen:
- Sortiment im Onlineshop, reguläre Listenpreise: Espresso Intenso 10,00 EUR, Filterkaffee Mild 9,00 EUR, Entkoffeiniert Sanft 13,00 EUR. Zu Preisen innerhalb des Kaffee-Abos liegen hier keine Angaben vor.
- Kaffee-Abo, Sorten: Alle drei Sorten sind im Abo wählbar.
- Kaffee-Abo, Aussetzen: Eine einzelne Lieferung kann ausgesetzt werden, wenn die Anfrage spätestens fünf Werktage vor deren Versand eingeht. Das Abo läuft danach unverändert weiter.
- Für Versandtermine und Sendungsstatus ist der Bereich Lager und Versand zuständig.
- Zu Herkunft, Anbau, Zertifikaten (etwa Bio) und Röstverfahren liegen dem Kundenservice keine freigegebenen Angaben vor.

Kundenanfrage:
Betreff: Abo im Oktober aussetzen

Guten Tag,

ich bin im Oktober drei Wochen unterwegs und möchte meine Abo-Lieferung in
dieser Zeit aussetzen. Geht das, und was muss ich dafür tun? Außerdem: Gibt
es Entkoffeiniert Sanft auch im Abo? Und ist Ihr Kaffee eigentlich Bio?

Beste Grüße
R. Novak

--------------------------------------------------------------------------
DREI FRAGEN, DREI ANTWORTLAGEN
--------------------------------------------------------------------------

1. Lieferung aussetzen ............. bedingt belegbar. Die Regel steht im
                                     Auszug (fünf Werktage vor dem Versand).
                                     Das Versanddatum der Oktober-Lieferung
                                     fehlt; ob die Frist zu halten ist,
                                     bleibt offen.
2. Entkoffeiniert Sanft im Abo ..... belegbar: alle drei Sorten sind im Abo
                                     wählbar.
3. Bio ............................. NICHT belegbar. Der Auszug sagt
                                     ausdrücklich, dass dem Kundenservice
                                     dazu keine freigegebenen Angaben
                                     vorliegen. Weder "ja" noch "nein" darf
                                     im Entwurf stehen.

FORMAT
Eine freundliche Antwort-Mail; darunter eine Liste "Offen".

CHECK
- Fragen, die der Context nicht abdeckt, nicht beantworten, sondern unter "Offen" eintragen.
- Verwende ausschließlich Angaben aus dem Context. Ergänze nichts.
```

---

## Fassung v3: Bedingung und Handlungsverbot

**Geändert:** Zwei Zeilen unter CHECK ergänzt. Sonst identisch mit v2.

```text
TASK
Entwirf eine Antwort-Mail auf die unten stehende Kundenanfrage.

CONTEXT
Du unterstützt den Kundenservice der Rösterei Morgenrot. Gültig sind ausschließlich die folgenden Angaben.

Fachinformationen:
- Sortiment im Onlineshop, reguläre Listenpreise: Espresso Intenso 10,00 EUR, Filterkaffee Mild 9,00 EUR, Entkoffeiniert Sanft 13,00 EUR. Zu Preisen innerhalb des Kaffee-Abos liegen hier keine Angaben vor.
- Kaffee-Abo, Sorten: Alle drei Sorten sind im Abo wählbar.
- Kaffee-Abo, Aussetzen: Eine einzelne Lieferung kann ausgesetzt werden, wenn die Anfrage spätestens fünf Werktage vor deren Versand eingeht. Das Abo läuft danach unverändert weiter.
- Für Versandtermine und Sendungsstatus ist der Bereich Lager und Versand zuständig.
- Zu Herkunft, Anbau, Zertifikaten (etwa Bio) und Röstverfahren liegen dem Kundenservice keine freigegebenen Angaben vor.

Kundenanfrage:
Betreff: Abo im Oktober aussetzen

Guten Tag,

ich bin im Oktober drei Wochen unterwegs und möchte meine Abo-Lieferung in
dieser Zeit aussetzen. Geht das, und was muss ich dafür tun? Außerdem: Gibt
es Entkoffeiniert Sanft auch im Abo? Und ist Ihr Kaffee eigentlich Bio?

Beste Grüße
R. Novak

--------------------------------------------------------------------------
DREI FRAGEN, DREI ANTWORTLAGEN
--------------------------------------------------------------------------

1. Lieferung aussetzen ............. bedingt belegbar. Die Regel steht im
                                     Auszug (fünf Werktage vor dem Versand).
                                     Das Versanddatum der Oktober-Lieferung
                                     fehlt; ob die Frist zu halten ist,
                                     bleibt offen.
2. Entkoffeiniert Sanft im Abo ..... belegbar: alle drei Sorten sind im Abo
                                     wählbar.
3. Bio ............................. NICHT belegbar. Der Auszug sagt
                                     ausdrücklich, dass dem Kundenservice
                                     dazu keine freigegebenen Angaben
                                     vorliegen. Weder "ja" noch "nein" darf
                                     im Entwurf stehen.

FORMAT
Eine freundliche Antwort-Mail; darunter eine Liste "Offen".

CHECK
- Fragen, die der Context nicht abdeckt, nicht beantworten, sondern unter "Offen" eintragen.
- Eine Bedingung steht im selben Satz wie die Zusage. Hängt sie an einer fehlenden Angabe, nenne die fehlende Angabe.
- Behaupte keine erledigte oder veranlasste Handlung.
- Verwende ausschließlich Angaben aus dem Context. Ergänze nichts.
```

---

## Fassung v4: Format über ein Musterbeispiel

**Geändert:** Der einfache FORMAT-Block durch ein Musterbeispiel ergänzt (aus Lektion 2.3). Sonst identisch mit v3. Die vollständige Fassung v4 entspricht `prompt-beispiel-format.txt`, ergänzt um die zwei Check-Zeilen aus v3.

```text
TASK
Entwirf eine Antwort-Mail auf die unten stehende Kundenanfrage.

CONTEXT
Du unterstützt den Kundenservice der Rösterei Morgenrot. Gültig sind ausschließlich die folgenden Angaben.

Fachinformationen:
- Sortiment im Onlineshop, reguläre Listenpreise: Espresso Intenso 10,00 EUR, Filterkaffee Mild 9,00 EUR, Entkoffeiniert Sanft 13,00 EUR. Zu Preisen innerhalb des Kaffee-Abos liegen hier keine Angaben vor.
- Kaffee-Abo, Sorten: Alle drei Sorten sind im Abo wählbar.
- Kaffee-Abo, Aussetzen: Eine einzelne Lieferung kann ausgesetzt werden, wenn die Anfrage spätestens fünf Werktage vor deren Versand eingeht. Das Abo läuft danach unverändert weiter.
- Für Versandtermine und Sendungsstatus ist der Bereich Lager und Versand zuständig.
- Zu Herkunft, Anbau, Zertifikaten (etwa Bio) und Röstverfahren liegen dem Kundenservice keine freigegebenen Angaben vor.

Kundenanfrage:
Betreff: Abo im Oktober aussetzen
Guten Tag,
ich bin im Oktober drei Wochen unterwegs und möchte meine Abo-Lieferung in dieser Zeit aussetzen. Geht das, und was muss ich dafür tun? Außerdem: Gibt es Entkoffeiniert Sanft auch im Abo? Und ist Ihr Kaffee eigentlich Bio?
Beste Grüße
R. Novak

FORMAT
Übernimm Aufbau und Ton des folgenden Beispiels, nicht seinen Inhalt. Das Beispiel beantwortet andere Fragen.

BEISPIEL (Hausstil)
Guten Tag,

vielen Dank für Ihre Nachricht.

Ihr Abo können Sie jederzeit per Mail an uns kündigen; bereits versendete Lieferungen sind davon nicht betroffen.

Zum Versandstatus Ihrer aktuellen Lieferung liegt mir hier keine Angabe vor. Dafür ist unser Bereich Lager und Versand zuständig; Sie erhalten dazu eine gesonderte Rückmeldung.

Freundliche Grüße
Sina Bergmann
Vertrieb und Kundenservice, Rösterei Morgenrot
ENDE BEISPIEL

Zusätzlich: höchstens 120 Wörter, je Frage ein eigener Absatz, eine Bedingung steht im selben Satz wie die Zusage. Am Ende, nach der Signatur, eine Liste mit der Überschrift "Offen".

CHECK
- Fragen, die der Context nicht abdeckt, nicht beantworten, sondern im Text als nicht vorliegend benennen und unter "Offen" eintragen.
- Hängt eine Bedingung an einer fehlenden Angabe, nenne die fehlende Angabe.
- Verwende ausschließlich Angaben aus dem Context. Ergänze nichts.
- Behaupte keine erledigte oder veranlasste Handlung. Erfinde keine Termine, Preise oder Fristen.
```

---

## Warum die Reihenfolge so ist

1. **Belegbarkeit vor allem anderen (v2).** Ein schöner Text mit erfundener Bio-Aussage ist nicht verwendbar, ein sperriger Text ohne erfundene Aussagen schon.
2. **Bedingung und Handlung (v3).** Eine unbedingte Zusage und eine behauptete Handlung wirken nach außen, sobald die Mail verschickt wird.
3. **Form zuletzt (v4).** Anrede, Signatur und Länge lassen sich am Ende am schnellsten reparieren und verdecken bis dahin keine inhaltlichen Fehler.

Diese Reihenfolge ist eine Empfehlung dieses Kurses, keine belegte Regel. Sie folgt aus der Frage, welcher Fehler am teuersten wäre, wenn er durchrutscht.
