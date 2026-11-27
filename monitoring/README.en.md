<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoring: what is read and what came of it

[Deutsch](README.md)

How global-law monitors every country: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). This page is the same for Bern only: every time an official source is read, when, and what came of it (acts added, changed and removed). The machine-readable form is [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` as `Kind: check` commits, and month by month in [checks/](checks/).

**Last check:** 2026-11-27 06:03 UTC, Bern: systematic collection (www.belex.sites.be.ch): 306 addresses read; 0 added, 0 changed, 1 removed; changes found; 1 not published, 0 of them with no reason. Flags: `audit-disagrees`.

## Sources

| Source | Folders | How often | Last successful check | Last result | State |
| --- | --- | --- | --- | --- | --- |
| [Bern: systematic collection (www.belex.sites.be.ch)](https://www.belex.sites.be.ch/) | `<act>/` | daily | 2026-11-27 06:03 UTC | changes found | watched |

## The last 30 days

| Started (UTC) | Source | Read | Added | Changed | Removed | Not published (no reason) | Result | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-27 05:58](checks/2026-11.md#ch-lexwork-bern-20261127t055815z) | lexwork-bern | 306 | 0 | 0 | 1 | 1 (0) | changes found `audit-disagrees` | — |
| [2026-11-26 06:02](checks/2026-11.md#ch-lexwork-bern-20261126t060233z) | lexwork-bern | 226 | 62 | 0 | 1 | 15 (0) | changes found | [97](https://github.com/lexifina/switzerland-bern-law/compare/95ad4ca483cf...670e281fe74d) |
| [2026-11-25 06:18](checks/2026-11.md#ch-lexwork-bern-20261125t061813z) | lexwork-bern | 416 | 208 | 4 | 1 | 82 (0) | changes found | [245](https://github.com/lexifina/switzerland-bern-law/compare/ad98aa0d0025...92f647c8e433) |
| [2026-11-24 14:40](checks/2026-11.md#ch-lexwork-bern-20261124t144009z) | lexwork-bern | 227 | 208 | 2 | 1 | 213 (0) | the check failed | — |
| [2026-11-24 11:58](checks/2026-11.md#ch-lexwork-bern-20261124t115847z) | lexwork-bern | 403 | 208 | 4 | 1 | 218 (0) | the check failed | — |

## Check it yourself

```
python tools/checktrail.py                      # the latest check of every source
python tools/checktrail.py --day 2026-11-23     # every check of a day
python tools/checktrail.py --act <id>           # when an act was seen and published
git log --grep='^Kind: check' --format='%ci %s'  # the checks in the history
```

Only the official publication has legal force; the texts here are copies for reading and searching.
