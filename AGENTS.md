# AGENTS.md

Dieses Projekt ist eine statische Web-App für das Modulhandbuch Musiktherapie.

## Ziel

Die App muss ohne Backend auf GitHub Pages laufen.
Keine Frameworks.
Kein Build-System.
Keine externen Bibliotheken ohne ausdrückliche Freigabe.

## Grundregel

Refactoring darf die bestehende Funktionalität nicht verändern.

## Fachliche Regeln

- Fachliche Inhalte dürfen nicht gekürzt, vereinfacht oder frei umgeschrieben werden.
- Interne Kürzel wie W1, W2, KM-1, RN-2 usw. dürfen in Planung, Modullandkarte, Modulprofilen und technischer Verwaltung sichtbar bleiben.
- In der automatischen Kurzdokumentation dürfen keine internen Kürzel und keine Abschnittsdauern erscheinen.
- Die Planung darf Dauerangaben enthalten.
- Die automatische Dokumentation soll klinisch lesbar sein und ohne technische Planungslogik funktionieren.
- Versionierung bleibt sichtbar bei 4.2, bis sie ausdrücklich geändert wird.
- Geronto-Modus und Akut-Modus dürfen fachlich nicht aufgeweicht werden.
- Akut-Modus muss eng und sicher führen.

## Technische Regeln

- index.html bleibt die Startdatei.
- CSS liegt in assets/css.
- JavaScript liegt in assets/js.
- Daten liegen in data.
- Keine Klassen oder IDs umbenennen, wenn dadurch bestehende Logik brechen könnte.
- Bestehende localStorage-Daten möglichst kompatibel halten.
- JSON Import/Export muss weiter funktionieren.
- Keine Patientendaten, Echtdokumentationen oder personenbezogenen Testdaten ins Repository einfügen.

## Testfälle nach jeder Änderung

Die vollständige Prüfliste steht in `docs/testfaelle.md`. Nach jeder Änderung sind mindestens Startseite, Tabs, Module, Planung, Dokumentation, Handbuch, Druck sowie JSON Import/Export zu prüfen.

## Lokaler Test

Da Daten per `fetch` aus JSON geladen werden, lokal mit einem Server testen:

```text
python -m http.server 8000
```

Danach `http://localhost:8000` öffnen.

## Stil

Code klar, einfach, kommentiert und wartbar halten. Keine unnötige technische Komplexität.
