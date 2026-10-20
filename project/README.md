# Projektdateien – Nordwind Medical

Übungsdateien für den Kurs. Die drei Fälle liegen wie echte NC-Vorgänge als Word-Dateien vor; alle übrigen Dateien sind Markdown. Szenario, Rollen und Systeme: [`szenarien.md`](szenarien.md).

## Dateien

| Datei | Inhalt | Verwendet in |
| --- | --- | --- |
| [`szenarien.md`](szenarien.md) | Nordwind Medical, Rollen, Systeme, Fallübersicht, Datenregeln | alle Labs |
| [`sop/nordwind-sop-nc.md`](sop/nordwind-sop-nc.md) | NC-Prozess (Schulungsfassung) | Lab 1.2, Lab 1.3, Lab 2.2, Wissen des Agenten |
| [`sop/nordwind-sop-capa.md`](sop/nordwind-sop-capa.md) | CAPA-Prozess (Schulungsfassung) | Lab 2.2, Lab 3.2, Wissen des Agenten |
| [`faelle/nc-01-pruefmittel-part1-eingang.docx`](faelle/nc-01-pruefmittel-part1-eingang.docx) | Erstmeldung NC-01 Prüfmittel | Lab 1.3, Lab 3.3 |
| [`faelle/nc-02-stueckzahl-part1-eingang.docx`](faelle/nc-02-stueckzahl-part1-eingang.docx) | Erstmeldung NC-02 Stückzahl | Lab 1.1, Lab 2.3, Lab 3.1, Lab 3.2, Lab 3.3, Lab 4.1 |
| [`faelle/nc-03-druckmessdosen-part1-eingang.docx`](faelle/nc-03-druckmessdosen-part1-eingang.docx) | Erstmeldung NC-03 Druckmessdosen | Lab 3.2, Lab 3.3, Lab 4.1 |
| `faelle/*-part2-3-referenz.docx` | reale Bearbeitung und Risikobewertung je Fall | Lab 3.3, Lab 4.1 (erst nach dem Agentenlauf öffnen) |
| [`kernschritte-referenz.md`](kernschritte-referenz.md) | Kernschritte der realen Bearbeitung je Fall (Kurzfassung der Referenzdateien) | Lab 3.3, Lab 4.1 (erst nach dem Agentenlauf öffnen) |
| [`prompt-karten-hitl.md`](prompt-karten-hitl.md) | Zero-Shot-Karte, Few-Shot-Karte mit NC-02-Muster, Feedback-Prompts, fünf Prüfpunkte | Lab 1.3 |
| [`nc-capa-prompt-bibliothek.md`](nc-capa-prompt-bibliothek.md) | Vorlage der Prompt-Bibliothek | Lab 1.3, Lab 4.1, Lab 5.2 |
| [`agenten-output-mit-fehlern.md`](agenten-output-mit-fehlern.md) | Agentenantwort mit fünf eingebauten Fehlern | Lab 3.2 |
| [`bewertungsbogen-agentenpruefung.md`](bewertungsbogen-agentenpruefung.md) | Raster für den Abgleich Agent vs. reale Bearbeitung, Tuning-Protokoll | Lab 3.3, Lab 4.1 |
| [`agent/`](agent/) | Anweisungen der Assistenten 1–3 (`01`–`03`), Gerüst des NC/CAPA-Agenten (`04`), sechs Referenz-Skills (`skills/`) | Lab 2.1–2.3, Lab 3.1, Lab 4.1 |

## Arbeitsregel für die Fälle

1. Nur die **Eingangsdatei** an den Agenten geben.
2. Antwort sichern.
3. Erst dann die **Referenzdatei** öffnen und mit dem Bewertungsbogen abgleichen.

So bleibt der Vergleich fair: Der Agent kennt nur, was auch bei einer echten Erstmeldung vorliegt.
