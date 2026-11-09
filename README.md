# Squash T-Party

Übungs-App für Squash: Drills für solo, zu zweit oder zu dritt mit animierter Court-Draufsicht, dazu Aufwärmen, Dehnen und Kraft.

- **Webseite:** https://squash-t-party.de
- **Besucherstatistik (GoatCounter):** https://squash-t-party.goatcounter.com
- **Kontakt:** pascal.haaf@gmx.de

## Aufbau

- `index.html` – die komplette App in einer Datei (HTML, CSS, JavaScript, eingebettete Schriften)
- `manifest.webmanifest`, `sw.js`, `icons/` – App-Modus: Installation auf dem Homescreen, Vollbild ohne Browserleiste, Offline-Start
- `CNAME` – eigene Domain für GitHub Pages, nicht löschen
- `.nojekyll` – GitHub Pages veröffentlicht die Dateien unverändert
- `fonts/` – Lizenzen der eingebetteten Schriften (SIL Open Font License)

## Hinweise

- Als App installieren: Android/Chrome → Menü → „App installieren“ bzw. „Zum Startbildschirm hinzufügen“. iPhone/Safari → Teilen → „Zum Home-Bildschirm“.
- Der Service Worker lädt immer zuerst die neueste Version aus dem Netz und nutzt die gespeicherte Kopie nur ohne Verbindung. Bei größeren Umbauten in `sw.js` den Cache-Namen hochzählen (`t-party-v1` → `v2`).

- Der GoatCounter-Zähler steht ganz unten in `index.html`. Bei Updates muss er drin bleiben, sonst werden keine Besuche gezählt. Die bisherigen Zahlen bleiben bei GoatCounter gespeichert.
- Geöffnete Übungen werden zusätzlich als `/uebung/<name>` gezählt.
- Favoriten und Hell/Dunkel-Wahl speichert jeder Browser lokal, sie hängen an der Adresse squash-t-party.de.
