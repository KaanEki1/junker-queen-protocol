# Junker Queen Protocol v5.0

## Wichtig vor dem Update
1. In der alten App **Backup exportieren**.
2. Das bestehende Homescreen-Icon **nicht löschen**.
3. `index.html`, `manifest.json` und `sw.js` auf GitHub ersetzen.
4. Committen, einige Minuten warten und die bestehende App neu öffnen.
5. Unter **HQ → Settings** gibt es jetzt auch **Backup importieren**.

v5 nutzt weiterhin den lokalen Speicher-Key `jqp_v3_db`, damit vorhandene Daten unter derselben GitHub-Pages-Adresse erhalten bleiben.

## Neu
- Monatskalender mit Navigation über Jahre
- Vergangene und zukünftige Tage antippen und bearbeiten
- Alte Meals ergänzen/löschen
- Alte Steps, Ziele, Notizen und Workouts bearbeiten
- Rezeptbibliothek
- Rezepte mit Zutaten, Gramm, kcal/100 g und Protein/100 g bearbeiten
- Beim Kochen Mengen für heute verändern und Makros automatisch neu berechnen
- Hall-of-Fame-Rezepte vorinstalliert
- Backup-Import und -Export
- Monatliche Ranked-Seasons
- Bronze, Silber, Gold, Platin, Diamant, Master, Grandmaster, Champion, JK
- Saison-XP aus Workout, Protein, Kalorien, Steps und Report
- leichte Inaktivitätsstrafe innerhalb einer gestarteten Season
- Pokalvitrine für abgeschlossene Monate
- alte Reports auswählen und kopieren
- Uhrzeiten für erste/letzte Mahlzeit sowie Workout Start/Ende
- Warm-up und Cooldown führen einseitige Übungen links/rechts getrennt
- Protein- und Dezimalanzeigen sauber gerundet

## Ranked-Balance
Maximal sind etwa 120 XP pro perfekten Tag möglich.
JK erfordert praktisch einen außergewöhnlich konstanten Monat. Die mittleren Ränge sind erreichbar, aber nicht geschenkt.


## v5.1 Hotfix
- „Heute“ verwendet jetzt immer das Datum in Europe/Vienna.
- Unvollständige migrierte Tagesdaten reparieren ihre Ziele automatisch.
- Verhindert 0/0 bei Kalorien, Protein und Steps, obwohl der Kalendertag Daten enthält.


## v5.2 UI & Game Feel
- Fußzeile auf Heute, Training und Essen reduziert.
- Schwebendes Plus-Menü für Kalender, Ranked, Rezepte, Reports und Settings.
- Aktueller Season-Rang inklusive XP permanent im Header.
- Neun eigenständige, animierte Ranked-Embleme im einheitlichen JQP-Stil.
- Glücklicherer Pause-Ende-Sound als aufsteigender Major-Arpeggio-Jingle.
- Haptisches Feedback, sofern vom Gerät/Browser unterstützt.
- Visuelle Button-, Navigation-, Sheet- und Rank-Animationen.
- Hall-of-Fame-Rezeptfehler behoben; Standardrezepte werden wieder angezeigt.
