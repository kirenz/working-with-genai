# Quellen und Wiederverwendung im Vollausbau

Recherche für die Ausarbeitung, Stand 07.09.2026. Kein Bericht über Tests, Produktzugänge oder eine Generalprobe. Die ausführlichen Kapitelzuordnungen stehen in den drei Autorennotizen unter `docs/authoring/`.

## Eigene Trainings als Ausgangspunkt

| Bestand | Übertragener didaktischer Baustein | Anpassung an diesen Kurs |
|---|---|---|
| `presentation/training-frech/uebungen.qmd`, `handout/_uebungen/` | Ein geführter Pfad, kontrollierte Unterlage, kopierbarer Auftrag und nachvollziehbares Ergebnis; Copy/Paste-Fallback beim Dokument | CompanyGPT-spezifische Links und betriebliche Inhalte entfallen; Morgenrot-Fall im gewöhnlichen Chat |
| `consulting/vwa-ki-strategie/buch/` | Aufgabenorientierte Erklärung, Kontext, Recherche, wiederverwendbare Anweisungen und Arbeitshilfen | Einsteigerumfang und sechsmoduliger Rahmen, keine VWA-Verfahrensannahmen |
| `consulting/vwa-ki-strategie/IT/` | Datenbedarf, Zuständigkeiten, enge Aktionsrechte und begrenzte Pilotvorhaben | Konkrete Entscheidungsfälle statt IT-Architektur, Einkaufsvergleich oder eigener API-Integration |
| Plattformunits `claude-sima` und `ai-sima`; `consulting/sima-ai/reference/` | Quellenbasierte Arbeitsabläufe, Projektmaterial, Dateiarbeit, Regeln und Skills | Kurze deutsche Aufgaben mit synthetischen Röstereidaten; Enterprise-Integrationen nicht vorausgesetzt |
| `kurse/n8n-grundlagen` und Units `n8n-grundlagen-uc` | Geführter Eigenbau, sichtbare Eingabe und Ausgabe, Handlungs- und Kontrollschritte | Ein kleiner Entwurfsablauf auf Kursinstanz, kein eigener kostenpflichtiger Modellzugang |
| `kurse/business-analytics` | Rösterei, Sortiment, Ausgangslage, Personen und Bilder | GenAI-Arbeitsaufträge eigens ergänzt; Rollen und vorhandene Fakten erhalten |

Es werden keine privaten Firmendaten, internen Links, Kundenlisten oder Firmenzugänge in das veröffentlichbare GenAI-Material übernommen. Herkunft und neue didaktische Ausgestaltung sind getrennt dokumentiert.

## Aktuelle Primärquellen

- OpenAI, [Projects in ChatGPT](https://help.openai.com/en/articles/10169521): Arbeitszusammenhang mit Anweisungen und Material. Einzelne Funktionen und Grenzen folgen dem Konto. Die Seite enthält unterschiedlich alte Angaben zu Teilen der Freigabe-Funktion; der Kurs setzt kein Teilen voraus.
- OpenAI, [Deep research](https://help.openai.com/en/articles/10500283): mehrstufiger Recherchemodus. Für einzelne aktuelle Angaben reicht oft ein enger Suchauftrag; überprüfte Originalquellen bleiben erforderlich.
- OpenAI, [App-Dokumentation](https://developers.openai.com/codex/app/): beim Abruf Weiterleitung zu `learn.chatgpt.com/docs/app`. Die Bezeichnung Codex aus dem Nutzerauftrag wird als gewünschter Arbeitsagenten-Zugang erhalten; keine automatische Gleichsetzung aller aktuellen Produktoberflächen.
- Anthropic, [Projects erstellen und verwalten](https://support.claude.com/en/articles/9519177-how-can-i-create-and-manage-projects): Projektmaterial und Anweisungen. **Quellenkonflikt:** Help Center nennt Zugang auch für Free, während die am selben Tag abgerufene [Preistabelle](https://claude.com/pricing) für Projects bei Free „No“ ausweist. Daher keine uneingeschränkte Gratis-Projektzusage; maßgeblich verfügbarer Zugang mit vollständigem Chat-Fallback.
- Anthropic, [Claude Code](https://code.claude.com/docs/en/overview): Dateien und Werkzeuge im Arbeitskontext. Passende Rechte und ein abgegrenzter Übungsordner sind Bestandteil des Arbeitsauftrags.
- Google, [Gems erstellen](https://support.google.com/gemini/answer/15235603): Anweisungen und Material für wiederkehrende Aufgaben. Ein sichtbarer Vorschauzustand ist noch kein gespeicherter Gem.
- n8n, [Basic LLM Chain](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.chainllm/) und [Edit Fields](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.set/): Grundlage für den geführten Miniworkflow. Die Kursinstanz und zentrale Modellanbindung müssen noch organisatorisch vorbereitet werden.
- Europäische Kommission, [AI Literacy FAQ](https://digital-strategy.ec.europa.eu/en/faqs/ai-literacy-questions-answers): kontextbezogene Förderung von KI-Kompetenz. Aktualisierte Detailantworten zu Artikel 4 stehen neben einem älteren Seitenkopf. Der Kurs behauptet kein vorgeschriebenes Zertifikat oder garantiertes individuelles Kompetenzniveau. Einzelne Rechtsfragen werden mit Quellenstand und Zuständigkeit eingeordnet.
- Datenschutzkonferenz, [Orientierungshilfe KI und Datenschutz](https://www.datenschutzkonferenz-online.de/media/oh/20240506_DSK_Orientierungshilfe_KI_und_Datenschutz.pdf): organisatorische Voraussetzungen und datenschutzbezogene Auswahlkriterien. Kein abschließender Freigabekatalog.
- [§ 2 UrhG](https://www.gesetze-im-internet.de/urhg/__2.html) und [§ 51 UrhG](https://www.gesetze-im-internet.de/urhg/__51.html): persönliche geistige Schöpfung und zweckgebundenes Zitatrecht. Eine Quellenangabe ersetzt keine Nutzungsbefugnis.

Weitere Quellen werden von den Autorinnen und Autoren der Modulgruppen in ihren Notizen konkret zugeordnet. Lange Dokumentationstexte werden nicht übernommen. Anbieterinformationen belegen Produktbeschreibungen, keine allgemeine Überlegenheit oder Produktivitätswirkung.

## Aktualität im Kurs

„Aktuell arbeiten“ bedeutet hier: einen Auftrag aus Material und Erfolgskriterien bilden, Kontext bewusst auswählen, Quellen und Versionen nachvollziehen, Werkzeuge gezielt einsetzen und wiederholbare Arbeitsschritte mit menschlichen Entscheidungen verbinden. Eine Liste angeblich bester Modelle wäre schnell veraltet und ist kein Lernziel.

Preise und Modellnamen werden nicht als dauerhafte Pflichtwerte in die Übungen eingebaut. Die Zugangsseiten dienen der eigenen konkreten Entscheidung vor einer optionalen Nutzung. Grundlegende Funktionen bleiben über Texteingabe bearbeitbar; konstruiertes Vergleichsmaterial wird von tatsächlichen Modellläufen unterschieden.
