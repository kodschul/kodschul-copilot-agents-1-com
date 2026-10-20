# Überblick: Copilot Agents im Qualitätsalltag

Ein Tag für das QS-Team von Nordwind Medical. Das Team nutzt Microsoft 365 Copilot Chat, um aus einem einzelnen Prompt einen geteilten NC/CAPA-Agenten zu bauen: zuerst mit drei Assistenten konzipieren, danach zusammensetzen, an echten Fällen prüfen und tunen.

## Ziel

Am Ende des Tages liegen vor:

- ein erprobter Prompt mit Mensch in the loop für die NC-Problembeschreibung und eine Prüfcheckliste,
- ein selbst gebauter Problem-Solver, ein Agentenkonzept mit Skill-Liste und eigene Skill-Dateien,
- ein zusammengesetzter Nordwind-NC/CAPA-Agent, gegen reale Bearbeitungen geprüft und getunt,
- ein im Team geteilter Agent mit Pflegeplan und ein persönlicher Aktionsplan.

## Ausgangslage: KI-Wildwuchs

Jede Person im Team nutzt KI anders: eigene Prompts, andere Tools, Fälle im privaten Chat. Das Ergebnis ist uneinheitlich und lässt sich bei NC und CAPA schwer nachvollziehen. Ein geteilter Agent mit SOP als Quelle, geprüften Skills und benanntem Owner ersetzt diesen Wildwuchs durch einen Standard. Die Entscheidung bleibt beim QS-Team.

## Zielgruppe und Voraussetzungen

| Punkt | Festlegung |
| --- | --- |
| Zielgruppe | QS-/QM-Team eines Medizinprodukte-Herstellers, bearbeitet NC (Abweichungen) und CAPA |
| Vorkenntnisse | Grundnutzung von Copilot Chat; keine Programmierkenntnisse |
| Lizenz und Zugang | Microsoft 365 Copilot, Copilot Chat im Browser (`m365.cloud.microsoft`) |
| Freigaben | Agenten erstellen und teilen (Agent Builder), Upload von `.md`-Dateien als Wissen |
| Dateien | Projektordner [`project/`](../project/README.md) lokal bereit |

## Szenario

Nordwind Medical stellt Medizinprodukte an zwei Standorten her. NCs laufen nach einer NC-SOP in zehn Schritten, CAPAs nach einer CAPA-SOP. Drei anonymisierte Fälle begleiten den Tag:

| Fall | Kern | Einsatz |
| --- | --- | --- |
| NC-01 Prüfmittel | 78 Prüfmittel nach Inventur nicht am Lagerplatz | Lab 1.3, Lab 3.3 |
| NC-02 Stückzahl | Dienstleister-Protokoll 201 statt 200 Stück, Prüfung in AG 150 hat den Fehler nicht erkannt | Lab 1.1, 2.3, 3.1, 3.2, 3.3, 4.1 |
| NC-03 Druckmessdosen | zwei Druckmessdosen bei der Endprüfung unterhalb der Verschweißung geplatzt | Lab 3.2, 3.3, 4.1 |

Der Agent hat keinen Zugriff auf ERP, CAQ-System oder DMS. Er schlägt Aufgaben und Sofortmaßnahmen vor; Daten beschaffen, bewerten und entscheiden bleibt beim Team.

## Tagesablauf

| Zeit | Programm | Handouts |
| --- | --- | --- |
| 09:00–10:30 | Auftakt und Modul 1: Vom KI-Wildwuchs zum Agenten (Lab 1.1–1.3) | [`m01-ai-essentials/`](../m01-ai-essentials/) |
| 10:30–10:45 | Pause | |
| 10:45–12:15 | Modul 2: KI baut KI, drei Assistenten (Lab 2.1–2.3) | [`m02-agentic-way/`](../m02-agentic-way/) |
| 12:15–13:15 | Mittagspause | |
| 13:15–14:45 | Modul 3: Der konkrete Use Case (Lab 3.1–3.3) | [`m03-build-nc-capa-agent/`](../m03-build-nc-capa-agent/) |
| 14:45–15:00 | Pause | |
| 15:00–16:00 | Modul 4: Tunen und gemeinsam reviewen (Lab 4.1–4.2) | [`m04-agent-tuning/`](../m04-agent-tuning/) |
| 16:00–16:30 | Modul 5: Teilen, pflegen, übertragen (Lab 5.1–5.2) | [`m05-share-and-transfer/`](../m05-share-and-transfer/) |

Zeiten flexibel, je nach Abstimmung.

## Arbeitsweise

- Zwei Übungsarten: Prompten mit Mensch in the loop (Lab 1.3), sonst Agenten bauen, zusammensetzen, prüfen und tunen.
- Lab 1.1, 1.2 und 3.2 sind Showcases, Lab 4.2 und 5.1 laufen im Plenum.
- Jedes Lab hat ein Handout `-thx` (Kernaussagen); Labs mit Übung zusätzlich `-exc` (Aufgaben) und `-sol` (Musterlösung).
- Regeln für alle Fälle: nur die Eingangsdatei an den Agenten geben, Antwort sichern, erst danach die Referenz öffnen.
- Datenregel: keine Patientendaten, keine personenbezogenen Daten, keine echten Chargen- oder Auftragsnummern.
