# Szenario: Nordwind Medical

Nordwind Medical ist ein fiktiver Hersteller von Medizinprodukten mit zwei Fertigungsstandorten (Standort A und B) und externen Dienstleistern. Das QS-Team bearbeitet Nichtkonformitäten (NC) und CAPAs nach zwei SOPs. Alle Personen-, Artikel-, Chargen-, Auftrags- und Dokumentnummern sind anonymisiert.

## Prozesse und Vorgaben

| Datei | Inhalt | Wichtigste Abschnitte |
| --- | --- | --- |
| [`sop/nordwind-sop-nc.md`](sop/nordwind-sop-nc.md) | NC-Prozess in 10 Schritten | A4.1 NC-Relevanz, A4.2 Isolation, A4.4 Problembeschreibung, A4.5 Umfang, A4.6 Risiko/Priorität, A4.7 Containment, A4.9 CAPA-Eskalation, A5 typische Fehler, C4 Prüfregeln, C5 Qualitätsgate |
| [`sop/nordwind-sop-capa.md`](sop/nordwind-sop-capa.md) | CAPA-Prozess in 12 Schritten | B4.2 Problemstellung und Ziel, B4.3 Ursachenanalyse, B4.5 Maßnahmenplan, B4.6 Wirksamkeit, B5 typische Fehler |

## Rollen

| Rolle | Aufgabe im Prozess |
| --- | --- |
| NC-Entdecker | erfasst die Beobachtung, isoliert, meldet |
| NC-Eigner | verantwortet Problembeschreibung, Umfang, Containment, Korrektur |
| NC/CAPA-Spezialist | prüft Vollständigkeit, bewertet CAPA-Bedarf, genehmigt Containment |
| SiBa / QP | Gesundheitsrisikobewertung (HHE) bei hoher Schadensschwere |
| QMS-Genehmiger | zusätzliche Genehmigung bei P1 und Abschluss |
| CAPA Board | entscheidet über CAPA bei P2 |

## Systeme

| System | Inhalt | Zugriff des Agenten |
| --- | --- | --- |
| ERP | Bestände, Aufträge, Chargen, Verwendungsnachweis | kein Zugriff |
| CAQ-System | NC- und CAPA-Vorgänge, Prüfaufträge, Prüfmittel, Mängel | kein Zugriff |
| DMS | gelenkte Vorgabedokumente | kein Zugriff |

Der Agent schlägt Aufgaben vor; Mitarbeitende beschaffen die Daten aus diesen Systemen und entscheiden.

## Die drei Fälle

Jeder Fall liegt in zwei Dateien vor: **Eingang** (Part 1, Erstmeldung, einzige Eingabe für den Agenten) und **Referenz** (Part 2 und 3, reale Bearbeitung und Risikobewertung des Teams).

| Fall | Kern | Eingang | Referenz |
| --- | --- | --- | --- |
| NC-01 Prüfmittel | 78 Prüfmittel nach Inventur nicht am Lagerplatz, Prüfintervall eventuell überschritten | [`nc-01-pruefmittel-part1-eingang.docx`](faelle/nc-01-pruefmittel-part1-eingang.docx) | [`nc-01-pruefmittel-part2-3-referenz.docx`](faelle/nc-01-pruefmittel-part2-3-referenz.docx) |
| NC-02 Stückzahl | Dienstleister-Protokoll 201 statt 200 Stück, Prüfung in AG 150 hat nicht entdeckt | [`nc-02-stueckzahl-part1-eingang.docx`](faelle/nc-02-stueckzahl-part1-eingang.docx) | [`nc-02-stueckzahl-part2-3-referenz.docx`](faelle/nc-02-stueckzahl-part2-3-referenz.docx) |
| NC-03 Druckmessdosen | zwei Druckmessdosen bei der Endprüfung unterhalb der Schweißnaht geplatzt | [`nc-03-druckmessdosen-part1-eingang.docx`](faelle/nc-03-druckmessdosen-part1-eingang.docx) | [`nc-03-druckmessdosen-part2-3-referenz.docx`](faelle/nc-03-druckmessdosen-part2-3-referenz.docx) |

## Datenregeln

- Nur die anonymisierten Nordwind-Dateien verwenden.
- Keine Patientendaten, keine personenbezogenen Daten, keine echten Chargen- oder Auftragsnummern in Prompts.
- Jedes KI-Ergebnis ist ein Vorschlag. Prüfung und Entscheidung liegen bei der zuständigen Rolle.
