# Aktennotiz: Datenregel für KI-gestützte Entwürfe

Kursmaterial „Working with GenAI", Modul 5, Lektion 5.2. Synthetische GenAI-Erweiterung des Lehrfalls Rösterei Morgenrot. Die Notiz ist ein Übungsmuster und keine Rechtsberatung. Was im eigenen Betrieb gilt, entscheidet die Regelung der eigenen Organisation.

---

## Ausgefülltes Beispiel: Rösterei Morgenrot, Kundenservice-Entwürfe

**Anlass.** Kundenanfragen zu Abo, Sortiment und Lieferung sollen mit einem Chatmodell als Entwurf vorbereitet werden. Sina Bergmann (Vertrieb und Kundenservice) hat gefragt, ob eingehende Mails dafür in das Chatkonto kopiert werden dürfen.

**Genutztes Konto.** Bis auf Weiteres ein kostenloses Einzelkonto. Zu diesem Konto liegt keine Vereinbarung vor, die eine Verarbeitung von Kundendaten im Auftrag der Rösterei regelt. Ob und wie Eingaben beim Anbieter gespeichert oder zum Training verwendet werden, ergibt sich aus dessen Bedingungen und Einstellungen. Diese sind vor einer Nutzung mit echten Daten zu prüfen.

**Regel.** In das Konto gehen nur Angaben, die eine Antwort tatsächlich braucht, und nur in dieser Form:

| Angabe in der Anfrage | Nötig für den Entwurf? | Umgang |
|---|---|---|
| Kundenfrage im Wortlaut (Sorte, Abo, Preis) | ja | mitgeben |
| Name, Anrede | nein | weglassen oder [Name] |
| Kunden-, Abo-, Rechnungsnummer | nein | weglassen oder [Kundennummer] |
| Liefer- oder Rechnungsadresse | nein, eigener Vorgang im Kundenkonto | weglassen |
| Telefonnummer, private Mailadresse | nein | weglassen |
| Angaben zu Dritten (Nachbar, Familie) | nein | weglassen |
| Angaben zu Gesundheit, Religion, Herkunft und ähnliche | nein, nie | vollständig entfernen, nicht ersetzen |
| Interne Vorgangsnotizen (Zahlungsverzug, Beschwerdeverlauf) | nur in Ausnahmefällen | nicht in dieses Konto; bei Bedarf gesondert klären |

**Wo die Platzhalter gesetzt werden.** Vor dem Chatfenster, nicht darin. Wer eine Mail zum Anonymisieren in das Chatkonto kopiert, hat die personenbezogenen Angaben bereits übermittelt. Für Kundenmails gilt: Fragen abschreiben oder herauskopieren, Rest bleibt im Postfach.

**Was das Modell nicht bekommt.** Zugriff auf das Kundenkonto, den Sendungsstatus oder das Rechnungssystem. Antworten mit solchen Angaben ergänzt die zuständige Person nach der Prüfung selbst.

**Was diese Regel nicht leistet.** Sie ersetzt keine datenschutzrechtliche Prüfung und keine Vereinbarung mit dem Anbieter. Sie regelt nur, wie das Team bis zu dieser Klärung arbeitet.

**Zuständigkeiten.**

| Frage | Wer klärt das verbindlich? | Stand |
|---|---|---|
| Welches Konto darf mit welchen Daten genutzt werden? | Aylin Yılmaz, Geschäftsführung | Regel oben gilt vorläufig |
| Welche Vertragslage besteht zum Anbieter? Wird eine geschäftliche Lizenz nötig? | Petra Lindqvist, Verwaltung und Controlling | offen |
| Datenschutzrechtliche Einordnung (Rechtsgrundlage, Auftragsverarbeitung, Betroffeneninformation) | Im Fall ist keine datenschutzbeauftragte Person benannt. Externe Beratung durch Aylin Yılmaz zu beauftragen | offen |
| Einhaltung im Alltag | Sina Bergmann für den Kundenservice | läuft |

Datum: 2026-09-07. Nächste Prüfung: beim Rückblick nach 30 Tagen (siehe Transferplan).

---

## Leere Vorlage für den eigenen Fall

**Anlass.** <Welche Aufgabe soll mit einem Chatmodell vorbereitet werden, und wer hat gefragt?>

**Genutztes Konto.** <Privat oder geschäftlich? Welche Vereinbarung besteht? Was ist zu Speicherung und Training bekannt, was noch nicht?>

**Regel.**

| Angabe im Ausgangsmaterial | Nötig für das Ergebnis? | Umgang |
|---|---|---|
| <…> | <ja / nein> | <mitgeben / Platzhalter / weglassen / nicht in dieses Konto> |

**Wo die Platzhalter gesetzt werden.** <Vor dem Chatfenster; wie konkret?>

**Was das Modell nicht bekommt.** <Systeme, Listen, Verläufe>

**Was diese Regel nicht leistet.** <Keine Rechtsprüfung, keine Vereinbarung mit dem Anbieter, keine Freigabe durch …>

**Zuständigkeiten.**

| Frage | Wer klärt das verbindlich? | Stand |
|---|---|---|
| Konto und Freigabe | <Rolle> | <offen / geklärt> |
| Vertragslage | <Rolle> | <…> |
| Datenschutzrechtliche Einordnung | <Rolle oder „nicht benannt, zu beauftragen"> | <…> |
| Einhaltung im Alltag | <Rolle> | <…> |
