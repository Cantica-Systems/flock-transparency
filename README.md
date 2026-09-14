# Michigan Flock transparency archive

One repo for [Flock Safety transparency portals](https://transparency.flocksafety.com/) in Michigan, grouped by county. Each portal's search audits, share lists, and page snapshots are copied here before they age off the public page (about 30 days). After that window the same records are only available through FOIA.

| County | Folder | Live portals |
|---|---|---|
| Kent | [`kent/`](kent/) | Grand Rapids PD, Kent County SO, Walker, Wyoming, Grandville, Lowell, Rockford DPS |
| Ottawa | [`ottawa/`](ottawa/) | Holland PD |
| Kalamazoo | [`kalamazoo/`](kalamazoo/) | Kalamazoo DPS, Portage PD |
| Muskegon | [`muskegon/`](muskegon/) | none yet — Muskegon PD portal is live without a public search-audit CSV |
| Allegan | [`allegan/`](allegan/) | none yet — known Flock users are probed daily |
| Wayne | [`wayne/`](wayne/) | Taylor PD, Sumpter Twp PD |
| Oakland | [`oakland/`](oakland/) | none yet — Ferndale portal is inactive; Troy has no audit CSV |
| Macomb | [`macomb/`](macomb/) | none yet — Roseville, Eastpointe, Shelby Twp, Fraser probed daily |
| Washtenaw | [`washtenaw/`](washtenaw/) | none yet — Milan portal has no public search-audit CSV |
| Genesee | [`genesee/`](genesee/) | none yet — Grand Blanc Twp, Fenton probed daily |
| St. Clair | [`st-clair/`](st-clair/) | none yet — sheriff, Port Huron probed daily |
| Lenawee | [`lenawee/`](lenawee/) | none yet — sheriff, Adrian, Tecumseh, Madison Twp probed daily |

Latest per-county summary: `kent/SNAPSHOT.md`, `ottawa/SNAPSHOT.md`, and so on.

## Layout

```
<county>/
  README.md
  SNAPSHOT.md
  data/<agency>/YYYY-MM.csv
  data/<agency>/sharing_*.csv
  data/<agency>/stats.csv
  raw/<agency>/page.txt
  raw/<agency>/page.html
```

Search-audit CSVs are partitioned by **search time**. Share lists are the current portal snapshot; `git log -p` is the history.

## Columns (search audits)

| Column | Meaning |
|---|---|
| `id` | Flock search UUID |
| `userId` | redacted by the portal (`***`) |
| `searchDate` | UTC timestamp of the search |
| `networkCount` | networks/devices included in that search |
| `offenseType` | stated search reason |
