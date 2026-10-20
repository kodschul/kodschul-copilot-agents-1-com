# Lab 3.1 – Lösung: Agent zusammensetzen

## Aufgabe 1: Agent anlegen

| Feld | Eintrag |
| --- | --- |
| Name | Nordwind-NC/CAPA-Assistent |
| Beschreibung | Text aus `agent/04-nordwind-nc-capa-agent.md` (endet mit „Entscheidet nichts.“) |
| Anweisungen | Codeblock unverändert, beginnt mit `# Rolle`, endet mit dem Hinweis „Vorschlag – Prüfung und Entscheidung durch die zuständige Rolle.“ |

## Aufgabe 2 und 3: Wissen und eigener Skill

Beispiel für ein Paar, das Skill 02 selbst geschrieben hat (Ersetzen):

| Datei | Version | Herkunft |
| --- | --- | --- |
| `nordwind-sop-nc.md` | – | Projekt |
| `nordwind-sop-capa.md` | – | Projekt |
| `skill-01-nc-erstbewertung.md` | 1.0 | Referenz |
| `skill-02-aufgabenplan-abweichungsanalyse.md` | 1.0 | eigene Datei aus Lab 2.3 |
| `skill-03` bis `skill-06` | 1.0 | Referenz |

Beim Ergänzen statt Ersetzen sind es neun Dateien, die eigene Datei braucht dann eine abweichende `description`, damit sie sich vom Referenz-Skill abgrenzt.

## Aufgabe 4 und 5: Konfiguration

- Funktionen: keine, Websuche aus.
- Starter-Prompts: „Neue NC vorbereiten“, „Was ist zu tun?“, „CAPA und 5-Why“, „Bearbeitung prüfen“.
- Bereit, wenn jede Datei den Status „Preparing“ verlassen hat.

## Aufgabe 6 und 7: Smoke-Test

Erwartete Form der Antwort auf „Neue NC vorbereiten“ mit NC-02 Part 1 (Aufbau laut Instruktion, Inhalt variiert je Lauf):

```text
Genutzte Skills: skill-01-nc-erstbewertung, skill-03-sofortmassnahmen, skill-02-aufgabenplan-abweichungsanalyse, ...
1. Erstbewertung und Problembeschreibung
2. Sofortmaßnahmen
3. Aufgabenplan
4. Risiko und Priorität (Vorbereitung)
5. CAPA-Eskalation (Hinweis)
Offene Punkte
Vorschlag – Prüfung und Entscheidung durch die zuständige Rolle.
```

Bestanden: Skill-Zeile vorhanden, fünf Teile in Reihenfolge, eigener Skill genannt. Fehlt der eigene Skill in der Zeile, passen `description` und Anfrage nicht zusammen: Beschreibung der Skill-Datei prüfen (Lab 4.1).
