# Sparkonto (Web-App)

Ein kleines Taschengeld-Sparkonto für Kinder als installierbare Web-App (PWA).
Gedacht fürs Fire Tablet im Amazon-Kids-Modus, läuft aber in jedem modernen Browser.

- Läuft komplett lokal im Browser – Daten liegen im `localStorage` des Geräts, es gibt keinen Server und keine Cloud.
- Funktioniert nach dem ersten Aufruf auch offline (Service Worker).
- Einstellungen und Buchungen sind durch eine Eltern-PIN geschützt (Standard: `0000` – bitte direkt ändern).

## Benutzen

App-URL im Browser öffnen, dann „Zum Startbildschirm hinzufügen“ bzw. „App installieren“.
Im Amazon-Kids-Modus: im Eltern-Dashboard die URL als erlaubte Website freigeben.

## Hosting

Statische Dateien, veröffentlicht über GitHub Pages (Branch `main`, Ordner `/`).
Nach Änderungen die Cache-Version in `sw.js` hochzählen.

## Lokal testen

```bash
python3 -m http.server 8000
```

Dann http://localhost:8000 öffnen.
