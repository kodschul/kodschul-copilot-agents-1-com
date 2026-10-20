# Lab 2.1 – Übung: Problem-Solver bauen und einsetzen

**Dauer:** ca. 35 Minuten · Bau einzeln, Canvas im Paar

## Ausgangslage

Aus der Vorstellungsrunde: Die NC-Bearbeitung dauert lange, wichtige Prüfschritte werden vergessen, die Qualität der Dokumentation schwankt. Der Problem-Solver bewertet dieses Problem als Agent-Use-Case.

| Datei | Zweck |
| --- | --- |
| `project/agent/01-problem-solver.md` | Name, Beschreibung, Anweisungen, Starter-Prompts |
| `project/sop/nordwind-sop-nc.md`, `project/sop/nordwind-sop-capa.md` | Wissen des Agenten |

## Aufgaben

1. Öffne Microsoft 365 Copilot Chat und wähle **Neuer Agent** → **Konfigurieren** (bzw. „Skip to configure"). (ca. 2 Min.)
2. Trage Name und Beschreibung aus `01-problem-solver.md` ein. (ca. 3 Min.)
3. Kopiere den Block „Anweisungen" (Codeblock) in das Feld Anweisungen. (ca. 3 Min.)
4. Lade `nordwind-sop-nc.md` und `nordwind-sop-capa.md` als Wissen hoch, trage zwei Starter-Prompts aus der Tabelle der Datei ein und speichere den Agenten. (ca. 7 Min.)
5. Teste mit einem kurzen Alltagsproblem. (ca. 3 Min.)
6. Gib das NC-Problem ein („Die NC-Bearbeitung dauert lange, wichtige Prüfschritte werden vergessen, die Qualität der Dokumentation schwankt") und beantworte die Rückfragen mit dem Zeitfresser aus der Vorstellungsrunde. (ca. 7 Min.)
7. Prüfe den Use-Case-Canvas (sieben Felder), wähle im Paar die Top-1-Empfehlung und notiere die Begründung. (ca. 10 Min.)

## Checkpoint

- Der Agent stellt Rückfragen, statt sofort eine Lösung zu liefern.
- Der Canvas ist ausgefüllt, die Top-1-Empfehlung ist begründet.

## Abschlusskriterien

- Der Agent „Problem-Solver QS" ist gespeichert und antwortet.
- Canvas und Top-1-Empfehlung liegen als Notiz vor (Eingabe für Lab 2.2).

## Fallback

Ohne freigegebenen Agent Builder: den Anweisungsblock als ersten Prompt in einen neuen Copilot-Chat einfügen und die beiden SOPs anhängen. Das Verhalten ist gleich, der Chat ist nicht gespeichert und nicht teilbar.
