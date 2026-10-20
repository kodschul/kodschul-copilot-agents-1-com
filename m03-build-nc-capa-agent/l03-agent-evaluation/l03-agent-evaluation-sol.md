# Lab 3.3 – Lösung: Agentenprüfung

Die Antwort des Agenten ist bei jedem Lauf anders. Die Lösung zeigt, welche Kernschritte aus Part 1 allein ableitbar sind und wie die sechs Kriterien bewertet werden.

## Aufgabe 1 bis 3: Lauf und Sicherung

Nur die Eingangsdatei des Falls wird an den Agenten gegeben. Der Agent nennt in der ersten Zeile die genutzten Skills; sie gehören in den Bewertungsbogen.

## Aufgabe 4: Abgleich mit den Kernschritten

Spalte „Erwartbar": **ja** = Tätigkeit als Aufgabe oder Vorschlag aus Part 1 ableitbar, **Frage** = nur als offene Frage ableitbar, **nein** = Ergebnis, das erst das Team ermittelt. „ja" und „Frage" zählen als Treffer, „nein" fließt nicht in K2 ein.

### NC-01 Prüfmittel

| Nr. | Kernschritt | Erwartbar | Hinweis |
| --- | --- | --- | --- |
| 1 | Ursprung früherer CAPA | Frage | Historie und Quellvorgang erfragen |
| 2 | Meldebogen berichtigen | nein | Fehler im Meldebogen aus Part 1 nicht erkennbar |
| 3 | Abteilungen kontrollieren Bereiche | ja | „Es kann jede Abteilung betroffen sein" |
| 4 | Kontrolle: nichts außerhalb der Kontrolle | Frage | Pflichtfrage NC A4.6 |
| 5 | Priorität P2 | ja | als Vorschlag, nicht abschließend ohne Anforderung (C4) |
| 6 | Erweiterte Analyse, Worst Case | ja | Aufgaben: Verwendung in Prüfaufträgen, Kalibrierstatus |
| 7 | Wiederaufgetauchte Prüfmittel kalibrieren | nein | Ergebnis der Suche |
| 8 | Containment: keine weiteren Maßnahmen | nein | Ergebnis der Analyse; der Agent schlägt Containment vor |
| 9 | Risikobetrachtung dynamisch | nein | Ergebnis; als Aufgabe „Nutzungsdaten auswerten" ableitbar |
| 10 | Dokumentation prüfen | ja | Skill 06, Qualitätsgate |

### NC-02 Stückzahl

| Nr. | Kernschritt | Erwartbar | Hinweis |
| --- | --- | --- | --- |
| 1 | Fehlerbild laufender CAPA zuordnen | Frage | „Bestehende CAPA passend?" (Skill 05) |
| 2 | Abweichungsanalyse Soll 200 / Ist 201 | ja | Mengenabgleich der Arbeitsgänge |
| 3 | Materialverwendung klären | ja | Verbleib und Status |
| 4 | Korrektur: Charge verschrotten | Frage | nur als Ausblick mit Genehmigungsbedarf |
| 5 | Weitere Produkte an CAPA übergeben | Frage | CAPA-Eskalation |
| 6 | Priorität P2 | ja | als Vorschlag |
| 7 | Sensibilisierung durchführen | nein | ohne nachgewiesenes Wissensdefizit nicht als Maßnahme zu akzeptieren |
| 8 | Verschrottung nachweisen | Frage | Nachweis als Abschlusspunkt |
| 9 | Risikobewertung: nicht außerhalb der Kontrolle | ja | Skill 04 |
| 10 | Dokumentation prüfen, schließen | ja | Skill 06 |

### NC-03 Druckmessdosen

| Nr. | Kernschritt | Erwartbar | Hinweis |
| --- | --- | --- | --- |
| 1 | Berstdrücke gegen Spezifikation | Frage | Spezifikation fehlt in Part 1, zweites Ereignis nicht erkennbar |
| 2 | Rückverfolgung wo eingeflossen | ja | Verwendungsnachweis im ERP |
| 3 | Chargen sperren | Frage | Part 1 nennt die Sperre; Agent bewertet sie für den potenziellen Umfang |
| 4 | Verwendung der Chargen prüfen | ja | Aufgabe |
| 5 | Umfang erweitern | ja | als Aufgabe „weitere Chargen prüfen"; neue Charge nicht erkennbar |
| 6 | Risikobewertung je Charge (AQL) | Frage | Auswertung der Prüfdaten als Aufgabe |
| 7 | Priorität P2 | ja | Worst Case für Anwender als Hypothese |
| 8 | Containment-Vorgehen prüfen | ja | Skill 03 |
| 9 | Korrektur: Sonderfreigabe | Frage | als Ausblick mit Genehmigungsbedarf |
| 10 | Ursachenanalyse an CAPA übergeben | Frage | Wiederholung in 12 Monaten erfragen |
| 11 | Dokumentation prüfen | ja | Skill 06 |

## Aufgabe 5: Punktevergabe je Kriterium

Punkte: 2 = erfüllt, 1 = teilweise, 0 = fehlt. Maximal 12.

| Kriterium | 2 Punkte | 1 Punkt | 0 Punkte |
| --- | --- | --- | --- |
| K1 Vollständigkeit | Aufgaben und Fragen zu Isolation (A4.2), Umfang (A4.5) und Risiko/Priorität (A4.6) | ein Bereich fehlt | mehrere Bereiche fehlen |
| K2 Treffer | Richtwert: mindestens drei Viertel der Schritte mit „ja" oder „Frage" vorgeschlagen | Richtwert: mindestens die Hälfte | weniger |
| K3 Datenqualität | nichts erfunden; Widerspruch oder Lücke benannt (NC-02: Kenntnisnahme vor Auftreten; NC-03: Spezifikation fehlt; NC-01: Anforderung fehlt) | eines davon | erfundene Nummer oder Widerspruch geglättet |
| K4 Maßnahmen | Isolation, Containment, Korrektur und CAPA-Maßnahme getrennt | eine Verwechslung | Containment durchgehend als Korrektur |
| K5 Priorität | Vorschlag mit Begründung nach SOP-Logik | Vorschlag ohne Begründung | als feststehend formuliert |
| K6 Grenzen | Daten, Ursache und Freigabe beim Menschen; kein Systemzugriff behauptet | einzelne Grenzverletzung | entscheidet oder behauptet eine Prüfung |

## Aufgabe 6: Schwächste Punkte

Die zwei Kriterien mit der niedrigsten Punktzahl markieren und die Fundstelle notieren. Bei Gleichstand zählt das Kriterium mit dem größeren Qualitätsrisiko (K3, K4, K6 vor K1, K2, K5). Die Zuordnung zu Skill oder Anweisungen erfolgt in Lab 4.1.
