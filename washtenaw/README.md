# Washtenaw County Flock archive

This is an archive of [Flock Safety transparency portals](https://transparency.flocksafety.com/) for Washtenaw County CLEMIS agencies. It collects the data those portals publish — search audits, share lists, and page snapshots — before that material falls off the public record. The portals keep about 30 days of search audits; after that window the same records are only available through FOIA.

- **Milan MI PD**

Other Michigan counties are sibling folders in this repo. See the [root README](../README.md).

Latest summary: [`SNAPSHOT.md`](SNAPSHOT.md).

## Layout

```
data/
  <agency>/
    YYYY-MM.csv
    sharing_outbound.csv
    sharing_inbound.csv
    stats.csv

raw/
  <agency>/page.txt
  <agency>/page.html
```

Watched daily for a search-audit CSV: Milan MI PD.

Guessed slugs (ad-hoc probe, not daily): Washtenaw County MI SO, Ann Arbor MI PD, Ypsilanti MI PD, Pittsfield Twp MI PD, Chelsea MI PD, Saline MI PD, Northfield Twp MI PD.
