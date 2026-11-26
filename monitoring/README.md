<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Beobachtung: was gelesen wird und was daraus folgte

[English](README.en.md)

Wie global-law jedes Land beobachtet: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). Diese Seite zeigt dasselbe nur für Bern: jedes Lesen einer amtlichen Quelle, wann, und was daraus folgte (Vorschriften hinzugefügt, geändert und entfernt). Maschinenlesbar in [data/checks/](../data/checks/) (JSON Lines, Schema `lexifina-check/1`), in `git log` als Commits mit `Kind: check` und Monat für Monat in [checks/](checks/).

**Letzte Prüfung:** 2026-11-26 06:10 UTC, Bern: Systematische Sammlung (www.belex.sites.be.ch): 226 Adressen gelesen; 62 hinzugefügt, 0 geändert, 1 entfernt; Änderungen gefunden; 15 nicht veröffentlicht, davon 0 ohne Grund.

## Quellen

| Quelle | Ordner | Wie oft | Letzte erfolgreiche Prüfung | Letztes Ergebnis | Stand |
| --- | --- | --- | --- | --- | --- |
| [Bern: Systematische Sammlung (www.belex.sites.be.ch)](https://www.belex.sites.be.ch/) | `<act>/` | täglich | 2026-11-26 06:10 UTC | Änderungen gefunden | beobachtet |

## Die letzten 30 Tage

| Beginn (UTC) | Quelle | Gelesen | Hinzugefügt | Geändert | Entfernt | Nicht veröffentlicht (ohne Grund) | Ergebnis | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-26 06:02](checks/2026-11.md#ch-lexwork-bern-20261126t060233z) | lexwork-bern | 226 | 62 | 0 | 1 | 15 (0) | Änderungen gefunden | [97](https://github.com/lexifina/switzerland-bern-law/compare/95ad4ca483cf...670e281fe74d) |
| [2026-11-25 06:18](checks/2026-11.md#ch-lexwork-bern-20261125t061813z) | lexwork-bern | 416 | 208 | 4 | 1 | 82 (0) | Änderungen gefunden | [245](https://github.com/lexifina/switzerland-bern-law/compare/ad98aa0d0025...92f647c8e433) |
| [2026-11-24 14:40](checks/2026-11.md#ch-lexwork-bern-20261124t144009z) | lexwork-bern | 227 | 208 | 2 | 1 | 213 (0) | die Prüfung ist fehlgeschlagen | — |
| [2026-11-24 11:58](checks/2026-11.md#ch-lexwork-bern-20261124t115847z) | lexwork-bern | 403 | 208 | 4 | 1 | 218 (0) | die Prüfung ist fehlgeschlagen | — |

## Selbst prüfen

```
python tools/checktrail.py                      # die letzte Prüfung jeder Quelle
python tools/checktrail.py --day 2026-11-23     # jede Prüfung eines Tages
python tools/checktrail.py --act <id>           # wann eine Vorschrift gesehen und veröffentlicht wurde
git log --grep='^Kind: check' --format='%ci %s'  # die Prüfungen in der Historie
```

Rechtskraft hat nur die amtliche Verkündung; die Texte hier sind Kopien zum Lesen und Suchen.
