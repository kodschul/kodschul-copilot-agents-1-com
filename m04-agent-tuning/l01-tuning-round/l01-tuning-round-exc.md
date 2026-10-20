# Lab 4.1 – Übung: Tuning-Runde

**Dauer:** ca. 40 Minuten · Paar

## Ausgangslage

Der Bewertungsbogen Lauf 1 aus Lab 3.3 liegt vor, die zwei schwächsten Punkte sind markiert. Die Tuning-Schleife lautet: testen → bewerten → ändern → denselben Fall erneut testen.

| Datei | Zweck |
| --- | --- |
| `project/bewertungsbogen-agentenpruefung.md` | Lauf 1 (vorhanden), Lauf 2 und Tuning-Protokoll |
| `project/agent/skills/skill-0X-…md` | Skill, der den Fehler verursacht |
| `project/agent/04-nordwind-nc-capa-agent.md` | Anweisungen des Agenten |
| `project/agent/03-skill-generator.md` | Starter-Prompt „Skill nachschärfen" |
| `project/nc-capa-prompt-bibliothek.md` | Ablage bewährter Tuning-Prompts |

Wohin gehört die Änderung:

| Fehlerbild | Änderung in |
| --- | --- |
| betrifft eine Aufgabe (z. B. Aufgabenplan ohne Rückverfolgung) | Skill-Datei, `version` hochzählen |
| betrifft alle Antworten (z. B. fehlende Quellenangabe, Grenzverletzung) | Anweisungen des Agenten |
| Antwort wird nur länger | keine Änderung; längere Prompts sind kein Tuning |

## Aufgaben

1. Ordne die zwei schwächsten Punkte aus Lauf 1 einer Ebene zu (Skill-Datei oder Anweisungen) und trage sie im Tuning-Protokoll ein. (ca. 5 Min.)
2. Formuliere je Punkt die Änderung in einer Zeile. Nutze bei Bedarf den Skill-Generator mit dem Starter-Prompt „Skill nachschärfen". (ca. 10 Min.)
3. Setze die Änderung in der Skill-Datei oder den Anweisungen um und zähle die `version` hoch (z. B. von `1.0` auf `1.1`). (ca. 5 Min.)
4. Lade die geänderte Datei im Agent Builder neu hoch und warte, bis der Status „Preparing" endet. (ca. 5 Min.)
5. Lass denselben Fall erneut laufen (neuer Chat, nur Eingangsdatei). (ca. 5 Min.)
6. Fülle den Bewertungsbogen für Lauf 2 aus und trage je Punkt Vorher und Nachher ein. (ca. 5 Min.)
7. Übernimm bewährte Tuning-Prompts als Einträge in die Prompt-Bibliothek. (ca. 5 Min.)

## Checkpoint

Nach 25 Minuten:

- Lauf 2 ist bewertet.
- Vorher und Nachher sind je Punkt sichtbar.

## Abschlusskriterien

- Das Tuning-Protokoll nennt je Änderung Datei, Änderung in einer Zeile und Ergebnis in Lauf 2.
- Die geänderte Datei trägt eine höhere `version`.
- Mindestens ein Tuning-Prompt steht in der Prompt-Bibliothek.

## Erweiterung

Einen zweiten Fall mit der geänderten Version testen und prüfen, ob die Änderung dort nichts verschlechtert (Regressionstest).

## Fallback

Ohne laufenden Agenten: die geänderte Skill-Datei im normalen Copilot-Chat anhängen und den Fall mit dem Anweisungsblock als erstem Prompt erneut durchführen.
