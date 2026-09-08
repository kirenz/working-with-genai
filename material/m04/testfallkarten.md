# Testfallkarten: Kundenservice-Auftrag Rösterei Morgenrot

Kursmaterial „Working with GenAI“, Lektion 4.2. Fünf feste Testfallkarten für den Arbeitsauftrag aus Modul 2 (`prompt-vorlage.txt`). Die Kundenmail im Abschnitt „Kundenanfrage“ des Auftrags wird je Testfall durch die Eingabe der Karte ersetzt; Aufgabe, Material, Format und Grenzen bleiben unverändert.

**Kennzeichnung:** synthetisch. Die fünf Falltypen sind eine Designentscheidung dieses Kurses. Alle Kundenmails sind erfunden.

**Lesart der Karten:** Eine Karte gilt als bestanden, wenn alle Kriterien unter „Erfüllt, wenn“ zutreffen. Ein einzelner bestandener Durchlauf sagt nur, dass es in diesem Durchlauf geklappt hat. Zwei oder drei Durchläufe je Karte zeigen, ob das Ergebnis schwankt; sie sind kein Nachweis von Zuverlässigkeit.

---

## T1 · Normalfall

**Falltyp:** Die Frage ist vollständig durch das Material gedeckt.

**Eingabe (Kundenmail):**

```text
Betreff: Preis Entkoffeiniert Sanft
Guten Tag,
was kostet der Entkoffeiniert Sanft regulär im Onlineshop? Ich möchte ihn einmal
ohne Abo probieren.
Viele Grüße
R. Winter
```

**Erwartung:** Der Preis wird genannt, als regulärer Listenpreis im Onlineshop, ohne Zusätze.

**Erfüllt, wenn:**

- [ ] K1 Der Entwurf nennt 13,00 EUR.
- [ ] K2 Der Preis ist als regulärer Listenpreis im Onlineshop bezeichnet, nicht als Abo-Preis oder Aktionspreis.
- [ ] K3 Der Entwurf enthält keine Aussage, die nicht im Material steht (keine Packungsgröße, keine Versandkosten, kein Lieferdatum).
- [ ] K4 Die Liste „Offen“ ist leer oder nennt nur Punkte, die die Kundin tatsächlich gefragt hat und die das Material nicht deckt.

**Nicht erfüllt, wenn** ein anderer Preis, ein Abo-Preis oder eine Angabe zu Packungsgröße oder Versand erscheint.

---

## T2 · Bedingung

**Falltyp:** Die Antwort gilt nur unter einer Bedingung, die das Material nennt.

**Eingabe (Kundenmail):**

```text
Betreff: Wechsel auf Espresso
Guten Tag,
ich habe den Filterkaffee Mild im Abo und möchte ab der nächsten Lieferung auf
Espresso Intenso wechseln. Geht das?
Viele Grüße
T. Osei
```

**Erwartung:** Der Wechsel wird als möglich beschrieben, aber ausdrücklich an die Fünf-Werktage-Bedingung geknüpft; ob er für die nächste Lieferung greift, bleibt offen, weil das Versanddatum fehlt.

**Erfüllt, wenn:**

- [ ] K1 Der Entwurf nennt die Bedingung „spätestens fünf Werktage vor dem Versand“.
- [ ] K2 Der Entwurf sagt nicht unbedingt zu, dass der Wechsel schon die nächste Lieferung betrifft.
- [ ] K3 Das fehlende Versanddatum steht unter „Offen“.
- [ ] K4 Kein Versanddatum und keine Frist wird erfunden.

**Nicht erfüllt, wenn** der Wechsel ohne Bedingung für die nächste Lieferung zugesagt oder ein Versandtermin genannt wird.

---

## T3 · Fehlende Angabe

**Falltyp:** Das Material enthält zur Frage nichts.

**Eingabe (Kundenmail):**

```text
Betreff: Paket unterwegs?
Guten Tag,
meine Abo-Lieferung ist noch nicht da. Können Sie mir sagen, wann sie verschickt
wurde und ob sie diese Woche noch ankommt?
Viele Grüße
L. Brandt
```

**Erwartung:** Keine Auskunft zum Versand. Beide Fragen stehen unter „Offen“, mit dem Hinweis, dass Lager und Versand zuständig ist.

**Erfüllt, wenn:**

- [ ] K1 Kein Versanddatum, kein Ankunftstag, keine „üblichen“ Laufzeiten werden genannt.
- [ ] K2 Versanddatum und Ankunft stehen unter „Offen“.
- [ ] K3 Der Entwurf behauptet nicht, dass bereits nachgefragt oder nachgeschaut wurde.
- [ ] K4 Die Zuständigkeit von Lager und Versand wird als Zuständigkeit genannt, nicht als Auskunft über die Sendung.

**Nicht erfüllt, wenn** ein Termin, eine Laufzeit oder ein Sendungsstatus im Text steht.

---

## T4 · Widerspruch

**Falltyp:** Die Eingabe behauptet etwas, das dem Material widerspricht.

**Eingabe (Kundenmail):**

```text
Betreff: Preis stimmt nicht
Guten Tag,
auf Ihrer Website stand letzte Woche 8,50 EUR für den Filterkaffee Mild. Jetzt
sehe ich 9,00 EUR. Welcher Preis gilt, und bekomme ich die Differenz zurück?
Viele Grüße
A. Kaya
```

**Erwartung:** Der Entwurf nennt den Preis aus dem Material (9,00 EUR) als regulären Listenpreis, entscheidet aber nicht, ob die Kundin recht hat, und sagt keine Erstattung zu. Der behauptete Preis und die Erstattungsfrage stehen unter „Offen“.

**Erfüllt, wenn:**

- [ ] K1 Der Entwurf nennt 9,00 EUR als regulären Listenpreis laut Material.
- [ ] K2 Der Entwurf behauptet nicht, dass es nie 8,50 EUR gab, und bestätigt es auch nicht.
- [ ] K3 Keine Erstattung wird zugesagt oder abgelehnt.
- [ ] K4 „Angabe der Kundin 8,50 EUR“ und „Erstattung“ stehen unter „Offen“ zur Klärung.

**Nicht erfüllt, wenn** der Entwurf der Kundin widerspricht, ihr recht gibt oder über die Erstattung entscheidet.

---

## T5 · Außerhalb des Bereichs

**Falltyp:** Die Eingabe liegt außerhalb dessen, wofür der Auftrag gebaut ist.

**Eingabe (Kundenmail):**

```text
Betreff: Großbestellung für unser Büro
Guten Tag,
wir möchten für unser Unternehmen monatlich 40 kg Espresso Intenso beziehen.
Welche Konditionen bieten Sie Geschäftskunden, und können Sie uns eine Rechnung
mit Zahlungsziel stellen?
Viele Grüße
M. Feldmann, Einkauf
```

**Erwartung:** Der Entwurf erkennt, dass das Material nur Endkundinnen und Endkunden im Onlineshop und Abo abdeckt. Er macht keine Konditionen und verweist die Anfrage zur Klärung weiter; alle Fragen stehen unter „Offen“.

**Erfüllt, wenn:**

- [ ] K1 Keine Mengenrabatte, Geschäftskundenpreise oder Zahlungsziele werden genannt oder in Aussicht gestellt.
- [ ] K2 Der Entwurf sagt, dass das Anliegen außerhalb der vorliegenden Angaben liegt und intern geklärt wird.
- [ ] K3 Alle drei Fragen (Konditionen, Rechnung, Zahlungsziel) stehen unter „Offen“.
- [ ] K4 Der Shop-Listenpreis wird höchstens als Shop-Preis genannt, nicht als Angebot für 40 kg.

**Nicht erfüllt, wenn** Konditionen, Rabatte oder Zahlungsmodalitäten im Text stehen.

---

## Eintragsvorlage

Für jede Karte und jeden Durchlauf eine Zeile. Zwei Durchläufe je Karte sind der Planwert im Kurs.

| Karte | Falltyp | Durchlauf | Datum | Werkzeug | Erfüllte Kriterien (K1 bis K4) | Befund in einem Satz | Bestanden |
|---|---|---|---|---|---|---|---|
| T1 | Normalfall | 1 | | | | | |
| T1 | Normalfall | 2 | | | | | |
| T2 | Bedingung | 1 | | | | | |
| T2 | Bedingung | 2 | | | | | |
| T3 | Fehlende Angabe | 1 | | | | | |
| T3 | Fehlende Angabe | 2 | | | | | |
| T4 | Widerspruch | 1 | | | | | |
| T4 | Widerspruch | 2 | | | | | |
| T5 | Außerhalb des Bereichs | 1 | | | | | |
| T5 | Außerhalb des Bereichs | 2 | | | | | |

**Auswertung in drei Sätzen:** Welche Karte ist in beiden Durchläufen bestanden? Welche in keinem? Welche schwankt? Ein Schwanken ist ein Befund über die Aufgabe, nicht über die Zuverlässigkeit des Werkzeugs; dafür wären deutlich mehr Durchläufe nötig, als dieser Kurs vorsieht.

## Leere Karte für den eigenen Fall

```text
TESTFALLKARTE T_ · Falltyp: (Normalfall / Bedingung / Fehlende Angabe /
Widerspruch / Außerhalb des Bereichs)

Eingabe:
(erfundene Anfrage im Wortlaut)

Erwartung:
(ein bis zwei Sätze: was soll der Entwurf tun, was nicht)

Erfüllt, wenn:
[ ] K1
[ ] K2
[ ] K3
[ ] K4 (optional)

Nicht erfüllt, wenn:
(der eine Fehler, der diese Karte scheitern lässt)
```
