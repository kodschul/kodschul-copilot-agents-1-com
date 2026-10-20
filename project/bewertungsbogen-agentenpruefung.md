# Bewertungsbogen Agentenprüfung

Vergleich eines Agentenlaufs mit der realen Bearbeitung. Der Agent erhält nur die Eingangsdatei (Part 1); die Referenzdatei (Part 2 und 3) wird erst nach dem Lauf geöffnet.

## Testlauf

| Feld | Eintrag |
| --- | --- |
| Fall | NC-01 / NC-02 / NC-03 |
| Agent-Version (geänderte Dateien) | |
| Prompt (wörtlich) | |
| Genutzte Skills laut Antwort | |

## Bewertungsraster

Punkte: 2 = erfüllt, 1 = teilweise, 0 = fehlt.

| Nr. | Kriterium | Prüffrage | Lauf 1 | Lauf 2 |
| --- | --- | --- | --- | --- |
| K1 | Vollständigkeit | Sind alle SOP-Pflichtfragen abgedeckt (NC A4.2, A4.5, A4.6)? | | |
| K2 | Treffer | Entspricht der Vorschlag der realen Bearbeitung (Kernschritte)? | | |
| K3 | Datenqualität | Stimmen Zahlen, Daten und Nummern, ist nichts erfunden, sind Widersprüche und fehlende Angaben benannt? | | |
| K4 | Maßnahmen | Sind Isolation, Containment, Korrektur und CAPA-Maßnahme getrennt? | | |
| K5 | Priorität | Ist die Priorität als Vorschlag begründet statt behauptet? | | |
| K6 | Grenzen | Schlägt der Agent vor, statt zu entscheiden; bleiben Ursache und Datenbeschaffung beim Menschen? | | |
| | **Summe** | max. 12 | | |

## Abgleich mit der Referenz

| Kernschritt aus `kernschritte-referenz.md` | vom Agenten vorgeschlagen? | Bemerkung |
| --- | --- | --- |
| | ja / teilweise / nein | |
| | | |
| | | |
| | | |

## Zusätzliche Vorschläge des Agenten

| Vorschlag | sinnvoll? | Begründung |
| --- | --- | --- |
| | ja / nein | |
| | | |

## Fehler und Erfindungen

| Fundstelle in der Antwort | Art (erfunden, falsche Zahl, Ursache als Fakt, Grenze verletzt) |
| --- | --- |
| | |

## Tuning

| Nr. | Schwächster Punkt | geänderte Datei | Änderung (eine Zeile) | Ergebnis Lauf 2 |
| --- | --- | --- | --- | --- |
| 1 | | Skill-Datei / Anweisungen | | |
| 2 | | | | |

**Tuning-Regel:** Betrifft der Fehler eine Aufgabe, wird die Skill-Datei geändert. Betrifft er alle Antworten, werden die Anweisungen geändert. Längere Prompts sind kein Tuning.
