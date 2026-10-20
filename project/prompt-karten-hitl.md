# Prompt-Karten Lab 1.3 – Prompten mit Mensch in the loop

Karten für die Übung in Lab 1.3. Eingabe ist die Erstmeldung **NC-01** ([`faelle/nc-01-pruefmittel-part1-eingang.docx`](faelle/nc-01-pruefmittel-part1-eingang.docx)). Die NC-SOP [`sop/nordwind-sop-nc.md`](sop/nordwind-sop-nc.md) wird an den Chat angehängt. Eckige Klammern `[…]` werden vor dem Absenden ersetzt.

## Karte A – Zero-Shot

Nur Anweisung, kein Beispiel.

```text
Du bist QS-Mitarbeitende bei Nordwind Medical und arbeitest nach der angehängten NC-SOP.
Aufgabe: Erstelle aus der Erstmeldung [NC-Meldung einfügen oder Datei anhängen] eine Problembeschreibung nach NC-SOP Abschnitt A4.4.
Regeln:
- Nutze nur Angaben aus der Meldung und der NC-SOP. Ergänze nichts.
- Fehlende Angaben schreibst du als „fehlt".
- Trenne Fakten, Annahmen und offene Punkte.
- Keine Ursache, keine Schuldzuweisung.
Format: Tabelle mit den Feldern Soll, Ist, Differenz, Ort, Zeit, Objekt, Umfang, Entdeckung, Historie; je Feld eine Spalte „Quelle".
```

## Karte B – Few-Shot

Gleiche Anweisung wie Karte A, ergänzt um ein Beispiel einer guten Problembeschreibung (NC-02). Die Karte-A-Anweisung vor das Beispiel setzen, den Satz am Ende anhängen.

```text
[Anweisung aus Karte A]

Beispiel für eine gute Problembeschreibung (anderer Fall, nur als Muster für Aufbau und Genauigkeit):

| Feld | Inhalt | Quelle |
| --- | --- | --- |
| Soll | 200 Stück laut Fertigungsauftrag FA-EX-2055 | Meldung |
| Ist | 201 Stück laut Ausführungsprotokoll des Dienstleisters | Meldung |
| Differenz | 1 Stück Mehrmenge | Meldung |
| Ort | AG 190 „Wareneingangsprüfung Standort A Dienstleister B" | Meldung |
| Zeit | Auftreten 2024-10-10, Kenntnisnahme 2024-09-19 (Widerspruch: Kenntnisnahme liegt vor dem Auftreten, als offene Frage markiert) | Meldung |
| Objekt | FA-EX-2055, Prüfauftrag PA-EX-10000; Artikel und Charge: fehlt | Meldung |
| Umfang | 201 Stück bestätigt; weitere Lose: fehlt | Meldung |
| Entdeckung | AG 190; in AG 150 wurde die Abweichung nicht erkannt | Meldung |
| Historie | nicht in der Meldung | – |

Offene Punkte: (1) Welches Datum ist richtig, Auftreten oder Kenntnisnahme? (2) Artikel und Charge nennen. (3) Welche weiteren Lose des Dienstleisters sind betroffen?

Erstelle die Problembeschreibung für die neue Meldung im selben Aufbau.
```

## Feedback-Prompts

Nach der Prüfung mit den fünf Prüfpunkten im selben Chat zurückgeben. Je Fehler ein gezielter Satz.

| Fehlerbild | Feedback-Prompt |
| --- | --- |
| Zahl, Datum oder Nummer steht nicht in der Meldung | „In Zeile [Feld] steht [Wert]. Das steht nicht in der Meldung. Streiche den Wert und schreibe ‚fehlt'. Prüfe danach alle übrigen Zahlen gegen die Meldung." |
| Ursache oder Schuldzuweisung | „Der Satz [Zitat] enthält eine Ursache. Formuliere ihn als Beobachtung ohne Ursache und ohne Personenbezug." |
| Widerspruch geglättet oder Lücke nicht benannt | „Die Meldung enthält [Widerspruch/Lücke]. Benenne sie im Feld [Feld] und stelle sie als offene Frage an den NC-Eigner." |

## Die fünf Prüfpunkte

| Nr. | Prüfpunkt | Prüffrage |
| --- | --- | --- |
| 1 | Quelle | Steht jede Aussage in Meldung oder NC-SOP? |
| 2 | Nichts erfunden | Stimmen Zahlen, Daten und Namen wörtlich mit der Meldung überein? |
| 3 | Getrennt | Sind Fakten, Annahmen und offene Punkte unterscheidbar? |
| 4 | Ursachenneutral | Enthält die Problembeschreibung keine Ursache und keinen Personenbezug? |
| 5 | Vollständig | Sind Soll, Ist, Ort, Zeit, Objekt und Umfang benannt oder als „fehlt" markiert? |

## Ergebnis sichern

Der beste Prompt (Zero-Shot oder Few-Shot, nach Feedback) wird als Eintrag 1 in [`nc-capa-prompt-bibliothek.md`](nc-capa-prompt-bibliothek.md) eingetragen. Die fünf Prüfpunkte bilden den Kern der Prüfcheckliste, die in Lab 3.2 und Lab 4.1 wiederverwendet wird.
