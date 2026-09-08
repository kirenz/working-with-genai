# Begründete Entscheidung: automatisieren, teilautomatisieren oder im Chat lassen?

Kursmaterial „Working with GenAI", Modul 6, Lektion 6.3. Vorlage für Portfolio-Teil 4. n8n ist keine Prüfungspflicht; die Entscheidung ist es.

## Ausgefülltes Beispiel: Statusanfragen bei Lager und Versand

| Kriterium | Befund für die Rösterei Morgenrot |
|---|---|
| **Häufigkeit** | Mehrere Statusanfragen pro Woche, gleichartig aufgebaut |
| **Prüfbarkeit des Entwurfs** | Hoch: Der Entwurf darf nur erklären und ankündigen; jede darüber hinausgehende Aussage fällt beim Lesen auf |
| **Datenlage** | Die Antwort braucht keine personenbezogenen Angaben; die Sendungsnummer bleibt außerhalb des Modells |
| **Was der Mensch tun muss** | Status im System des Paketdienstes prüfen, Entwurf ergänzen, versenden. Das ist der Kern der Arbeit und bleibt |
| **Modellzugang im Betrieb** | Nicht vorhanden. Ein Workflow mit Modellschritt bräuchte einen bezahlten Zugang mit passender Vereinbarung |
| **Was schiefgehen kann** | Ein Entwurf mit zugesagtem Ankunftstag geht ungeprüft hinaus; das Material veraltet |

**Entscheidung.** Vorerst kein eigener Workflow. Die Statusanfragen laufen über das Projekt mit Startpaket im Chatkonto (Lektion 6.2), weil das ohne zusätzlichen Zugang funktioniert und die Prüfung ohnehin von Hand geschieht. Ein Workflow wird erneut geprüft, wenn (a) ein geschäftlicher Modellzugang mit Vereinbarung besteht und (b) der Rückblick nach 30 Tagen zeigt, dass Entwürfe im Regelfall ohne inhaltliche Korrektur bleiben. Auch dann endet der Workflow beim Entwurf; die Prüfung und der Versand bleiben bei Ellen Ruppert.

**Begründung in einem Satz.** Der Nutzen liegt in der gleichbleibenden Qualität des Entwurfs und im Wegfall des Wiederholens der Anweisungen, nicht im Wegfall der Prüfung; dafür reicht das Projekt.

## Leere Vorlage für den eigenen Fall

| Kriterium | Befund |
|---|---|
| **Häufigkeit** | <wie oft, wie gleichartig?> |
| **Prüfbarkeit des Entwurfs** | <woran fällt ein Fehler beim Lesen auf?> |
| **Datenlage** | <welche Angaben braucht der Entwurf, welche bleiben außerhalb?> |
| **Was der Mensch tun muss** | <welcher Schritt bleibt in jedem Fall bei einer Person?> |
| **Modellzugang im Betrieb** | <vorhanden, mit welcher Vereinbarung? nicht vorhanden?> |
| **Was schiefgehen kann** | <konkret, nicht „Fehler">

**Entscheidung.** <Chat mit Startpaket / Workflow bis zum Entwurf / später erneut prüfen, unter welcher Bedingung?>

**Begründung in einem Satz.** <…>
