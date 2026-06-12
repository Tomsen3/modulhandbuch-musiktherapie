# Datenstruktur

## `modules.json`

Enthält die 59 Modulprofile in der bestehenden, verlustfrei übernommenen Struktur sowie die bisherige Modulreihenfolge. Jedes Modul enthält Titel, Methode und das vollständige HTML des fachlichen Profils.

Die kompakteren Metadaten für Karte, Filter und Planung liegen aus Kompatibilitätsgründen weiterhin in `assets/js/modules.js`.

## `handbook.json`

Enthält Titelblock, Grundlagen- und Handbuchinhalt sowie Literaturverzeichnis als HTML. Die Handbuchansicht baut daraus Navigation, Suche und Schnellzugriffe auf.

## `recommendations.json`

Dokumentiert den vorgesehenen Ort für Empfehlungen. Die aktuell verwendeten Empfehlungen bleiben vorerst in `assets/js/planning.js`, damit sich das Verhalten beim Refactoring nicht verändert.

## `settings.json`

Enthält Bezeichnungen und Farben der vier Settings. Die bestehende Sicherheits- und Filterlogik bleibt derzeit in JavaScript.

## `glossary.json`

Enthält kurze Erklärungen zentraler Begriffe.

## Planung und Dokumentation

Die Planung darf Modulcodes, Wirkdimensionscodes und Dauerangaben anzeigen und speichern. Die automatische Dokumentation nutzt lesbare Modultitel, Methoden- und Wirkformulierungen und darf keine internen Kürzel oder Abschnittsdauern ausgeben.

## Kompatibilität

Die Struktur wurde zunächst verlustfrei ausgelagert. Eine spätere Normalisierung darf erst nach fachlicher Prüfung erfolgen und benötigt eine Kompatibilitätsschicht für bestehende Planungen und JSON-Exporte.
