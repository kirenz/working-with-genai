# Prompt-Fassungen v1 bis v4: derselbe Auftrag, vier Stände

Kursmaterial „Working with GenAI", Modul 2, Lektion 2.3. Zu jeder Fassung steht, was gegenüber der vorherigen geändert wurde. Genau eine Änderung je Schritt. Die Fassungen gehören zu **Portfolio-Teil 2** (Arbeitsauftrag im Wortlaut und Entwicklungsschritte).

Die Kundenanfrage ist in allen Fassungen dieselbe (`kundenanfrage-2.txt`). Sie wird hier mit `[Kundenanfrage 2 im Wortlaut]` abgekürzt; im echten Prompt steht sie vollständig.

---

## Fassung v1: der Zuruf

```text
Beantworte diese Kundenanfrage freundlich im Stil unseres Kundenservice.

[Kundenanfrage 2 im Wortlaut]
```

Kein Material, kein Format, keine Grenzen. Ergebnis siehe `durchlauf-1-entwurf.txt`.

---

## Fassung v2: Material und Grenzen ergänzt

**Geändert:** Die Fachinformationen kommen als Material hinein, dazu die Grenze „nur Material, Lücken unter Offen".

```text
Du unterstützt den Kundenservice der Rösterei Morgenrot.

AUFGABE
Entwirf eine Antwort-Mail auf die unten stehende Kundenanfrage.

MATERIAL (nur diese Angaben sind gültig)
Fachinformationen:
- Sortiment im Onlineshop, reguläre Listenpreise: Espresso Intenso 10,00 EUR, Filterkaffee Mild 9,00 EUR, Entkoffeiniert Sanft 13,00 EUR. Zu Preisen innerhalb des Kaffee-Abos liegen hier keine Angaben vor.
- Kaffee-Abo, Sorten: Alle drei Sorten sind im Abo wählbar.
- Kaffee-Abo, Aussetzen: Eine einzelne Lieferung kann ausgesetzt werden, wenn die Anfrage spätestens fünf Werktage vor deren Versand eingeht. Das Abo läuft danach unverändert weiter.
- Für Versandtermine und Sendungsstatus ist der Bereich Lager und Versand zuständig.
- Zu Herkunft, Anbau, Zertifikaten (etwa Bio) und Röstverfahren liegen dem Kundenservice keine freigegebenen Angaben vor.

Kundenanfrage:
[Kundenanfrage 2 im Wortlaut]

GRENZEN
- Verwende ausschließlich Angaben aus dem Material. Ergänze nichts.
- Fragen, die das Material nicht abdeckt, nicht beantworten, sondern unter "Offen" eintragen.
```

---

## Fassung v3: Bedingung und Handlungsverbot

**Geändert:** Zwei Zeilen unter GRENZEN ergänzt. Sonst identisch mit v2.

```text
GRENZEN
- Verwende ausschließlich Angaben aus dem Material. Ergänze nichts.
- Fragen, die das Material nicht abdeckt, nicht beantworten, sondern unter "Offen" eintragen.
- Eine Bedingung steht im selben Satz wie die Zusage. Hängt sie an einer Angabe, die fehlt (etwa einem Versanddatum), nenne die fehlende Angabe.
- Behaupte keine erledigte oder veranlasste Handlung.
```

---

## Fassung v4: Format über ein Musterbeispiel

**Geändert:** Ein Block FORMAT mit Musterbeispiel eingefügt (aus Lektion 2.2). Sonst identisch mit v3. Die vollständige Fassung v4 entspricht `prompt-beispiel-format.txt`, ergänzt um die zwei Grenzzeilen aus v3.

```text
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

Zusätzlich: höchstens 120 Wörter, je Frage ein eigener Absatz. Am Ende, nach der Signatur, eine Liste mit der Überschrift "Offen".
```

---

## Warum die Reihenfolge so ist

1. **Belegbarkeit vor allem anderen (v2).** Ein schöner Text mit erfundener Bio-Aussage ist nicht verwendbar, ein sperriger Text ohne erfundene Aussagen schon.
2. **Bedingung und Handlung (v3).** Eine unbedingte Zusage und eine behauptete Handlung wirken nach außen, sobald die Mail verschickt wird.
3. **Form zuletzt (v4).** Anrede, Signatur und Länge lassen sich am Ende am schnellsten reparieren und verdecken bis dahin keine inhaltlichen Fehler.

Diese Reihenfolge ist eine Empfehlung dieses Kurses, keine belegte Regel. Sie folgt aus der Frage, welcher Fehler am teuersten wäre, wenn er durchrutscht.
