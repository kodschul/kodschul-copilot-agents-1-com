# Lab 3.1 – Übung: Agent zusammensetzen

## Ausgangslage

Der Nordwind-NC/CAPA-Agent wird im Agent Builder aus dem vorbereiteten Gerüst angelegt. Bereitgestellt in `output/project/`:

- `agent/04-nordwind-nc-capa-agent.md` – Felder, Anweisungen, Starter-Prompts
- `sop/nordwind-sop-nc.md`, `sop/nordwind-sop-capa.md` – SOPs als Wissen
- `agent/skills/skill-01-nc-erstbewertung.md` bis `skill-06-bearbeitung-pruefen.md` – Referenz-Skills
- `faelle/nc-02-stueckzahl-part1-eingang.docx` – Testfall (nur Part 1)
- die eigene Skill-Datei aus Lab 2.3

## Aufgaben

1. Öffne Microsoft 365 Copilot Chat → Agent erstellen → Konfigurieren. Trage Name und Beschreibung aus `agent/04-nordwind-nc-capa-agent.md` ein und kopiere den Codeblock unter „Anweisungen“ in das Feld Anweisungen.
2. Lade als Wissen die beiden SOPs und die sechs Skill-Dateien hoch (alle als `.md`).
3. Ersetze die Referenz-Skill-Datei der eigenen Aufgabe durch die Datei aus Lab 2.3 oder lade sie zusätzlich hoch. Notiere die Dateiliste mit Version.
4. Deaktiviere die Websuche, übernehme die vier Starter-Prompts aus dem Gerüst und speichere den Agenten.
5. Warte, bis alle Dateien nach „Preparing“ bereit sind.
6. Gib NC-02 Part 1 in den Agenten (Datei anhängen oder Inhalt einfügen) und starte mit dem Starter-Prompt „Neue NC vorbereiten“.
7. Prüfe die Antwort: Folgt sie dem Standardablauf mit fünf Teilen? Nennt die erste Zeile die genutzten Skill-Dateien, darunter den eigenen Skill?

## Checkpoint

- Alle Wissensdateien zeigen den Status bereit.
- Die Antwort enthält die Zeile mit den genutzten Skill-Dateien.
- Die Antwort gliedert sich in Erstbewertung, Sofortmaßnahmen, Aufgabenplan, Risiko/Priorität und CAPA-Hinweis.

## Abschlusskriterien

- Der Agent ist gespeichert und läuft mit eigenem Skill im Wissen.
- Die Dateiliste mit Version ist notiert.
- Die Antwort des Smoke-Tests ist unverändert gesichert (Grundlage für Lab 3.3).

## Erweiterung

Dieselbe Meldung mit dem Starter-Prompt „Was ist zu tun?“ absenden und prüfen, ob die Skill-Zeile jetzt auf Skill 02 zeigt.

## Fallback

Ohne Agent Builder: den Codeblock der Anweisungen als ersten Prompt in einen neuen Copilot-Chat-Verlauf einfügen und SOPs sowie Skill-Dateien anhängen. Einschränkung: nicht teilbar und ohne gespeicherte Konfiguration; Starter-Prompts entfallen, die Prompts werden von Hand eingegeben.
