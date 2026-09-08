# Vier Arbeitsweisen nebeneinander

Kursmaterial „Working with GenAI", Modul 6, Lektion 6.1. Orientierungskarte, keine Rangfolge. Die Reihenfolge in der Tabelle ist keine Reihenfolge des Könnens.

Die Spalten beschreiben vier Nutzungsweisen, wie dieser Kurs sie verwendet, nicht den Funktionsumfang der Produkte. Ein Chatfenster kann Dateien, Werkzeuge und Verbindungen zu anderen Systemen nutzen; ein Projekt ist ein Chat mit hinterlegten Anweisungen. Die Grenzen verschwimmen, die Fragen bleiben dieselben.

## Übersicht

| | Chat | Projekt (Projects bei ChatGPT und Claude, Gems bei Gemini; eigenständige Umsetzungen, keine identischen Funktionen) | Arbeitsagent (Codex, Claude Code) | Workflow (z. B. n8n) |
|---|---|---|---|---|
| **Wo stehen die Anweisungen?** | in der Nachricht | einmal hinterlegt, im Anweisungsfeld nachlesbar | in einer Datei im Arbeitsbereich | in einem Knoten des Ablaufs |
| **Wechselt die Aufgabe?** | ja, ständig | nein, gleiche Art | wechselt im selben Arbeitsbereich | nein, die möglichen Pfade liegen fest |
| **Wer steuert die Schritte?** | die Person, Nachricht für Nachricht | die Person, mit hinterlegten Regeln | das Werkzeug, innerhalb der Freigaben | der vorher gebaute Ablauf |
| **Wer sieht das Ergebnis, wann?** | sofort, weil angefordert | sofort, weil angefordert | nach dem Lauf, als Datei | nur, wenn jemand hinsieht |
| **Was greift das Werkzeug?** | was in der Nachricht steht | was hinterlegt ist | Dateien im Arbeitsbereich | was der Ablauf ihm reicht |
| **Zusätzliche Sicherung nötig?** | sobald Dateien oder Verbindungen im Spiel sind: ja | wie Chat | ja: Freigabeeinstellung des Werkzeugs | ja: kein Versandknoten, keine Aktivierung ohne Regelung |
| **Voraussetzung im Kurs** | kostenloses Chatkonto | kostenloses Chatkonto, Funktion kontoabhängig | freiwillig, Kopierweg als Ersatz | Kursinstanz, sonst Ersatzweg |

## Die fünfte Möglichkeit: kein Sprachmodell

Eine exakt regelgebundene Aufgabe ist mit einer Textvorlage, einer Tabellenformel oder einer gewöhnlichen Automatisierung oft besser bedient: Dieselbe Eingabe liefert dasselbe Ergebnis, und die Prüfung richtet sich auf die Regel und die Eingabedaten statt auf jede einzelne Ausgabe. Ganz ohne Prüfung geht es nicht, denn eine falsche Formel rechnet zuverlässig falsch. Ein Sprachmodell lohnt sich, wo Sprache, Vielfalt oder Einordnung gefragt sind.

## Drei Fragen für die eigene Aufgabe

1. **Wiederholt sich die Aufgabe, und stehen die Regeln fest?** Wenn nein: Chat. Wenn ja: Projekt.
2. **Liegen Material und Ergebnis als Dateien nebeneinander, und sollen sie dort bleiben?** Wenn ja: Arbeitsagent ist passend; der Kopierweg im Chat liefert dasselbe Ergebnis mit zwei Handgriffen mehr.
3. **Soll etwas entstehen, ohne dass in diesem Moment jemand hinsieht?** Dann ist es ein Workflow, und vor dem Bauen ist zu klären, wer prüft, woran und wann.

## Was unabhängig von der Wahl gleich bleibt

- Der Auftrag behält seine vier Teile: Task, Context, Format, Check.
- Die Datenregel gilt weiter. Ein Projekt ist kein Freigabenachweis, ein Ordner auch nicht.
- Die Verantwortung bleibt bei einem Menschen. Automatische Prüfschritte sind möglich und verschieben nur, wo eine Person hinsehen muss; es ändert sich vor allem, wie leicht die Prüfung ausgelassen werden kann.
