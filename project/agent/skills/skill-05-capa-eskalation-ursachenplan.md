---
name: capa-eskalation-ursachenplan
description: Prüft die CAPA-Eskalation einer NC (NC-SOP Schritt 9) und erstellt Problemstellung, messbares CAPA-Ziel und einen Untersuchungsplan mit 5-Why und Ishikawa für Auftretens-, Entdeckungs- und systemische Ursache (CAPA-SOP Schritt 2–3). Verwenden bei „Brauchen wir eine CAPA?", „5-Why", „Ishikawa", „Ursachenanalyse planen".
version: 1.0
---

# Skill 05 – CAPA-Eskalation und Ursachenanalyse strukturieren

## Wann verwenden

- „Ist für diese NC eine CAPA nötig?"
- „Strukturiere eine 5-Why-Kette / einen Ishikawa."
- „Wie gehen wir die Ursachenanalyse an?"

**Nicht verwenden**, um eine Ursache festzustellen. Der Skill strukturiert; die Antworten auf jedes „Warum" liefert das Team mit Belegen.

## Eingaben

- Problembeschreibung, Priorität (falls bestimmt), Ergebnisse der Abweichungsanalyse, Teamnotizen.
- NC-SOP A4.9; CAPA-SOP `nordwind-sop-capa.md` B4.2, B4.3, B5.

## Vorgehen

### Teil A – CAPA-Eskalation (NC-SOP A4.9)

1. P1 → CAPA verpflichtend. P3 → vorbeugende CAPA prüfen.
2. P2 → Prüfkriterien beantworten: wiederkehrend (mehr als einmal in 12 Monaten), systemisch (Kontrolle fehlt), FSN/FSCA-Bewertung nötig, negativer Trend oder Häufung, bestehende CAPA passend?
3. Bestehende CAPA nur erweitern, wenn Problem und Umfang übereinstimmen, Projektleiter und Spezialist zustimmen und die NC vor Umsetzung der Maßnahmen auftrat.
4. Ergebnis als Vorschlag: CAPA notwendig / keine CAPA (mit Begründung) / Verknüpfung mit bestehender CAPA / Board-Entscheidung nötig.

### Teil B – Problemstellung und Ziel (CAPA-SOP B4.2)

5. Problemstellung als Soll-Ist-Differenz ohne Ursache.
6. Umfang (Produkte, Prozesse, Standorte, Zeitraum) mit begründeten Ausschlüssen.
7. Messbares CAPA-Ziel auf Fehler-, Prozess- oder Produktebene. „Mitarbeiter schulen" ist kein Ziel.

### Teil C – Untersuchungsplan (CAPA-SOP B4.3)

8. Timeline der Ereignisse aus den gelieferten Daten.
9. **Zwei getrennte 5-Why-Ketten:** Auftreten (warum entstand der Fehler?) und Entdeckung/Escape (warum hat die vorgesehene Kontrolle ihn nicht erkannt?). Bei P1 zusätzlich eine systemische Kette.
10. Jede Stufe erhält Status **belegt** (mit Nachweis) oder **offen** (mit benötigtem Beleg). Vorgeschlagene Antworten des Agenten sind immer „offen – Hypothese".
11. Ishikawa 6M (Mensch, Maschine, Methode, Material, Mitwelt, Messung) in Textform; je Einflussfaktor Status bestätigt / ausgeschlossen / offen und benötigter Beleg.
12. Sparring: Logiksprünge, Zirkelschlüsse, fehlende Belege und Widersprüche zwischen 5-Why, Ishikawa und Daten benennen.

## Ausgabeformat

**1. CAPA-Eskalation:** Vorschlag mit Begründung je Kriterium (Tabelle Kriterium | Befund | Quelle)

**2. Problemstellung, Umfang, CAPA-Ziel**

**3. 5-Why Auftreten**

| Stufe | Warum? | Antwort | Status | Beleg / benötigter Beleg |
| --- | --- | --- | --- | --- |

**4. 5-Why Entdeckung/Escape** (gleiche Tabelle)

**5. Ishikawa 6M**

| Kategorie | Einflussfaktor | Status | Beleg / Prüfschritt |
| --- | --- | --- | --- |

**6. Sparring-Hinweise** und nächste Untersuchungsschritte

## Regeln und Grenzen

- „Mitarbeiterfehler" ist keine abschließende Ursache: unterscheiden zwischen Wissen fehlt, Handlung ausgelassen, Ausführung fehlerhaft, Entscheidung fehlerhaft, und Fragen zu Vorgabe, Ergonomie, Qualifikation, Zeitdruck, Systemsicherung stellen (CAPA-SOP B4.3.5).
- Lautet eine Maßnahme nur „Schulung" oder „Sensibilisierung": nachfragen, ob ein Wissensdefizit objektiv als Ursache nachgewiesen ist (SOP C4).
- Keine Ursache als bestätigt darstellen, wenn kein Beleg vorliegt.
- Leere 6M-Kategorien als Prüfsignal nennen, nicht auffüllen.

## Prüfhinweise für den Menschen

- Gibt es eine eigene Kette für die Entdeckung?
- Woher stammt jede Antwort: aus Daten oder aus dem Agenten?
- Ist das CAPA-Ziel messbar und nicht nur eine Maßnahme?

## SOP-Bezug

NC-SOP A4.9, C4. CAPA-SOP B4.2, B4.3 (inkl. B4.3.2–B4.3.6), B5.1–B5.3.
