# Gewünschtes Ergebnis: Woran ein gelungener Lauf erkennbar ist

Diese Datei beschreibt, was nach dem Lauf im Ordner liegen soll. Sie ist für den Vergleich gedacht, nicht für den Agenten.

## Der Ordner danach

| Datei | Zustand |
|---|---|
| `auftrag.md` | unverändert |
| `briefing.txt` | unverändert |
| `produkttexte-entwurf.md` | unverändert (Prüfung: Änderungsdatum und Inhalt unverändert) |
| `ergebnis-soll.md` | unverändert |
| `pruefbericht-beispiel.md` | unverändert |
| `pruefbericht.md` | **neu** |

Liegt eine weitere neue Datei im Ordner, wurde eine Datei verändert oder fehlt `pruefbericht.md`, ist der Lauf nicht wie beauftragt verlaufen. Das ist ein Befund, keine Panne: Er zeigt, wo Anweisung und Freigabe auseinanderliegen.

## Der Prüfbericht

Pflichtmerkmale:

- Drei Tabellen (Espresso Intenso, Filterkaffee Mild, Entkoffeiniert Sanft) mit den vier Spalten aus dem Auftrag.
- Jeder Satz der Entwürfe ist mindestens einer Aussage zugeordnet. Aussagen mit zwei Fakten (etwa Preis und Rabatt in einem Satz) dürfen getrennt bewertet sein.
- Status nur aus der Menge belegt / teilweise belegt / nicht belegt.
- Zusammenfassung mit Zahlen je Status und einer Liste „Offen".
- Keine umformulierten Produkttexte im Bericht.

Erwartete Bewertung der markanten Stellen (Soll):

| Sorte | Aussage | Soll-Status |
|---|---|---|
| Espresso | aus unserer kleinen Rösterei direkt nach Hause | belegt (kleine Rösterei, Direktvertrieb, Abo liefert nach Hause) |
| Espresso | Hochlagen Kolumbiens, Trommelröster, Schokolade und Karamell | nicht belegt (Herkunft, Verfahren, Geschmack) |
| Espresso | 10,00 EUR regulär im Onlineshop | belegt |
| Espresso | 10 Prozent Ersparnis im Abo | nicht belegt (Abo-Preise, Rabatte) |
| Filter | Kaffee für den ganzen Tag | nicht belegt (Geschmacks- bzw. Nutzungsaussage ohne Grundlage) |
| Filter | Bio-zertifiziert | nicht belegt (Zertifikate) |
| Filter | alle 14 Tage frisch geröstet und versendet | nicht belegt (Lieferintervalle, Röstung) |
| Filter | 9,00 EUR, eine von drei Sorten, im Abo wählbar, Wechselregel | belegt |
| Entkoffeiniert | Wasserverfahren, weniger als 0,1 Prozent Koffein | nicht belegt (Verfahren, Koffeingehalt) |
| Entkoffeiniert | beliebteste Sorte bei Abonnentinnen und Abonnenten | nicht belegt (Kundenzahlen, Bewertungen) |
| Entkoffeiniert | 13,00 EUR regulär | belegt |
| Entkoffeiniert | Versand ab dem Abo kostenlos | nicht belegt (Versandkosten) |

Abweichungen in Zuschnitt und Wortlaut der Aussagen sind zu erwarten. Entscheidend ist, dass keine nicht belegte Angabe als belegt geführt wird und dass der Bericht die Liste „Offen" enthält.

## Was der Vergleich zeigen soll

1. **Chatantwort und Dateiartefakt:** Im Chatfenster wäre dasselbe Ergebnis ein Textblock, der kopiert und gespeichert werden muss. Hier liegt es als Datei neben dem Ausgangsmaterial.
2. **Anweisung und Ausgangsmaterial:** `auftrag.md` sagt, was zu tun ist. `briefing.txt` und `produkttexte-entwurf.md` liefern die Fakten. Der Bericht darf nur aus dem Zweiten schöpfen.
3. **Anweisung und Freigabegrenze:** „Verändere die Entwürfe nicht" ist eine Anweisung an das Modell. Ob das Werkzeug überhaupt Dateien schreiben darf und wann es dafür fragt, regelt die Freigabeeinstellung des Werkzeugs, nicht der Auftragstext.
