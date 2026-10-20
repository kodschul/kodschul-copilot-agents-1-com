# FAQ

**Kann der Agent auf ERP, CAQ-System oder DMS zugreifen?**
Nein. Der Agent arbeitet nur mit dem, was im Chat steht und im Wissen liegt. Er schlägt Aufgaben vor, die das Team in den Systemen erledigt.

**Wer entscheidet, ob eine Abweichung eine NC ist oder welche Priorität gilt?**
Das QS-Team. Der Agent liefert einen Vorschlag mit Begründung, markiert als „Vorschlag, Entscheidung NC-Eigner".

**Warum klingt eine erfundene Antwort genauso sicher wie eine richtige?**
Ein Sprachmodell erzeugt immer flüssigen Text. Der Ton sagt nichts über Richtigkeit; Quelle und Prüfpunkte schaffen Verlässlichkeit.

**Was ist der Unterschied zwischen Instruktion, Wissen und Skill?**
Die Instruktion legt Rolle, Ablauf und Grenzen fest. Wissen sind Dokumente zum Nachschlagen (SOPs). Ein Skill beschreibt eine wiederkehrende Aufgabe mit festem Ausgabeformat und liegt als Datei im Wissen.

**Warum höchstens sechs Skills?**
Jeder Skill muss getestet und gepflegt werden. Sechs Skills decken die SOP-Schritte ab, ohne dass sich Skills überschneiden.

**Was tun, wenn der Agent einen Fehler macht?**
Betrifft er eine Aufgabe, die Skill-Datei ändern, neu hochladen und die Version hochzählen. Betrifft er alle Antworten, die Anweisungen ändern. Danach denselben Fall erneut laufen lassen.

**Warum wird nur Part 1 an den Agenten gegeben?**
Eine echte Erstmeldung enthält nur den Eingang. Die reale Bearbeitung ist die Vergleichsgrundlage und wird erst nach dem Lauf geöffnet.

**Dürfen echte Fälle in den Chat?**
Für den Kurs nur die anonymisierten Fälle. Im Arbeitsalltag gelten die Datenregeln des Unternehmens: keine Patientendaten, keine personenbezogenen Daten.

**Was ist, wenn Agent Builder im eigenen Tenant nicht freigegeben ist?**
Als Fallback die Anweisungen als ersten Prompt in einen neuen Copilot-Chat-Verlauf einfügen und SOPs sowie die passende Skill-Datei anhängen. Das Ergebnis ist inhaltlich gleich, aber nicht teilbar und ohne gespeicherte Konfiguration.

**Wer pflegt den Agenten nach dem Kurs?**
Eine benannte Person (Owner). Der Pflegeplan aus Lab 5.1 legt Review-Turnus, Testfälle und Abschaltkriterium fest.

**Was passiert bei einer SOP-Änderung?**
Die SOP im Wissen ersetzen, betroffene Skills anpassen und die drei Testfälle als Regressionstest erneut laufen lassen.
