# Genesee County Flock archive

This is an archive of [Flock Safety transparency portals](https://transparency.flocksafety.com/) for Genesee County CLEMIS agencies. It collects the data those portals publish — search audits, share lists, and page snapshots — before that material falls off the public record. The portals keep about 30 days of search audits; after that window the same records are only available through FOIA.

No public portal captured yet. Known CLEMIS member Flock users in this county are probed daily; a live URL with a search-audit CSV is captured and added here.

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

Watch list (probed daily, not yet public): Grand Blanc Twp MI PD, Fenton MI PD.
