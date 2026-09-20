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


## Gemeinsame Nutzung / Ersteinrichtung

Beim ersten Start öffnet die App automatisch eine kurze Ersteinrichtung.
Dort kann jede Person eigene Startgewichte für die Arbeitsätze festlegen.
Diese Werte werden lokal auf dem jeweiligen Gerät gespeichert.

Später können die Startgewichte jederzeit in der App unter:
`Verlauf → Startgewichte bearbeiten`
angepasst werden.


## Finaler Freitag-Plan (18 Sätze)

1. Beinpresse: 1 Aufwärmsatz + 2 Arbeitssätze (8–12)
2. Bankdrücken: 2 Aufwärmsätze + 2 Arbeitssätze (6–10)
3. Latzug: 1 Aufwärmsatz + 2 Arbeitssätze (8–12)
4. Kabelrudern: 2 Arbeitssätze (8–12), kein eigener Aufwärmsatz
5. Beinbeuger: 2 Arbeitssätze (10–15), kein eigener Aufwärmsatz
6. Seitheben: 2 Arbeitssätze (12–20)
7. Schräge Sit-ups: 2 Arbeitssätze (10–15 je Seite)

Seitheben und schräge Sit-ups können als Supersatz ausgeführt werden.


## Finales UI-Update

- Notizfelder aus dem Training entfernt.
- Chat-Export enthält nur Trainingswerte und Progressionshinweise.
- Cache-Strategie aktualisiert, damit neue App-Versionen zuverlässig geladen werden.


## Version 2 (18.09.2026 16:37)

- Belohnungssystem: Freitag-Streak, Monatsfortschritt, 12-Wochen-Konstanz und 4er-Meilensteine.
- Beinpresse: Maschinenstufen 21–213 kg in 8-kg-Schritten; aktuelles Arbeitsgewicht 101 kg.
- Beinbeuger: Knie 10, Knöchel 4.
- Sätze können in der laufenden Einheit mit − entfernt und mit + Satz ergänzt werden.
- Satzänderungen gelten nur für die aktuelle Einheit.
- Kopfzeile v.2, Beschreibungstext entfernt, keine Notizfelder.


## Version 2.1 (20.09.2026 09:34)

- Reihenfolge: Beinpresse → Beinbeuger → Bankdrücken → Latzug → Kabelrudern → Seitheben → schräge Sit-ups.
- Freitag bleibt der Ankertag.
- Gültiges Wochenfenster: Donnerstag 00:00 bis Sonntag 24:00.
- Donnerstag zählt als vorgezogen; Samstag/Sonntag als Nachholen.
- Die Serie bleibt bis Sonntag offen und geht erst nach verpasstem Nachholfenster verloren.
- Pro Freitagsslot zählt höchstens eine Einheit.
- Verlauf speichert tatsächliches Trainingsdatum und den zugehörigen Freitag.
- Profil zeigt passende Hinweise für Vorziehen, regulären Freitag und Nachholen.
