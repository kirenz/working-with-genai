# Kriterien nach Ergebnisart

Kursmaterial „Working with GenAI“, Lektion 4.1 · Was ein gutes KI-Ergebnis ausmacht

Vier Karten als Arbeitshilfe. Die Einteilung ist eine Entscheidung dieses Kurses und keine Norm; für andere Aufgaben kommen andere Kriterien dazu. Alle Beispiele sind erfunden und beziehen sich auf die Rösterei Morgenrot.

**Vor jedem Ergebnis:** Was behauptet dieser Text über die Welt, und woran ließe sich das prüfen? Wozu wird das Ergebnis gebraucht?

---

## Karte A · Auskunft nach Aktenlage

Eine Antwort, die sich auf festgelegtes Material stützt: Kundenauskunft, Auszug aus einer Regelung, Sachstand.

- [ ] Jede inhaltliche Aussage ist im mitgegebenen Material gedeckt.
- [ ] Lücken sind ausgewiesen und nicht gefüllt.
- [ ] Widersprüche zwischen Quellen sind benannt und nicht entschieden.
- [ ] Es wird nichts zugesagt, was das Material nicht trägt.
- [ ] Die vorgegebene Form ist eingehalten (Textsorte, Länge, Aufbau).

Häufiger Befund: eine sachlich richtige Ergänzung, die im Material nicht steht.

---

## Karte B · Zusammenfassung und Strukturierung

Vorhandenes Material wird gekürzt, geordnet oder umgeformt: Besprechungsnotizen, Protokolle, ein Stapel Rückmeldungen.

- [ ] Was für den Zweck zählt, ist enthalten; nichts kommt hinzu.
- [ ] Gewichtungen („Hauptgrund“, „vor allem“) stehen nur im Ergebnis, wenn sie in der Vorlage stehen.
- [ ] Ursachen sind nicht aus nebeneinanderstehenden Beobachtungen abgeleitet.
- [ ] Die Ordnung ist nachvollziehbar und benannt (nach Thema, nach Zeit, nach Zuständigkeit).
- [ ] Eigene Einordnungen sind als solche erkennbar.

Häufiger Befund: eine Wertung, die in der Vorlage nicht vorkommt und im Ergebnis wie ein Befund aussieht.

---

## Karte C · Ideen und Vorschläge

Eine Sammlung von Möglichkeiten: Themen, Wege, Ansätze.

- [ ] Spannweite: verschiedene Ansätze, nicht Varianten desselben Gedankens.
- [ ] Passung: zu Größe, Mitteln und Zuständigkeiten der beschriebenen Lage.
- [ ] Voraussetzungen: erkennbar, was jeder Vorschlag verlangt.
- [ ] **Sachbehauptungen innerhalb der Ideen sind geprüft wie eine Auskunft.**
- [ ] Idee und Begründung sind getrennt beurteilt.

Häufiger Befund: eine brauchbare Idee mit einer erfundenen Begründung. Gestrichen wird die Begründung, nicht die Idee.

---

## Karte D · Vergleich mit Zahlen

Zwei oder mehr Dinge nebeneinander: Angebote, Sorten, Monate, Varianten.

- [ ] Gleiche Bezugsgröße je Spalte: derselbe Zeitraum, dieselbe Einheit, dieselbe Menge.
- [ ] Jede Zelle stammt aus einer benennbaren Quelle.
- [ ] Fehlende Werte stehen als Lücke, nicht als Schätzung.
- [ ] Rechnungen sind nachvollziehbar; der Rechenweg steht dabei oder ist in einem Schritt nachzuvollziehen.
- [ ] Die Zeilen sind vollständig; eine weggelassene Position verändert einen Vergleich stärker als eine falsche Zahl.

Häufiger Befund: zwei Zahlen mit unterschiedlicher Bezugsgröße in derselben Spalte.

---

## Beispiel 1 · Ideensammlung mit Sachbehauptungen

Konstruiert, kein aufgezeichneter Modelloutput. Auftrag war: Ideen, wie sich Rückfragen zum Sortenwechsel verringern lassen.

```text
1. Die Fünf-Werktage-Regel in die Bestätigungsmail des Abos aufnehmen.
2. Ein Feld im Kundenkonto, in dem der Sortenwechsel selbst ausgelöst
   werden kann.
3. Eine Erinnerungsmail sieben Tage vor dem Versand, da erfahrungsgemäß
   rund 60 Prozent der Wechselwünsche zu spät eingehen.
4. Den Wechsel jederzeit zulassen und die Fünf-Werktage-Regel abschaffen,
   wie es im Abo-Handel üblich ist.
```

| Nr. | Was ist Vorschlag? | Was ist Sachbehauptung? | Umgang |
|---|---|---|---|
| 1 | die Aufnahme in die Bestätigungsmail | keine | bleibt; Entscheidung liegt bei der Rösterei |
| 2 | ein Selbstbedienungsfeld im Konto | keine; setzt aber ein Kundenkonto voraus | bleibt; Voraussetzung notieren |
| 3 | die Erinnerungsmail | „rund 60 Prozent der Wechselwünsche gehen zu spät ein“ | Vorschlag bleibt, Zahl streichen oder als zu prüfende Annahme kennzeichnen |
| 4 | den Wechsel jederzeit zulassen | „wie es im Abo-Handel üblich ist“ | Behauptung streichen; zusätzlich prüfen, woran die Fünf-Werktage-Regel hängt (Produktionsplanung) |

Ergebnis: vier brauchbare Vorschläge, zwei gestrichene Sätze. Die Prüfung entfernt selten Ideen, sie entfernt ihre erfundenen Begründungen. Und: Nicht gedeckt heißt nicht falsch. Die 60 Prozent können zutreffen; belegt sind sie nicht, und deshalb tragen sie keine Entscheidung.

---

## Beispiel 2 · Vergleich mit unterschiedlichen Bezugsgrößen

Konstruiert. Zwei Angebote für Beutel mit Aromaventil, alle Angaben erfunden.

**Die Quelle, zwei Angebotsschreiben:**

```text
ANGEBOT NORDHANG VERPACKUNG, 12.08.2026
Beutel 250 g mit Aromaventil, Karton mit 1.000 Stück: 189,00 EUR netto.
Versand pauschal 24,00 EUR netto je Karton. Lieferzeit 10 Werktage.
Mindestabnahme 1 Karton.

ANGEBOT SEITZ & TOECHTER, 14.08.2026
Beutel 250 g mit Aromaventil: 0,21 EUR netto je Stück ab 500 Stück.
Versandkostenfrei ab 2.000 Stück, darunter 29,00 EUR netto.
Lieferzeit 3 Wochen. Mindestabnahme 500 Stück.
```

**Das konstruierte Ergebnis:**

| Merkmal | Nordhang | Seitz & Töchter |
|---|---|---|
| Preis | 189,00 EUR | 0,21 EUR |
| Versand | 24,00 EUR | kostenfrei |
| Lieferzeit | 10 Werktage | 3 Wochen |

**Der Befund:** Die Zeile „Preis“ vergleicht einen Kartonpreis mit einem Stückpreis. Die Zahlen stehen beide so in den Angeboten und sind trotzdem nicht vergleichbar. Die Zeile „Versand“ nennt „kostenfrei“, ohne die Bedingung ab 2.000 Stück; bei 1.000 Stück fielen 29,00 EUR an. Und es fehlt eine Zeile: die Mindestabnahme, die für einen kleinen Betrieb den Ausschlag geben kann.

**Die reparierte Fassung**, bezogen auf 1.000 Stück, mit Rechenweg:

| Merkmal | Nordhang | Seitz & Töchter |
|---|---|---|
| Preis je Stück | 0,189 EUR (189,00 EUR ÷ 1.000) | 0,21 EUR (laut Angebot) |
| Preis 1.000 Stück, netto | 189,00 EUR | 210,00 EUR (1.000 × 0,21 EUR) |
| Versand bei 1.000 Stück | 24,00 EUR | 29,00 EUR (unter 2.000 Stück) |
| Summe 1.000 Stück, netto | 213,00 EUR | 239,00 EUR |
| Lieferzeit | 10 Werktage | 3 Wochen (Angabe in anderer Einheit) |
| Mindestabnahme | 1.000 Stück (1 Karton) | 500 Stück |

Was die reparierte Tabelle leistet: Sie nennt die Bezugsmenge im Kopf jeder Zeile, sie zeigt den Rechenweg, sie führt die fehlende Zeile ein, und sie weist die unterschiedliche Zeiteinheit als solche aus, statt „3 Wochen“ stillschweigend in Werktage umzurechnen.

Was sie nicht leistet: eine Entscheidung. Bei 500 Stück sieht der Vergleich anders aus, und die Frage, ob 1.000 Beutel überhaupt gebraucht werden, beantwortet keine Tabelle.
