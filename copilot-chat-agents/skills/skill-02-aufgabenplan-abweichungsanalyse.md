---
name: aufgabenplan-abweichungsanalyse
description: Erstellt aus einer NC-Meldung einen Aufgabenplan für die Abweichungsanalyse und Umfangsbestimmung (NC-SOP Schritt 5) mit Pflichtfrage, Datenquelle und Rolle je Aufgabe. Verwenden bei „Was ist zu tun?", „Welche Daten brauchen wir?", „Welche Chargen/Prüfmittel/Aufträge könnten betroffen sein?".
version: 1.0
---

# Skill 02 – Aufgabenplan für die Abweichungsanalyse

## Wann verwenden

- „Was müssen wir jetzt prüfen, um den Umfang zu bestimmen?"
- „Welche Daten fehlen für die vollständige Abweichungsanalyse?"
- „Welche weiteren Chargen, Produkte oder Prüfaufträge könnten betroffen sein?"

**Nicht verwenden** für Sofortmaßnahmen (Skill 03) oder Ursachenanalyse (Skill 05).

## Ausgangslage

Der Agent hat **keinen Zugriff** auf ERP, CAQ-System, DMS oder Labordaten. Er schlägt Aufgaben vor; die Mitarbeitenden beschaffen die Daten. Jede Aufgabe muss so konkret sein, dass eine Person sie ohne Rückfrage ausführen kann.

## Eingaben

- Problembeschreibung (Skill 01) oder Erstmeldung.
- NC-SOP `nordwind-sop-nc.md`, Abschnitt A4.5 (Pflichtfragen) und A5.2.

## Vorgehen

1. Bestimme das betroffene Objekt (Artikel, Charge, Auftrag, Prüfmittel, Prozess, Dokument, Lieferant).
2. Leite aus jeder Pflichtfrage der SOP A4.5 mindestens eine Aufgabe ab, soweit sie für den Fall relevant ist:
   - frühester möglicher Zeitpunkt der Abweichung,
   - letzte nachweislich konforme Ausführung,
   - seitdem bearbeitete Lose, Produkte, Vorgänge,
   - gemeinsame Ursachenquellen (Material, Lieferant, Programm, Prüfmittel, Qualifikation, Prozessparameter),
   - Zuverlässigkeit der Entdeckungsmethode und nachgelagerte Prüfungen,
   - baugleiche oder ähnliche Produkte und Prozesse,
   - Lieferanten-, externe und Kundenbestände.
3. Denke die Rückverfolgung in beide Richtungen: **wo eingeflossen** (Verwendung in Folgeprodukten, Baugruppen, Systemen) und **woher gekommen** (Rohmaterial, Lieferant, Vorstufe).
4. Ordne jeder Aufgabe eine Datenquelle zu: ERP (Bestände, Verwendung, Auftragshistorie), CAQ-System (Prüfaufträge, Prüfmittelverwendung, Mängel), Labor/Prüfung (Nachmessung), DMS (Vorgaben, Revisionen), Personen (Befragung).
5. Ordne eine Rolle zu (NC-Eigner, Fachexperte, NC/CAPA-Spezialist, Lager, Einkauf, Prüfmittelverwaltung).
6. Priorisiere: zuerst Aufgaben, die den Umfang vergrößern könnten oder Produkt außerhalb der Kontrolle betreffen.
7. Nenne die Annahmen, auf denen der Plan beruht.

## Ausgabeformat

**1. Kurzfazit:** Kernfrage der Umfangsbestimmung in einem Satz.

**2. Aufgabenplan**

| Nr. | Aufgabe | Pflichtfrage (SOP A4.5) | Datenquelle | Rolle | Priorität |
| --- | --- | --- | --- | --- | --- |
| 1 | … | … | ERP / CAQ / Labor / DMS / Befragung | … | hoch / mittel |

**3. Rückverfolgung** (kurz): vorwärts (wo eingeflossen) und rückwärts (woher).

**4. Entscheidungen, die nach den Aufgaben anstehen** (z. B. Umfang festlegen, Containment erweitern).

**5. Annahmen und offene Punkte**

## Regeln und Grenzen

- Keine Ergebnisse vorwegnehmen („es sind keine weiteren Chargen betroffen") – nur Aufgaben formulieren.
- Keine Chargen-, Auftrags- oder Prüfmittelnummern erfinden; nur Nummern aus der Meldung verwenden.
- Eine Umfangsbegrenzung braucht eine Begründung mit Nachweis (SOP A4.5, Herausforderung).
- Höchstens 12 Aufgaben; ähnliche Aufgaben zusammenfassen.

## Prüfhinweise für den Menschen

- Deckt der Plan beide Richtungen der Rückverfolgung ab?
- Ist die letzte konforme Ausführung als Aufgabe enthalten?
- Fehlt eine Datenquelle, die im Haus genutzt wird?

## SOP-Bezug

NC-SOP A4.5 (Abweichungsanalyse und Umfangsbestimmung), A5.2 (zu enge Umfangsbestimmung), A5.5 (objektive Nachweise).
