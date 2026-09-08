# Demo-Ordner: Ein Arbeitsagent prüft Produkttexte

Kursmaterial „Working with GenAI", freiwilliger Praxispfad (Kapitel „Codex und Claude Code: Wenn das Werkzeug Dateien anfasst"). Synthetische GenAI-Erweiterung des Lehrfalls Rösterei Morgenrot. Alle Dateien sind erfunden und dürfen ohne Bedenken einem Werkzeug übergeben werden.

## Was in diesem Ordner liegt

| Datei | Rolle | Wird vom Agenten … |
|---|---|---|
| `auftrag.md` | Die Anweisung an den Agenten (Aufgabe, Material, Format, Grenzen) | gelesen |
| `briefing.txt` | Das freigegebene Briefing: die einzige gültige Faktenquelle | gelesen |
| `produkttexte-entwurf.md` | Drei Produkttexte mit gedeckten und ungedeckten Aussagen | gelesen, nicht verändert |
| `ergebnis-soll.md` | Beschreibung des gewünschten Ergebnisses, zum Vergleich nach dem Lauf | nicht benötigt |
| `pruefbericht-beispiel.md` | Fertiges, konstruiertes Beispiel eines Prüfberichts (Fallback, falls kein Agent verfügbar ist) | nicht benötigt |

Erwartetes Artefakt nach dem Lauf: eine **neue Datei `pruefbericht.md`** in diesem Ordner. Sonst darf sich nichts ändern.

## Ablauf in Kurzform

1. Ordner lokal ablegen (alle Dateien in ein gemeinsames Verzeichnis).
2. Arbeitsagent in genau diesem Ordner starten (Claude Code oder Codex, je nach Zugang).
3. Als erste Nachricht: `Lies auftrag.md und führe den Auftrag aus.`
4. Freigabefragen des Werkzeugs lesen, bevor sie bestätigt werden: Welche Datei will es schreiben?
5. Nach dem Lauf: `pruefbericht.md` öffnen und gegen `ergebnis-soll.md` vergleichen. Prüfen, ob `produkttexte-entwurf.md` unverändert ist.

Wer keinen Agenten nutzen kann oder will, nimmt den Kopierweg aus dem Buchkapitel: Briefing und Entwürfe in ein Chatfenster einfügen, den Prüfbericht als Text erzeugen lassen und ihn selbst als Datei speichern. Das Ergebnis ist vergleichbar, der Weg dahin ist der Unterschied, um den es im Kapitel geht.
