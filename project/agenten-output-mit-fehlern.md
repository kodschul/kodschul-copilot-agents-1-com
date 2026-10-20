# Agenten-Output mit Fehlern (Showcase Lab 3.2)

Antwort eines Agenten auf die Meldung [`faelle/nc-02-stueckzahl-part1-eingang.docx`](faelle/nc-02-stueckzahl-part1-eingang.docx). Die Antwort enthält **fünf Fehler**. Grundlage für die Prüfung sind die Eingangsdatei und die NC-SOP.

---

**Genutzte Skills:** skill-01-nc-erstbewertung, skill-03-sofortmassnahmen, skill-05-capa-eskalation-ursachenplan

### 1. Kurzfazit

Bei der Wareneingangsprüfung von FA-EX-2055 wurde eine Mengenabweichung von einem Stück festgestellt. Die Abweichung ist eine tatsächliche NC (Vorschlag, Entscheidung NC-Eigner).

### 2. Problembeschreibung

| Feld | Inhalt | Quelle |
| --- | --- | --- |
| Soll | 200 Stück laut Fertigungsauftrag FA-EX-2055 | Meldung |
| Ist | 201 Stück laut Ausführungsprotokoll des Dienstleisters | Meldung |
| Differenz | 1 Stück Mehrmenge | Meldung |
| Ort | AG 190 „Wareneingangsprüfung Standort A Dienstleister B" | Meldung |
| Zeit | Auftreten 2024-09-10, Kenntnisnahme 2024-09-19 | Meldung |
| Objekt | FA-EX-2055, Charge CH-EX-5120, Prüfauftrag PA-EX-10000 | Meldung |
| Umfang | 201 Stück | Meldung |
| Entdeckung | AG 190; in AG 150 hat die Prüferin die Stückzahl nicht sorgfältig abgeglichen | Meldung |

### 3. Sofortmaßnahmen

| Nr. | Maßnahme | Art | Rolle |
| --- | --- | --- | --- |
| 1 | Material von FA-EX-2055 im CAQ-System und physisch sperren | Korrektur | NC-Eigner |
| 2 | Mengenabgleich aller Arbeitsgänge des FA mit dem Dienstleister-Protokoll | Aufgabe Umfang | NC-Eigner |

### 4. Priorität

Vorschlag: P2. Begründung: tatsächliche NC; aus der Meldung ergibt sich kein Hinweis auf externes Audit, FDA Warning Letter oder Form 483 (NC-SOP A4.6). Bestätigung durch die zuständige Rolle.

### 5. CAPA

Eine CAPA ist nicht nötig. Als Maßnahme wird die Prüferin in AG 150 geschult, damit die Stückzahl künftig sorgfältig abgeglichen wird.

### 6. Offene Punkte

1. Wo befindet sich das Material aktuell?
2. Gibt es weitere Aufträge mit Dienstleister B mit gleicher Abweichung?

*Vorschlag – Prüfung und Entscheidung durch die zuständige Rolle.*
