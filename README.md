# Freitag Gym Tracker – PWA

Diese Version kann auf Android/iPhone wie eine App installiert und danach auch offline verwendet werden.

## Dateien
- `index.html` – die App
- `manifest.webmanifest` – App-Metadaten
- `sw.js` – Offline-/Cache-Funktion
- `icons/` – App-Icons

## Installation / Hosting

Eine PWA benötigt HTTPS. Am einfachsten:

### GitHub Pages
1. Neues GitHub-Repository anlegen.
2. Den Inhalt dieses ZIPs in das Repository hochladen.
3. Unter `Settings → Pages` als Quelle den `main`-Branch auswählen.
4. Die danach angezeigte HTTPS-Adresse am Smartphone öffnen.
5. In Chrome/Samsung Internet: `App installieren` bzw. `Zum Startbildschirm hinzufügen`.

Alternativ funktioniert jeder andere statische HTTPS-Webspace.

## Nutzung
- Der Trainingstag ist automatisch auf Freitag ausgerichtet.
- Nach `Training abschließen` wird die Einheit lokal gespeichert.
- Der Verlauf und die Progression bleiben auf dem jeweiligen Gerät erhalten.
- `Chat-Export` erzeugt einen kompakten Text zum Einfügen in ChatGPT.
- Die Daten werden nicht an einen Server übertragen.

## Wichtig
Die Trainingsdaten liegen im lokalen Browser-/App-Speicher des jeweiligen Geräts.
Bei Löschen der Websitedaten oder Wechsel auf eine andere Domain gehen diese lokalen Daten verloren.


## Backup / Import

Im Bereich `Verlauf` gibt es zwei Funktionen:

- **Backup exportieren**: erstellt eine JSON-Datei mit dem vollständigen lokalen App-Stand.
- **Backup importieren**: stellt diesen Stand auf demselben oder einem anderen Gerät wieder her.

Das Backup umfasst:
- Trainingshistorie
- aktuelle Trainingsgewichte und Progression
- nächsten Freitag
- noch nicht abgeschlossene Eingaben und Notizen

Beim Import wird der aktuelle lokale App-Stand nach einer Sicherheitsabfrage vollständig ersetzt.

Empfehlung: Nach einigen Trainingseinheiten oder vor einem Handywechsel ein Backup exportieren und z. B. in der persönlichen Cloud speichern.
