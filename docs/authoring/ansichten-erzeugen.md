# Ansichtsdateien erzeugen

Ein Erzeugungslauf für die lokale gemeinsame Durchsicht, keine Test- oder Review-Schleife. Zuerst `quarto render` für das Buch. Danach das eigenständige Folienprojekt als Reveal.js rendern. Dessen Konfiguration liegt in `slides/_quarto.yml`; die Ausgabe geht nach `_book/slides/`:

```sh
quarto render
quarto render slides
```

Ergebnisse im Quarto-Ausgabeverzeichnis `_book/`, Navigation über `kursuebersicht.html`. Die GitHub-Workflow-Datei bildet diese Erzeugung für einen später ausdrücklich beauftragten Release ab; sie wurde in diesem Auftrag weder gepusht noch ausgelöst.
