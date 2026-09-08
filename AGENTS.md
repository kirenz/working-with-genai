# AGENTS.md — Kurs-Repo „Working with GenAI"

Lokale Schreibregeln für dieses Kursprojekt. Nutzerauftrag und übergeordnete Anweisungen haben Vorrang. Abgeleitet aus dem Vorbild-Repo `kurse/n8n-grundlagen`, gekürzt und auf diesen Kurs angepasst.

Der beschlossene neue Zuschnitt mit eigenen Grundlagen- und Use-Case-Lektionen steht in `docs/kurskonzept-v3.md`. Die konkrete Gliederung wird in der v3-Ausarbeitung umgesetzt; `docs/kursmanifest.json` ordnet die ausgearbeiteten Buchkapitel, Units und Folien einander zu. Der organisatorische Rahmen aus v2 bleibt bestehen. Diese Datei regelt, **wie** geschrieben wird.

---

## Repo-Struktur

```
.
├── _quarto.yml              # Buch-Build; nur eingehängt, was existiert
├── AGENTS.md                # diese Datei — Buch-Stil
├── README.md                # Repo-Beschreibung und Arbeitsstand
├── book-theme.scss          # Buch-Theme (aus n8n-grundlagen übernommen)
├── index.qmd                # Willkommen
├── start/, prompting/, kontext/       # Module 1–3
├── qualitaet/, verantwortung/, transfer/ # Module 4–6
├── praxis/                  # Freiwilliger Arbeitsagenten-Pfad
├── slides/                  # Reveal.js-Decks mit eigenen Schreibregeln
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

Analogien nur einsetzen, wenn sie beim Verständnis helfen. Höchstens eine pro Hauptbegriff, keine Pflichtanalogie.

### 4. Pro Lektion ein Kapitel

Eine Lektion = ein `.qmd` = eine Plattform-Unit, ergänzt um passende Folien. Grundlagen, Praxis und Orientierung dürfen unterschiedlich umfangreich sein. Grundlagen müssen keinen eigenen Durchlauf im Chatfenster enthalten. Genau ein H1, aussagekräftige H2, H3 nur sparsam. Themen, die eigenständig gelernt und später nachgeschlagen werden, bekommen einen eigenen verständlichen Titel in der Seitenleiste. Es gibt keine feste Zahl von Lektionen je Modul.

### 5. Struktur nach Lernziel

Grundlagen erhalten eigenständige, auffindbare Lektionen. Sie erklären den Zusammenhang in verständlichem Fließtext, nennen die gebräuchlichen Begriffe und erläutern sie an einem kurzen kommentierten Beispiel. Eine Beobachtung oder unbewertete Vermutung kann davorstehen. Notwendige Erklärungen stehen weder ausschließlich in Callouts noch in aufklappbaren Lösungen.

Praxislektionen führen über einen konkreten Anlass und geeignetes Material zu einem begrenzten Auftrag. Auf die eigene Durchführung folgen Prüfung und erklärendes Feedback. Schritte werden nur dort nummeriert, wo die Reihenfolge wichtig ist. Pro Modul wird ein zusammenhängender Beitrag zum eigenen Vorhaben bearbeitet; nicht jede Lektion braucht eine eigene Variante oder einen Portfolio-Eintrag.

Orientierungslektionen schaffen Überblick und benötigen kein Quiz. Bewertete Wissensfragen folgen erst auf die erforderlichen Erklärungen. Ein Quiz, eine Analogie oder ein Callout ist kein Pflichtbestandteil jeder Lektion. Kurze Hilfen zu einem einzelnen Schritt können direkt beim Schritt stehen.

Die Plattform-Unit muss die Kernerklärung selbst vermitteln. Der Buch-Tab bietet die vollständige Darstellung, ist aber keine Voraussetzung, um die Lernschritte zu verstehen. Die Erstellung erfolgt weiterhin zuerst im Buch.

### 6. Keine Verweise auf spätere Kapitel

Vorgriffe wie „in Modul 4 bauen wir…" veralten, sobald sich die Reihenfolge ändert. Bezug auf **frühere** Kapitel ist erlaubt und erwünscht („die Datenregeln aus Modul 1 gelten weiter").

### 7. Belegdisziplin — kursspezifisch

Dieser Kurs handelt vom Unterschied zwischen *plausibel* und *belegt*. Das Material darf diesen Unterschied nicht selbst verletzen.

- **Keine Häufigkeitsbehauptungen ohne Quelle.** Verboten sind Formulierungen wie „der häufigste Fehler", „meistens", „in der Regel", „das ist der Normalfall", wenn keine Quelle dahintersteht. Stattdessen den Mechanismus beschreiben: „Ein Chatmodell setzt Text fort, der zur Anfrage passt." Oder als Möglichkeit formulieren: „Damit besteht das Risiko, dass …".
- **Keine Vorhersage von Modellverhalten als Gewissheit.** Weder „das Modell wird die Garantiedauer erfinden" noch „das Modell fragt zurück". Was wir behaupten dürfen: dass ein Risiko besteht und vor der Verwendung geprüft werden muss.
- **Keine unbelegten Ursachenbehauptungen.** Konkrete Trainingsinhalte und der Grund für eine einzelne fehlerhafte Ausgabe werden nicht aus dem Ergebnis abgeleitet. Trainingswissen, mitgegebenen Kontext und Werkzeugabruf unterscheiden. Eine nicht durch das Material belegte Aussage ist nicht automatisch sachlich falsch; Halluzination und fehlende Quellenstütze nicht gleichsetzen.
- **Quellenrolle ausweisen.** Designentscheidungen dieses Kurses (etwa die Vierteilung Task/Context/Format/Check) werden als solche gekennzeichnet und nicht als belegter Standard verkauft. Belegte Aussagen bekommen die Primärquelle als Link. Übersicht: `docs/kurskonzept-v2.md`, Abschnitt 11.
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
- Lange Code- oder Prompt-Blöcke ohne verständliche Einordnung im umgebenden Text
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

Ziel ist **kurse.kirenz.de**, nicht eine HdM-Instanz. Slug: `working-with-genai`. Der vorhandene Flag `simulator_enabled` bleibt für diesen Kurs auf `false`.

Pro Lektion liefert das Repo `quarto_url` (Buch-Kapitel) und optional `slide_url` und `youtube_video_id`. Seeds, Import und Veröffentlichung sind **eigene, gesondert zu autorisierende Schritte** — sie gehören nicht zur Kapitelarbeit.

Für die vorhandenen Decks unter `slides/` gilt die dortige `AGENTS.md` mit indirekter Ansprache. Es gilt weiter: **keine Folie ohne Buch-Kapitel als Quelle.** Die Zuordnung von Buch, Folien und Units steht in `docs/kursmanifest.json`.
