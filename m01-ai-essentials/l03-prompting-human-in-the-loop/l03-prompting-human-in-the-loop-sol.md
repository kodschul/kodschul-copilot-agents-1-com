# Lab 1.3 – Lösung: Prompten mit Mensch in the loop

Copilot formuliert bei jedem Lauf anders. Die Lösung zeigt deshalb das Ergebnis, auf das die Prüfung zielt, nicht den Wortlaut einer Copilot-Antwort.

## Aufgabe 1 bis 3: Entwürfe erzeugen

Zero-Shot (Karte A) und Few-Shot (Karte B) liefern zwei Entwürfe derselben Meldung. Der Unterschied liegt in Aufbau und Detailtiefe: Few-Shot folgt dem Muster NC-02 (Tabelle mit Quelle je Feld, Widerspruch als offene Frage markiert). Entscheidend sind nicht die Formulierungen, sondern die fünf Prüfpunkte.

## Aufgabe 4: Prüfpunkte an NC-01

Was jeder Prüfpunkt an dieser Meldung zu prüfen hat:

| Nr. | Prüfpunkt | Prüfung an NC-01 |
| --- | --- | --- |
| 1 | Quelle | Jede Angabe stammt aus der Meldung oder der NC-SOP. Angaben über Ursachen, Prüfintervalle einzelner Prüfmittel oder Lagerprozesse stehen nicht in der Meldung. |
| 2 | Nichts erfunden | Wörtlich: 78 Prüfmittel, Standort A, 2025-10-09 (Auftreten und Kenntnisnahme), Sofortmaßnahme am 2025-10-10, Status „Schwund virtuell". Prüfmittelnummern, Typen und Abteilungen stehen nicht in der Meldung. |
| 3 | Getrennt | „Es besteht das Risiko, dass sich die Prüfmittel im Umlauf befinden und das Prüfintervall überschritten ist" ist eine Annahme, keine bestätigte Tatsache. |
| 4 | Ursachenneutral | Die Meldung nennt keine Ursache. „Schwund" bezeichnet den Buchungsstatus, keine Ursache. |
| 5 | Vollständig | Soll (verbindliche Anforderung mit Dokument) und Historie sind in der Meldung nicht genannt und werden als „fehlt" ausgewiesen. |

## Aufgabe 5: Feedback

Passende Feedback-Prompts aus der Karte, angewandt auf typische Funde:

| Fund im Entwurf | Feedback-Prompt (Auszug) |
| --- | --- |
| Entwurf nennt Prüfmittelnummern, die in der Meldung fehlen | „In Zeile Objekt steht [Wert]. Das steht nicht in der Meldung. Streiche den Wert und schreibe ‚fehlt'. Prüfe danach alle übrigen Zahlen gegen die Meldung." |
| Entwurf schreibt „wegen unzureichender Lagerorganisation" | „Der Satz [Zitat] enthält eine Ursache. Formuliere ihn als Beobachtung ohne Ursache und ohne Personenbezug." |
| Entwurf behauptet, das Prüfintervall sei überschritten | „Die Meldung enthält nur das Risiko eines überschrittenen Prüfintervalls. Benenne es im Feld Umfang als Annahme und stelle es als offene Frage an den NC-Eigner." |

## Aufgabe 6: Musterergebnis und Bibliothekseintrag

**Problembeschreibung NC-01**

| Feld | Inhalt | Quelle |
| --- | --- | --- |
| Soll | Prüfmittel sind am Lagerplatz auffindbar; verbindliche Anforderung (Dokument, Revision): fehlt | Meldung / fehlt |
| Ist | Bei der Bestandsaufnahme des Prüfmittellagers am Standort A waren 78 Prüfmittel nicht an ihrem Lagerplatz | Meldung |
| Differenz | 78 Prüfmittel am Lagerplatz nicht auffindbar, Verbleib unbekannt | Meldung |
| Ort | Prüfmittellager Standort A; betroffen kann jede Abteilung sein | Meldung |
| Zeit | Auftreten 2025-10-09, Kenntnisnahme 2025-10-09 | Meldung |
| Objekt | 78 Prüfmittel (Nummern und Typen: fehlt) | Meldung |
| Umfang | 78 nicht am Lagerplatz bestätigt; Prüfmittel im Umlauf mit überschrittenem Prüfintervall: Risiko, nicht bestätigt (Annahme) | Meldung |
| Entdeckung | Bestandsaufnahme des Prüfmittellagers | Meldung |
| Historie | fehlt | – |

**Isolation und Sofortmaßnahme laut Meldung:** keine Isolation; am 2025-10-10 wurden alle nicht auffindbaren Prüfmittel auf den Status „Schwund virtuell" gebucht (Statusbuchung).

**Vorläufige NC-Einordnung (Vorschlag):** nicht abschließend, weil keine konkrete Anforderung benannt ist (NC-SOP C4). Entscheidung beim NC-Eigner.

**Offene Punkte:**

1. Welches Dokument legt die Anforderung fest (Lagerplatz, Prüfintervall)?
2. Prüfmittelnummern und Kalibrierstatus der 78 Prüfmittel?
3. Wurden die Prüfmittel in Prüfaufträgen verwendet, und wann zuletzt?
4. Verhindert die Statusbuchung „Schwund virtuell" die weitere Verwendung?
5. Gibt es einen Quellvorgang oder ähnliche Ereignisse?

**Prompt-Bibliothek, Eintrag 1**

| Feld | Inhalt |
| --- | --- |
| SOP-Bezug | NC-SOP A4.4 |
| Prompt | Karte B (Few-Shot) mit Musterbeschreibung NC-02, ergänzt um die Rückfragen aus dem Feedback |
| Benötigte Dateien | `sop/nordwind-sop-nc.md`, Meldung als `.docx` |
| Getestet mit | NC-01 |
| Prüfhinweise | fünf Prüfpunkte; besonders Prüfpunkt 2 (Nummern) und 5 („fehlt" statt Ergänzung) |
| Wird zu Skill | Skill 01 (Erstbewertung) |
