# n8n-Miniworkflow: alle Feldwerte zum Kopieren

Kursmaterial „Working with GenAI", Modul 6, Lektion 6.2. Drei Knoten auf der bereitgestellten Kursinstanz: Auslöser, Felder, Sprachmodell. Der Workflow endet beim sichtbaren Entwurf. Kein Versandknoten, keine Aktivierung.

Knotennamen und Feldbezeichnungen entsprechen der n8n-Dokumentation zu **Edit Fields (Set)** und **Basic LLM Chain** (Abruf 07.09.2026). Einzelne Bezeichnungen können sich mit der Version der Kursinstanz unterscheiden; die Lehrenden-Einrichtungsanleitung sieht einen Abgleich vor dem Kurs vor.

## Knoten 1: Auslöser

| Einstellung | Wert |
|---|---|
| Knoten | **Trigger manually** (Manual Trigger) |
| Name | `Start` |

## Knoten 2: Edit Fields (Set)

| Einstellung | Wert |
|---|---|
| Knoten | **Edit Fields (Set)** |
| Name | `Anfrage und Material` |
| Mode | **Manual Mapping** |
| Include Other Input Fields | aus |

Unter **Fields to Set** zwei Felder anlegen (Schaltfläche zum Hinzufügen eines Feldes, in der Kursinstanz voraussichtlich *Add Field*):

**Feld 1**

| | |
|---|---|
| Name | `anfrage` |
| Type | String |
| Value (Fixed) | siehe unten |

```text
Betreff: Wo bleibt meine Lieferung?
Guten Tag, meine Abo-Lieferung mit der Sendungsnummer [SENDUNGSNUMMER] ist noch nicht da. Die Versandbestätigung kam am Dienstag. Kommt das Paket bis Freitag? Ich bin dann verreist.
Viele Grüße
K. Weber
```

**Feld 2**

| | |
|---|---|
| Name | `material` |
| Type | String |
| Value (Fixed) | siehe unten |

```text
Versandinformationen Lager und Versand (nur diese Angaben sind gültig):
- Abo-Lieferungen werden dienstags und donnerstags versendet.
- Mit dem Versand erhält die Kundin oder der Kunde eine Versandbestätigung per Mail mit einer Sendungsnummer.
- Der Paketdienst nennt als Laufzeit ein bis drei Werktage nach dem Versand. Die Rösterei gibt keine Ankunftsgarantie für einen bestimmten Tag.
- Der Sendungsstatus kann nur mit der Sendungsnummer geprüft werden. Die Prüfung erfolgt durch Lager und Versand, nicht durch das Chatmodell.
- Gilt eine Sendung nach fünf Werktagen ab Versand als nicht zugestellt, löst Lager und Versand eine Nachforschung beim Paketdienst aus und informiert die Kundin oder den Kunden.
```

Nach **Execute step** zeigt das Output-Panel ein Element mit den beiden Feldern `anfrage` und `material`.

## Knoten 3: Basic LLM Chain

| Einstellung | Wert |
|---|---|
| Knoten | **Basic LLM Chain** |
| Name | `Entwurf` |
| Prompt | **Define below** |
| Prompt-Feld | Modus **Expression**, Inhalt siehe unten |
| Require Specific Output Format | aus |
| Chat Model (Anschluss unten am Knoten) | das von den Lehrenden bereitgestellte Chat-Model mit der Credential laut Kursinfo |

Inhalt des Prompt-Felds (im Expression-Modus, vollständig einfügen):

```text
Du unterstützt den Bereich Lager und Versand der Rösterei Morgenrot.

AUFGABE
Entwirf eine Antwort-Mail auf die Kundenanfrage unten.

MATERIAL (nur diese Angaben sind gültig)
{{ $json.material }}

KUNDENANFRAGE
{{ $json.anfrage }}

FORMAT
Antwort-Mail, höchstens 120 Wörter, Anrede "Guten Tag", sachlicher Ton.
Absenderzeile "Ellen Ruppert, Lager und Versand, Rösterei Morgenrot".
Am Ende eine Liste mit der Überschrift "Offen".

GRENZEN
- Verwende ausschließlich Angaben aus dem Material. Ergänze nichts.
- Nenne keinen Ankunftstag und keinen Sendungsstatus. Trage beides unter "Offen" ein.
- Behaupte nicht, dass etwas veranlasst wurde. Kündige an, dass Lager und Versand den Status mit der Sendungsnummer prüft.
- Verwende die Sendungsnummer nicht im Text.
```

Die beiden Ausdrücke `{{ $json.material }}` und `{{ $json.anfrage }}` holen die Werte aus dem vorherigen Knoten. Im Expression-Modus werden sie beim Ausführen ersetzt; im Modus Fixed blieben sie als Text stehen.

Nach **Execute step** zeigt das Output-Panel ein Element mit einem Feld `text`, das den Entwurf enthält.

## Ersatzweg ohne Modellzugang

Statt Knoten 3 einen zweiten **Edit Fields (Set)** anhängen, Name `Entwurf (manuell)`, ein Feld `text` vom Typ String, Wert Fixed: der Inhalt aus `entwurf-konstruiert.txt` oder ein selbst im Chatkonto erzeugter und geprüfter Entwurf. Der Workflow zeigt dann dieselbe Struktur und dasselbe Ausgabefeld; nur der Modellschritt ist von Hand gefüllt.

## Was nicht dazugehört

Kein Knoten **Send Email**, kein Gmail- oder Outlook-Knoten, kein Trigger auf ein echtes Postfach, kein Klick auf *Activate*. Der Workflow wird gespeichert und bleibt inaktiv. Getestet wird mit **Execute step** am Knoten oder **Execute workflow** in der Übersicht.
