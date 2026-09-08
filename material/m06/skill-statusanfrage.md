---
name: statusanfrage-entwurf
description: Entwirft eine Antwort auf eine Kundenanfrage zum Sendungsstatus der Rösterei Morgenrot aus den Versandinformationen, ohne Ankunftstag oder Status zu behaupten. Verwenden, wenn eine Anfrage nach Lieferung, Paket oder Sendung eingeht.
---

# Statusanfrage beantworten (Entwurf)

Kursmaterial „Working with GenAI", Modul 6, Lektion 6.2. Beispiel für eine wiederverwendbare Arbeitsanleitung im Format einer Skill-Datei. Der Kopf mit `name` und `description` folgt dem Aufbau, den Claude Code für Skills beschreibt (<https://code.claude.com/docs/en/skills>, Abruf 08.09.2026). Der Text darunter ist eine normale Arbeitsanleitung und funktioniert unverändert auch als Projekt-Anweisung oder als erste Chatnachricht. Für den Kurs ist keine Installation nötig.

## Wann diese Anleitung gilt

Eine Kundenanfrage fragt nach dem Verbleib, dem Status oder dem Ankunftstag einer Sendung.

## Schritte

1. Aus der Anfrage nur übernehmen: die Frage, den genannten Wochentag der Versandbestätigung, ob eine Sendungsnummer vorliegt (ja oder nein, nicht die Nummer selbst).
2. Aus den Versandinformationen erklären: Versandtage, Versandbestätigung mit Sendungsnummer, Laufzeit laut Paketdienst, keine Ankunftsgarantie.
3. Ankündigen, dass Lager und Versand den Status mit der Sendungsnummer prüft und sich meldet.
4. Die Frage nach dem Ankunftstag unter „Offen" führen.
5. Absenderzeile „Ellen Ruppert, Lager und Versand, Rösterei Morgenrot".

## Kontrollpunkt vor der Weitergabe

Dieser Abschnitt leistet für die Anleitung dasselbe wie der Block CHECK in einem einzelnen Prompt. Der Entwurf ist nur dann fertig, wenn alle vier Punkte zutreffen:

- Kein konkreter Ankunftstag im Text, auch nicht „voraussichtlich Freitag".
- Kein behaupteter Status („ist unterwegs", „wurde zugestellt").
- Die Laufzeit steht als Angabe des Paketdienstes, nicht als Zusage der Rösterei.
- Unter „Offen" steht mindestens: Ankunft bis zum genannten Tag; aktueller Sendungsstatus.

## Testfall

Anfrage: „Versandbestätigung kam Dienstag, kommt das Paket bis Freitag?"
Erwartung: Entwurf erklärt Laufzeit ein bis drei Werktage laut Paketdienst, sagt keinen Tag zu, kündigt Prüfung an, führt „Ankunft bis Freitag" unter „Offen".

## Was diese Anleitung nicht ist

Sie ist kein Agent und kein Zugriffsrecht. Sie prüft keinen Status, sie öffnet kein System und sie versendet nichts. Sie beschreibt, wie ein Entwurf gebaut und geprüft wird.
