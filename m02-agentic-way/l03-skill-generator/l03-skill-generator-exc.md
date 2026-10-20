# Lab 2.3 – Übung: Skill-Datei schreiben

**Dauer:** ca. 35 Minuten · Paar

## Ausgangslage

Das Konzept mit der Skill-Liste liegt vor. Jedes Paar wählt einen der sechs Skills; die Gruppe deckt alle sechs ab. Der Skill-Generator ist vom Trainer geteilt.

| Datei | Zweck |
| --- | --- |
| `project/agent/03-skill-generator.md` | Assistent, Starter-Prompt „Skill aus Konzept" |
| `project/sop/nordwind-sop-nc.md`, `project/sop/nordwind-sop-capa.md` | SOP-Abschnitte |
| `project/prompt-karten-hitl.md`, `project/nc-capa-prompt-bibliothek.md` | HITL-Prompt aus Lab 1.3 (Eintrag 1) |
| `project/faelle/nc-02-stueckzahl-part1-eingang.docx` | Testmeldung |

SOP-Abschnitte je Skill:

| Skill | SOP-Abschnitt |
| --- | --- |
| 01 Erstbewertung | NC A4.1, A4.4 |
| 02 Aufgabenplan | NC A4.5 |
| 03 Sofortmaßnahmen | NC A4.2, A4.7 |
| 04 Risiko und Priorität | NC A4.6 |
| 05 CAPA-Eskalation | NC A4.9, CAPA B4.2–B4.3 |
| 06 Bearbeitung prüfen | NC A5, C5, CAPA B5 |

## Aufgaben

1. Wähle einen Skill aus der Liste und notiere Nummer und Name. (ca. 3 Min.)
2. Öffne den Skill-Generator und sende den Starter-Prompt „Skill aus Konzept" mit dem Konzepteintrag des Skills, dem SOP-Abschnitt und dem HITL-Prompt aus Lab 1.3. (ca. 10 Min.)
3. Speichere die gelieferte Skill-Datei als Markdown unter `skill-<nr>-<name>.md`. (ca. 3 Min.)
4. Prüfe die Datei auf Frontmatter (`name`, `description`, `version`) und die sieben Abschnitte von „Wann verwenden" bis „SOP-Bezug". Ergänze Fehlendes mit einer Nachfrage an den Generator. (ca. 7 Min.)
5. Öffne einen neuen Copilot-Chat, hänge Skill-Datei und Meldung NC-02 (Part 1) an, stelle die Aufgabe des Skills und vergleiche die Antwort mit dem Ausgabeformat der Datei. (ca. 7 Min.)
6. Zeige im Debrief die Skill-Datei der Gruppe. (ca. 5 Min.)

## Checkpoint

Nach 23 Minuten:

- Die Skill-Datei liegt vor.
- Sie enthält Ausgabeformat und Grenzen.

## Abschlusskriterien

- Eine Skill-Datei mit Frontmatter und allen sieben Abschnitten ist gespeichert.
- Der Kurztest an NC-02 ist durchgeführt, Abweichungen vom Ausgabeformat sind notiert.

## Erweiterung

Zweiten Skill aus der Liste erzeugen und prüfen, ob sich die Beschreibungen der beiden Skills klar abgrenzen.

## Fallback

Ohne Zugriff auf den Skill-Generator: die Referenzdatei aus `project/agent/skills/` verwenden und Aufgabe 4 bis 6 daran durchführen.
