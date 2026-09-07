# AGENTS.md — Kurs-Repo „Working with GenAI"

Lokale Schreibregeln für dieses Kursprojekt. Nutzerauftrag und übergeordnete Anweisungen haben Vorrang. Abgeleitet aus dem Vorbild-Repo `kurse/n8n-grundlagen`, gekürzt und auf diesen Kurs angepasst.

Kursaufbau, Zeitbudget und Modulzuschnitt stehen in `docs/kurskonzept-v2.md`. Diese Datei regelt nur, **wie** geschrieben wird.

---

## Repo-Struktur

```
.
├── _quarto.yml              # Buch-Build; nur eingehängt, was existiert
├── AGENTS.md                # diese Datei — Buch-Stil
├── README.md                # Repo-Beschreibung und Arbeitsstand
├── book-theme.scss          # Buch-Theme (aus n8n-grundlagen übernommen)
├── index.qmd                # Willkommen
├── prompting/               # Modul 2 — Strukturierte Arbeitsaufträge
│   └── arbeitsauftrag.qmd
├── material/                # Downloads für Teilnehmende (Lehrfall, Vorlagen)
└── docs/                    # Konzept und Umsetzungsstand (nicht Teil des Buchs)
```

Weitere Modul-Verzeichnisse entstehen erst, wenn Kapitel darin geschrieben werden. **Keine leeren Skelette in `_quarto.yml` eintragen** — ein Buch mit Platzhalterkapiteln ist schlechter als ein kurzes Buch.

Modul-Verzeichnis-Slug und Lesson-Datei-Slug: kebab-case, beschreibend, ohne `modul-XX`-Präfix. Die Reihenfolge steht in `_quarto.yml`.

---

## Die zwei Stilwelten dieses Kurses

| Welt | Wo | Ansprache |
|---|---|---|
| **Buch** | dieses Repo, alle `.qmd` | **Wir-Form** („Wir kopieren das Material…") |
| **Plattform-Unit** | `hdm/lernplattform/.../units/working-with-genai/*.json` | **Indirekt oder Sie** („Das Ergebnis gegen das Material lesen", „Ihre Angaben bleiben…") |

Wer Inhalte zwischen Buch und Unit überträgt, schaltet bewusst um. Das Buch ist die kanonische Quelle: **Erst das Kapitel, dann die Unit.**

**Die fachliche Grundlage darf nicht nur in einer Unit-JSON stehen.** Lehrfalldaten, Prompts, Vorlagen und Materialien gehören vollständig in den Buchtext **und** als Datei nach `material/`. Eine Unit darf verdichten und eigene diagnostische Aufgaben mit anderen Beispielen enthalten.

---

## Verbindliche Schreibregeln

### 1. Wir-Form

Durchgängig im sichtbaren Buchtext.

| Verwenden | Vermeiden |
|---|---|
| „Wir kopieren das Material in den Prompt." | „Sie kopieren…" / „Du kopierst…" |
| „Wir prüfen das Ergebnis gegen die Fachinformationen." | „Man prüft das Ergebnis…" |
| „Drei Fragen genügen." | (auch okay — beschreibend, ohne Anrede) |

Ausnahme: Text **innerhalb** eines Prompt-Codeblocks. Dort spricht der Auftrag das Modell direkt an („Entwirf eine Antwort-Mail…"), das ist der Gegenstand und keine Leseransprache.

### 2. Callout-Disziplin

- `::: {.callout-tip}` — Faustregeln, Analogien, Lesehinweise. Title Pflicht.
- `::: {.callout-note}` — Hintergrund, Quellenherkunft, Einordnung. Title empfohlen.
- `::: {.callout-important}` — Datenregeln, Fallstricke, Pflicht-Aufmerksamkeit. Title Pflicht.

**Maximal 4–5 Callouts pro Kapitel.** Wer mehr braucht, hat zwei Kapitel.

### 3. Analogien aus dem Berufsalltag

Geeignet: Büro und Assistenz, Urlaubsvertretung, Werkstatt, Bibliothek und Dossier, Küche und Rezept, Qualitätskontrolle, Cockpit.

Nicht geeignet: Märchen, Mythologie, Zauberei, Cartoon-Tiere, Superhelden, Videospiele, Kindergarten-Beispiele, „cute"-Stil.

Eine Analogie pro Hauptbegriff. Mehrere für denselben Begriff verwirren.

### 4. Pro Lektion ein Kapitel

Eine Lektion = ein `.qmd` = eine Plattform-Unit. Lernzeit 5–15 Minuten plus einen eigenen Durchlauf im Chatfenster. Genau ein H1, mehrere H2, H3 nur sparsam.

### 5. Kapitelstruktur bei Übungskapiteln

Kapitel, in denen etwas selbst gemacht wird, folgen dieser Reihenfolge:

1. Kurze Einleitung (1–2 Sätze)
2. `## <Der Lehrfall oder das Ausgangsmaterial>` — vollständig, nichts nachschlagen müssen
3. `## Zielbild` — was am Ende dasteht, plus die Bausteine als Tabelle oder Liste
4. `## Schritt für Schritt selbst bauen` — durchnummerierte `### Schritt 1`, `### Schritt 2`, …
5. Konstruiertes Beispiel und eigene Variante als Unterabschnitte des praktischen Teils
6. `## Fehler diagnostizieren` — Beobachtung und nächster Prüfschritt; Ursachen nur als Hypothesen benennen
7. `## Kontrollpunkt für Modul XX` — Lernziele in Verb-Infinitiv-Form

**Theorie steht in Callouts neben dem passenden Schritt**, nicht in Vorab-Sektionen. Wer ein Konzept in einem eigenen H2-Block vor dem ersten `### Schritt` erklären will, baut stattdessen einen Callout.

**Vorbild im Repo:** `prompting/arbeitsauftrag.qmd`.

### 6. Keine Verweise auf spätere Kapitel

Vorgriffe wie „in Modul 4 bauen wir…" veralten, sobald sich die Reihenfolge ändert. Bezug auf **frühere** Kapitel ist erlaubt und erwünscht („die Datenregeln aus Modul 1 gelten weiter").

### 7. Belegdisziplin — kursspezifisch

Dieser Kurs handelt vom Unterschied zwischen *plausibel* und *belegt*. Das Material darf diesen Unterschied nicht selbst verletzen.

- **Keine Häufigkeitsbehauptungen ohne Quelle.** Verboten sind Formulierungen wie „der häufigste Fehler", „meistens", „in der Regel", „das ist der Normalfall", wenn keine Quelle dahintersteht. Stattdessen den Mechanismus beschreiben: „Ein Chatmodell setzt Text fort, der zur Anfrage passt." Oder als Möglichkeit formulieren: „Damit besteht das Risiko, dass …".
- **Keine Vorhersage von Modellverhalten als Gewissheit.** Weder „das Modell wird die Garantiedauer erfinden" noch „das Modell fragt zurück". Was wir behaupten dürfen: dass ein Risiko besteht und vor der Verwendung geprüft werden muss.
- **Quellenrolle ausweisen.** Designentscheidungen dieses Kurses (etwa die Vierteilung Aufgabe/Material/Format/Grenzen) werden als solche gekennzeichnet und nicht als belegter Standard verkauft. Belegte Aussagen bekommen die Primärquelle als Link. Übersicht: `docs/kurskonzept-v2.md`, Abschnitt 11.
- **Keine erfundene Forschung.** Keine Studien, Prozentwerte oder Benchmark-Zahlen ohne nachprüfbare Quelle.
- **Beispielausgaben als konstruiert kennzeichnen.** Musterergebnisse im Buch sind konstruiert, keine aufgezeichneten Modelloutputs. Das steht dabei.

### 8. Werkzeug- und Datendisziplin

- Jede Pflichtübung läuft im **kostenlosen Chatkonto**. Keine Übung setzt ein Abonnement, eine API oder eine Installation voraus.
- **Kein Anbieter-Ranking.** Vergleiche beschreiben Unterschiede am eigenen Fall, sie küren keinen Sieger.
- **Keine erfundenen Preise oder Funktionsumfänge.** Wenn eine Angabe nicht geprüft wurde, steht sie nicht im Text.
- **Kein automatischer Versand.** Ergebnisse enden als Entwurf.
- Lehrfalldaten sind **synthetisch**. Für eigene Fälle gilt: Platzhalter statt echter Namen, Adressen, Kunden- und Vertragsnummern.

### 9. Disziplin-Verbote

- Direkt-Anrede (du, Sie) im Buchtext
- „man"-Konstruktionen
- Emojis im Fließtext (Ausnahme: Status-Marker in Tabellen ✅ 🟡)
- Lange Code- oder Prompt-Blöcke ohne erklärenden Folge-Callout
- Marketing-Sprache, Superlative, „revolutionär"
- Unnötige Anglizismen im sichtbaren Text; Fachbegriffe nur, wenn sie im selben Satz erklärt werden

---

## Erstentwurf-Workflow

Ein nicht voll ausgearbeitetes Kapitel wird markiert:

```
::: {.callout-note title="Status — Erstentwurf"}
Erstentwurf. Ausbau-Punkte am Ende des Kapitels.
:::
```

und schließt mit `## Was als Nächstes ausgebaut werden muss` plus konkreten TODO-Punkten.

**Ein Kapitel im Vollausbau trägt keinen dieser Marker.** Ein beauftragtes Musterkapitel gilt nicht als fertig, solange es nur Ausbau-TODOs enthält.

---

## Validierung

**Buch rendern** (Repo-Root):

```bash
quarto render
```

Errors müssen behoben sein, Warnings inhaltlich geprüft. Output unter `_book/`.

**Plattform-Unit prüfen** (DB-frei, ohne Import):

```bash
cd /Users/jankirenz/code/hdm/lernplattform/apps/api
uv run python scripts/validate_unit.py app/db/units/working-with-genai/<datei>.unit.json
```

Schlägt eine Datei hier fehl, würde auch der echte Import fehlschlagen.

---

## Anbindung an die Lernplattform

Ziel ist **kurse.kirenz.de**, nicht eine HdM-Instanz. Slug: `working-with-genai`. Der vorhandene Flag `simulator_enabled` wird für diesen Kurs später auf `false` gesetzt.

Pro Lektion liefert das Repo `quarto_url` (Buch-Kapitel) und optional `slide_url` und `youtube_video_id`. Seeds, Import und Veröffentlichung sind **eigene, gesondert zu autorisierende Schritte** — sie gehören nicht zur Kapitelarbeit.

Slide-Decks gibt es in diesem Repo noch nicht. Wenn sie hinzukommen, gilt für `slides/` eine eigene `slides/AGENTS.md` mit indirekter Ansprache, und es gilt weiter: **keine Folie ohne Buch-Kapitel als Quelle.**
