# Junker Queen Protocol v4.0

## Deine Daten bleiben erhalten
v4 verwendet bewusst denselben lokalen Speicher wie v3 (`jqp_v3_db`).

Dadurch bleiben unter derselben GitHub-Pages-Adresse erhalten:
- Meals und Tageswerte
- Schritte
- Reports
- bisherige Woche
- bereits geplante Übungen
- das heutige Workout

Die App überschreibt einen bereits vorhandenen Tag nicht neu.

Trotzdem vor dem Update einmal **Backup** exportieren.

## Neu in v4
- Safe Area oben korrigiert
- weißer Bereich unten behoben
- Wassertracking optional und standardmäßig ausgeblendet
- 90 Sekunden Pause zwischen Übungen
- Timer basiert auf einer echten Endzeit
- Countdown korrigiert sich nach App-Wechsel
- Sound bei den letzten Sekunden und am Timerende
- einseitige Übungen führen links und rechts separat
- Wechselton zwischen linker und rechter Seite
- Protein gilt ab 95 % des Ziels als geschafft
- vergangene Reports über Datum auswählbar und kopierbar
- Versionsanzeige

## GitHub aktualisieren
1. In der bisherigen App zuerst **Backup** drücken.
2. ZIP entpacken.
3. `index.html`, `manifest.json` und `sw.js` in deinem Repository ersetzen.
4. Commit changes.
5. 1–3 Minuten warten.
6. Web-App auf dem iPhone vollständig schließen und neu öffnen.
7. Falls weiterhin v3 erscheint: GitHub-Pages-Seite in Safari neu laden. Notfalls Homescreen-App löschen und erneut hinzufügen.

## iPhone-Hinweise
- Wake Lock wird angefordert, iOS kann den Bildschirm in einzelnen Situationen trotzdem sperren.
- Beim Verlassen der App kann iOS JavaScript pausieren. v4 merkt sich deshalb die genaue Endzeit und zeigt beim Zurückkehren den korrekten Timerstand.
- Töne funktionieren nach dem manuellen Start des Workout-Players.
