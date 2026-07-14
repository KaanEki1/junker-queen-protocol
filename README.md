# Junker Queen Protocol 6.1

Eine installierbare, lokale Fitness-Web-App (PWA) mit Premium-Mobile-UI.

## Enthalten

- Tagesdashboard für Kalorien, Protein, Schritte und Workout-Fortschritt
- Daily Coach und Step-Missionen
- vollständiger Workout-Player mit Timer, Satztracking, Pausen, Sound und Haptik
- Kalender mit nachträglicher Tagesbearbeitung
- monatliches Ranked-/Season-XP-System mit Pokalvitrine
- Mahlzeiten- und Rezepttracking
- Tagesreports, Backup-Export und Backup-Import
- Daily Check-in für Gewicht, Energie, Hunger, Wasser und Notizen
- Offline-Unterstützung via Service Worker
- lokale Datenspeicherung im Browser; keine externe Datenübertragung

## Start

Die Dateien müssen über einen lokalen oder normalen Webserver ausgeliefert werden. Ein direktes Öffnen per `file://` unterstützt Service Worker nicht zuverlässig.

Beispiel:

```bash
python3 -m http.server 8080
```

Danach `http://localhost:8080` öffnen.

## Dateien

- `index.html` – komplette App, UI und Logik
- `manifest.json` – PWA-Konfiguration
- `sw.js` – Offline-Cache

## Daten

Alle Nutzerdaten liegen in `localStorage` unter `jqp_v3_db`, damit vorhandene Daten aus älteren Versionen erhalten bleiben.


## Neu in 6.1
- Momentum-Bar mit Daily XP und Streak
- Sofortige XP-Floats bei Aktionen
- Celebration-Popups und Confetti für große Ziele
- Goal-Hit-States für Dashboard-Karten
- Animierte Step-Missionen und abgeschlossene Übungen
- Reduced-Motion-Unterstützung bleibt erhalten
