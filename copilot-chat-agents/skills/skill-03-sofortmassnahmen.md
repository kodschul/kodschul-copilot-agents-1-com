---
name: sofortmassnahmen
description: Schlägt Isolation und Containment für eine NC vor (NC-SOP Schritt 2 und 7), getrennt von Korrekturen und CAPA-Maßnahmen, und prüft vorhandene Sofortmaßnahmen auf Lücken. Verwenden bei „Was müssen wir sofort tun?", „Reicht die Sperre?", „Ist das Containment oder Korrektur?".
version: 1.0
---

# Skill 03 – Sofortmaßnahmen: Isolation und Containment

## Wann verwenden

- „Welche Sofortmaßnahmen schlägst du vor?"
- „Reicht die bisherige Isolation aus?"
- „Ist ‚Charge verschrotten' Containment oder Korrektur?"

**Nicht verwenden** für den Aufgabenplan der Umfangsbestimmung (Skill 02) oder für ursachenbezogene Maßnahmen (Skill 05).

## Begriffe (SOP A5.4)

| Art | Zweck | Beispiele |
| --- | --- | --- |
| **Isolation** | sofort verhindern, dass betroffene Elemente weiterverwendet werden | Sperrlager, CAQ-/ERP-Statussperre, Kennzeichnung „nicht verwenden", Prüfmittelsperre |
| **Containment** | den gesamten bestätigten und potenziellen Umfang kontrollieren, bis Konformität hergestellt ist | Auslieferungsstopp, Sortierung, 100-%-Prüfung, erhöhte Stichprobe, Information betroffener Stellen |
| **Korrektur** | betroffene Elemente konform machen oder genehmigt verwenden/verwerfen | Nacharbeit, Sonderfreigabe, Verschrottung, Rücksendung |
| **CAPA-Maßnahme** | Ursache beseitigen, Wiederauftreten verhindern | Prozessänderung, Poka-Yoke, Prüfplanänderung |

## Eingaben

- Problembeschreibung (Skill 01) oder Erstmeldung mit den bereits umgesetzten Maßnahmen.
- NC-SOP `nordwind-sop-nc.md`, Abschnitte A4.2, A4.7, A4.8, A5.4.

## Vorgehen

1. Liste die bereits dokumentierten Maßnahmen und ordne jede einer Art zu (Isolation, Containment, Korrektur, CAPA-Maßnahme, **keine Sofortmaßnahme** – z. B. „Sensibilisierung geplant").
2. Prüfe die Isolation gegen die Pflichtfragen A4.2: Was muss sofort gestoppt werden, was ist sicher und was potenziell betroffen, wirkt die Sperre physisch **und** im führenden System, sind alle Standorte und externen Fertiger berücksichtigt, ist Produkt außerhalb der Kontrolle?
3. Steht „keine Isolation" in der Meldung: begründen lassen oder Isolation vorschlagen.
4. Schlage fehlende Isolations- und Containment-Maßnahmen risikobasiert vor, je mit Verantwortlicher Rolle, Frist und Aufhebungskriterium.
5. Ist Produkt potenziell außerhalb der Kontrolle von Nordwind Medical: Einbindung der Rollen für Vigilanz/FSN/FSCA und SiBa/QP als Prüfpunkt nennen.
6. Nenne mögliche Korrekturen nur als Ausblick und kennzeichne sie als Korrektur (Entscheidung nach Umfangsbestimmung und Risikobewertung).

## Ausgabeformat

**1. Kurzfazit** (ist der Fall ausreichend gesichert?)

**2. Bewertung vorhandener Maßnahmen**

| Maßnahme (wörtlich) | Art | Wirksam für | Lücke |
| --- | --- | --- | --- |

**3. Vorschläge Isolation / Containment**

| Nr. | Maßnahme | Art | Umfang | Rolle | Frist | Aufhebungskriterium |
| --- | --- | --- | --- | --- | --- | --- |

**4. Ausblick Korrektur** (kurz, als Vorschlag)

**5. Eskalationspunkte** (Produkt außerhalb Kontrolle, Auslieferungsstopp zu prüfen, Genehmigung nötig)

## Regeln und Grenzen

- Containment nie als Korrektur bezeichnen und umgekehrt.
- „Sensibilisierung" oder „Schulung" ist keine Sofortmaßnahme gegen betroffene Elemente.
- Keine Freigabe oder Aufhebung vorschlagen, ohne objektives Kriterium.
- Umsetzung und Genehmigung liegen beim Menschen (bei P1 zusätzlich QMS-Genehmiger).

## Prüfhinweise für den Menschen

- Ist jede Maßnahme der richtigen Art zugeordnet?
- Deckt das Containment auch den **potenziellen** Umfang ab?
- Gibt es ein Kriterium, wann die Sperre aufgehoben wird?

## SOP-Bezug

NC-SOP A4.2 (Isolation), A4.6 (Auslieferungsstopp), A4.7 (Containment), A4.8 (Korrekturen), A5.4.
