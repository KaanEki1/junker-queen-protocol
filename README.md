# Junker Queen Protocol 6.2

Eine installierbare, vollständig lokale Fitness-Web-App (PWA) mit Premium-Mobile-UI, fairem XP-System und Offline-Unterstützung.

## Neu in 6.2

### Faire Streaks

- Ein Tag zählt erst ab **50 Daily XP** zur Streak.
- Anzeige von aktuellem Streak, längstem Streak und heutigem Status.
- Die App zeigt exakt, wie viele XP heute noch zur Streak-Sicherung fehlen.

### Ehrliche Daily- und Season-XP

Die maximalen 120 Daily XP bestehen aus:

- Workout: 35 XP
- Protein: 25 XP
- Kalorien: 20 XP
- Schritte: 30 XP
- Report: 10 XP

Workout-XP werden als ganze Zahlen auf die normalen Hauptübungen verteilt. Die letzte Übung erhält den Rundungsrest, sodass die Summe immer exakt 35 XP beträgt. Warm-up, Cooldown und Extra-Übungen geben keine normalen Season-XP. Schritt-XP werden anteilig und ganzzahlig vergeben. Jeder sichtbare XP-Float entspricht echten Daily- und Season-XP.

### Reward Queue

Mehrere gleichzeitig erreichte Erfolge werden vollständig nacheinander angezeigt. Daily-Meilensteine erscheinen zuerst, Hauptziele danach und ein Rank-up zuletzt.

### Rezeptverwaltung

- Erstellen und bearbeiten
- endgültig löschen mit Sicherheitsabfrage
- duplizieren
- Favoriten markieren
- suchen
- sortieren nach letzter Verwendung, Bewertung, Protein, Kalorien oder Name
- Hall-of-Fame-Rezepte können ebenfalls gelöscht werden
- das Löschen eines Rezepts verändert keine bereits gespeicherten Meals

### Premium-UX

- hochwertigerer, kompakterer Header
- täglicher Fokus direkt sichtbar
- transparente, aufklappbare Daily-XP-Aufschlüsselung
- Dashboard-Zustände: offen, fast erreicht, erreicht und überschritten
- überarbeitete Step-Missionen
- echter Workout-Gesamtfortschritt
- verbesserte Satz- und Seitenwechsel-Anzeige
- hochwertigerer Ranked-Screen mit Resttagen, benötigten Daily XP und bestem Rang
- konsistente Sounds und Haptics
- ruhige Animationen und Unterstützung für `prefers-reduced-motion`

## Daten und Migration

Alle Nutzerdaten bleiben unter dem bestehenden Local-Storage-Key `jqp_v3_db` erhalten. Version 6.2 ergänzt fehlende Felder fehlertolerant und löscht keine vorhandenen Tages-, Meal-, Workout-, Report-, Rezept- oder Pokaldaten.

## Start

Die Dateien müssen über einen lokalen oder normalen Webserver ausgeliefert werden. Ein direktes Öffnen per `file://` unterstützt Service Worker nicht zuverlässig.

Beispiel:

```bash
python3 -m http.server 8080
```

Danach `http://localhost:8080` öffnen.

## GitHub Pages

Alle vier Dateien gemeinsam in das bestehende GitHub-Pages-Verzeichnis hochladen:

- `index.html`
- `manifest.json`
- `sw.js`
- `README.md`

Der Service Worker verwendet einen neuen Cache-Namen und entfernt bei der Aktivierung ältere Caches. Der App-Identifier bleibt unverändert, damit eine bestehende Installation updatefähig bleibt.

## Datenschutz

Die App verwendet keine externen Frameworks, CDNs oder Server. Alle Daten bleiben lokal im Browser, sofern der Nutzer nicht selbst ein Backup exportiert.
