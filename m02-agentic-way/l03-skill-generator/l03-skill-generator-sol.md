# Lab 2.3 – Lösung: Skill-Datei schreiben

Der Skill-Generator formuliert bei jedem Lauf anders. Maßstab ist die Referenzdatei in `project/agent/skills/`; die Lösung zeigt die Prüfpunkte und das erwartete Verhalten beim Kurztest.

## Aufgabe 1: Skill wählen

Die sechs Referenzdateien und ihre Namen:

| Nr. | Datei | `name` |
| --- | --- | --- |
| 01 | `skill-01-nc-erstbewertung.md` | `nc-erstbewertung` |
| 02 | `skill-02-aufgabenplan-abweichungsanalyse.md` | `aufgabenplan-abweichungsanalyse` |
| 03 | `skill-03-sofortmassnahmen.md` | `sofortmassnahmen` |
| 04 | `skill-04-risiko-prioritaet-vorbereiten.md` | `risiko-prioritaet-vorbereiten` |
| 05 | `skill-05-capa-eskalation-ursachenplan.md` | `capa-eskalation-ursachenplan` |
| 06 | `skill-06-bearbeitung-pruefen.md` | `bearbeitung-pruefen` |

## Aufgabe 2: Prompt an den Generator

Starter-Prompt der Datei `03-skill-generator.md`, am Beispiel Skill 02:

```text
Erstelle den Skill „aufgabenplan-abweichungsanalyse" nach diesem Übergabepaket: [Konzepteintrag, SOP-Abschnitt NC A4.5 und HITL-Prompt aus Lab 1.3 einfügen]
```

## Aufgabe 3 und 4: Datei und Prüfung

Eine vollständige Skill-Datei erfüllt diese Punkte (Beispiel Skill 02):

| Prüfpunkt | Erwartung | Beispiel aus Skill 02 |
| --- | --- | --- |
| Frontmatter | `name` (Kleinbuchstaben, Bindestriche), `description` mit Zweck und Auslösern, `version` | `name: aufgabenplan-abweichungsanalyse`, `version: 1.0` |
| Wann verwenden | drei Nutzerfragen, dazu wann nicht | „Was müssen wir jetzt prüfen, um den Umfang zu bestimmen?"; nicht für Sofortmaßnahmen (Skill 03) |
| Eingaben | Pflicht und optional, SOP-Abschnitt | Problembeschreibung (Skill 01), NC-SOP A4.5 |
| Vorgehen | nummerierte, prüfbare Schritte | je Pflichtfrage der SOP mindestens eine Aufgabe ableiten |
| Ausgabeformat | feste Überschriften und Tabellenköpfe | Tabelle „Nr. \| Aufgabe \| Pflichtfrage (SOP A4.5) \| Datenquelle \| Rolle \| Priorität" |
| Regeln und Grenzen | was beim Menschen bleibt | Agent schlägt Aufgaben vor, Daten beschafft das Team; keine Nummern erfinden |
| SOP-Bezug | Abschnitte | NC-SOP A4.5, A5.2, A5.5 |

## Aufgabe 5: Kurztest an NC-02 Part 1

Bei Skill 02 zielt ein brauchbarer Aufgabenplan mindestens auf diese Punkte (alle aus der Meldung ableitbar):

| Aufgabe | Pflichtfrage |
| --- | --- |
| Menge in allen Arbeitsgängen des Fertigungsauftrags FA-EX-2055 mit dem Dienstleister-Protokoll und dem Prüfauftrag PA-EX-10000 abgleichen | seitdem bearbeitete Vorgänge, Entdeckungsmethode |
| Verbleib und Status des Materials klären | betroffene Elemente |
| weitere Aufträge desselben Dienstleisters oder mit derselben Prüfung AG 150 auf gleiche Abweichung prüfen | baugleiche Prozesse, Zuverlässigkeit der Entdeckung |

Abweichungen vom Ausgabeformat der Datei (fehlende Spalte, Ergebnisse statt Aufgaben, erfundene Nummern) sind ein Befund für die Skill-Datei, nicht für die Meldung.

## Valide Alternative

Ein anderer Skill (01 bis 06) führt zu einer anderen Datei und anderen Testerwartungen. Maßstab bleiben Frontmatter, sieben Abschnitte, Ausgabeformat und Grenze „Mensch entscheidet".
