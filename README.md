# Working with GenAI — Kurs-Repo

Repo für den HdM-Microcredential **„Generative KI in der Praxis: Produktivität steigern und Prozesse sicher optimieren"**. Der Kurs läuft vom 18.09.2026 (Kickoff) bis 08.10.2026 (Recap) und wird auf **kurse.kirenz.de** unter dem Slug `working-with-genai` ausgespielt.

Inhaltlicher Kern: der Unterschied zwischen einem Text, der gut klingt, und einem Ergebnis, das man vertreten kann. Sechs Module zu je drei Lektionen, ein durchgehender synthetischer Lehrfall (Nordwerk Elektrowerkzeuge), ein Praxisportfolio als Prüfungsleistung.

## Struktur

```
.
├── _quarto.yml              # Buch-Build-Konfiguration
├── AGENTS.md                # Schreibregeln für das Buch (kanonisch)
├── README.md                # diese Datei
├── book-theme.scss          # Buch-Theme, aus kurse/n8n-grundlagen übernommen
│
│  # — Buch (kanonische Quelle) —
├── index.qmd                # Willkommen
├── prompting/
│   └── arbeitsauftrag.qmd   # Modul 2.1 — Vom Zuruf zum Arbeitsauftrag
│
│  # — Downloads für Teilnehmende —
├── material/
│   ├── lehrfall-fachinformationen.txt
│   ├── kundenanfrage.txt
│   ├── prompt-vorlage.txt
│   └── portfolio-vorlage.md
│
│  # — Planung, nicht Teil des Buchs —
└── docs/
    ├── kurskonzept-v2.md    # abgestimmtes Kurskonzept
    └── umsetzung.md         # Stand, Prüfungen, offene Punkte
```

## Bauen

```bash
quarto render
open _book/index.html
```

Das Build erfasst nur die in `_quarto.yml` unter `project.render` gelisteten Pfade. `material/` und das Kurskonzept werden als verlinkte Ressourcen in den Buch-Build kopiert.

## Arbeitsweise

**Buch zuerst.** Pro Lektion entsteht erst das Quarto-Kapitel, danach die Unit für die Lernplattform. Buchtext steht in der **Wir-Form**, Unit-Text in **indirekter Ansprache oder Sie-Form**. Details in `AGENTS.md`.

**Nichts nur in der Unit.** Lehrfalldaten, Prompts und Vorlagen stehen vollständig im Buch und zusätzlich unter `material/`. Eine Unit darf verdichten und eigene diagnostische Aufgaben ergänzen.

**Belegdisziplin.** Keine Häufigkeitsbehauptungen ohne Quelle, keine Vorhersage von Modellverhalten als Gewissheit, keine erfundene Forschung, keine ungeprüften Preise. Siehe `AGENTS.md`, Abschnitt 7.

## Arbeitsstand

| Modul | Buch | Plattform-Unit |
|---|---|---|
| 1 — Ankommen: erster Erfolg und erste Grenzen | ⬜ konzipiert | ⬜ |
| 2 — Strukturierte Arbeitsaufträge | 🟡 1 von 3 Lektionen im Vollausbau | 🟡 1 von 3 |
| 3 — Kontext bereitstellen | ⬜ konzipiert | ⬜ |
| 4 — Qualität prüfen | ⬜ konzipiert | ⬜ |
| 5 — Verantwortung und Risiko-Orientierung | ⬜ konzipiert | ⬜ |
| 6 — In den Alltag bringen | ⬜ konzipiert | ⬜ |

Ausgearbeitet ist das Musterkapitel **2.1 Vom Zuruf zum Arbeitsauftrag** mit der zugehörigen Unit `02-01-arbeitsauftrag.unit.json` in der Lernplattform. Die übrigen 17 Lektionen sind in `docs/kurskonzept-v2.md` konzipiert und werden nach demselben Muster geschrieben. Leere Platzhalterkapitel werden bewusst nicht angelegt.

Keine Slide-Decks und keine Videos in diesem Repo. Der Textpfad ist selbsttragend; Screenshots und einige kurze Demos kommen später an den Oberflächen-Stellen dazu.

## Lizenz

Inhalt: © Jan Kirenz, 2026.

## Veröffentlichung

- [Online-Buch](https://kirenz.github.io/working-with-genai/)
- [Kurs mit Musterlektion](https://kurse.kirenz.de/courses/working-with-genai)

GitHub Actions baut das Buch mit Quarto 1.8.27 und veröffentlicht es auf GitHub Pages.
