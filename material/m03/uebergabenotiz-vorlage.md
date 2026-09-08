# Übergabenotiz für einen neuen Chat

Kursmaterial „Working with GenAI“, Lektion 3.1 · Chatverlauf und Kontextfenster

Eine Übergabenotiz ist der kurze Kopf über der eigentlichen Frage, wenn eine Arbeit in einem neuen Chatfenster fortgesetzt wird. Sie ersetzt den gewachsenen Verlauf durch einen geprüften Zwischenstand. Die Notiz wird außerhalb des Chats gepflegt, in einer Textdatei, und vor jedem Neustart hineinkopiert.

**Datenregel:** Für Übungen ausschließlich erfundene Angaben verwenden. Keine echten Namen, Adressen, Kunden- oder Vertragsnummern.

---

## Vorlage

```text
ÜBERGABENOTIZ
Aufgabe:        <Was soll am Ende herauskommen? Ein Satz.>
Stand:          <Was ist bereits erledigt und geprüft? Zwei bis drei Sätze.>
Gültige Quelle: <Titel, Stand, Herkunft. Eine Zeile je Quelle.>
Nicht gültig:   <Was wurde ausdrücklich verworfen, und warum?>
Regeln:         <Die Vorgaben, die weiter gelten sollen.>
Offen:          <Was ist noch ungeklärt?>

Nächster Schritt:
<Die konkrete Frage oder der konkrete Auftrag.>
```

---

## Ausgefülltes Beispiel aus dem Lehrfall

Konstruiert, erfundene Angaben. Die Ausgangslage ist die aus Lektion 3.1: In einem gewachsenen Chat liegen zwei Fassungen desselben Steckbriefs, und das Ergebnis nennt eine Aufbrauchempfehlung aus der ersetzten Fassung.

```text
ÜBERGABENOTIZ
Aufgabe:        Kurzübersicht der Aufbrauchempfehlungen je Sorte für den
                Kundenservice der Rösterei Morgenrot.
Stand:          Sortenübersicht mit Röstgrad, Bohnen, Geschmacksnoten und
                Zubereitung liegt vor und ist gegen den Steckbrief geprüft.
                Offen ist nur noch die Spalte Aufbrauchempfehlung.
Gültige Quelle: [Q1] Sortensteckbrief Version 3, Stand 21.08.2026,
                Marlene Bosch.
Nicht gültig:   Sortensteckbrief Version 2 vom 12.03.2026. Ersetzt; die
                Aufbrauchempfehlung wurde in Version 3 geändert. Version 2
                wird nicht mitgegeben und nicht als Ersatz verwendet.
Regeln:         Nur Angaben aus [Q1]. Hinter jeder Angabe die Kennung [Q1].
                Fehlendes als "nicht im Material" kennzeichnen. Keine
                Mengen, Termine oder Preise ergänzen. Ergebnis ist ein
                Entwurf.
Offen:          Ob die Übersicht auch im Shop verwendet wird; entscheidet
                Jonas Halder.

Nächster Schritt:
Nenne für jede der drei Sorten die Aufbrauchempfehlung aus [Q1], jeweils
mit Kennung. Wenn eine Sorte keine Angabe hat, schreibe "nicht im Material".

=== DOKUMENT [Q1] BEGINN ===
(vollständiger Text des Sortensteckbriefs Version 3)
=== DOKUMENT [Q1] ENDE ===
```

---

## Wozu die einzelnen Zeilen dienen

| Zeile | Wofür sie da ist |
|---|---|
| Aufgabe | Verhindert, dass der neue Chat mit einer Detailfrage beginnt, deren Zweck nicht erkennbar ist. |
| Stand | Ersetzt den Verlauf durch das, was geprüft ist. Ungeprüfte Zwischenergebnisse gehören nicht hierher. |
| Gültige Quelle | Macht die Kennungen wieder verwendbar, mit denen das Ergebnis später belegt wird. |
| Nicht gültig | Der wichtigste Eintrag. Er hält fest, was aus dem alten Verlauf gerade nicht mitkommen soll, und nennt den Grund. |
| Regeln | Vorgaben, die im alten Chat schon einmal gegeben wurden und sonst verlorengingen. |
| Offen | Trennt Ungeklärtes von Erledigtem, damit es nicht stillschweigend als geklärt behandelt wird. |
| Nächster Schritt | Der eigentliche Auftrag. Alles darüber ist Kontext. |

## Selbst prüfen

1. Steht in „Nicht gültig“ jede Fassung, jedes Dokument und jede Zahl, die im alten Chat aufgetaucht ist und nicht mehr gelten soll?
2. Ist der Stand tatsächlich geprüft, oder wurde ein ungeprüftes Zwischenergebnis übernommen?
3. Lässt sich der nächste Schritt allein mit dieser Notiz und den mitgegebenen Quellen bearbeiten, ohne den alten Chat zu kennen? Wenn nicht, fehlt in der Notiz etwas.
