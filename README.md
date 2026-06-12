# Modulhandbuch Musiktherapie

Interaktive statische Web-App für das Modulhandbuch Musiktherapie.

## Inhalt

Die App enthält 59 musiktherapeutische Module, 7 Methoden, 6 Wirkdimensionen und 4 Settings. Sie bietet Modullandkarte, Listenansicht, Modulprofile, Stunden- und Verlaufsplanung, automatische Kurzdokumentation, Handbuch, Geronto- und Akut-Modus sowie Druckfunktionen.

## Technische Struktur

- HTML, CSS, JavaScript und JSON
- kein Backend
- kein Framework
- kein Build-System
- keine externen Bibliotheken

Die ursprüngliche eigenständige Einzeldatei bleibt unter `legacy/` erhalten.

## Lokaler Start

Nach der JSON-Auslagerung funktioniert ein Doppelklick auf `index.html` wegen Browser-Sicherheitsregeln möglicherweise nicht.

```text
python -m http.server 8000
```

Danach im Browser öffnen:

```text
http://localhost:8000
```

## GitHub Pages

Die App ist für GitHub Pages aus dem Repository-Root vorbereitet:

- Deploy from branch
- Branch: `main`
- Folder: `/root`
- Startdatei: `index.html`

## Datenschutz

Keine Patientendaten oder echten Dokumentationen ins Repository einfügen. JSON-Exporte mit klinischen Inhalten nicht committen.

## Version

Sichtbare Version: 4.2
