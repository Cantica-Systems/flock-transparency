# Michigan Flock transparency archive

One repo for [Flock Safety transparency portals](https://transparency.flocksafety.com/) in Michigan, grouped by county. Each portal's search audits, share lists, and page snapshots are copied here before they age off the public page (about 30 days). After that window the same records are only available through FOIA.

| County | Folder | Live portals |
|---|---|---|
| Kent | [`kent/`](kent/) | Grand Rapids PD, Kent County SO, Walker, Wyoming, Grandville, Lowell, Rockford DPS |
| Ottawa | [`ottawa/`](ottawa/) | Holland PD |
| Kalamazoo | [`kalamazoo/`](kalamazoo/) | Kalamazoo DPS, Portage PD |
| Muskegon | [`muskegon/`](muskegon/) | none yet — Muskegon PD portal is live without a public search-audit CSV |
| Allegan | [`allegan/`](allegan/) | none yet — guessed slugs kept for ad-hoc probe |
| Wayne | [`wayne/`](wayne/) | Taylor PD, Sumpter Twp PD |
| Oakland | [`oakland/`](oakland/) | none yet — Ferndale portal is inactive; Troy has no audit CSV |
| Macomb | [`macomb/`](macomb/) | none yet — guessed slugs kept for ad-hoc probe |
| Washtenaw | [`washtenaw/`](washtenaw/) | none yet — Milan portal has no public search-audit CSV |
| Genesee | [`genesee/`](genesee/) | none yet — guessed slugs kept for ad-hoc probe |
| St. Clair | [`st-clair/`](st-clair/) | none yet — guessed slugs kept for ad-hoc probe |
| Lenawee | [`lenawee/`](lenawee/) | none yet — guessed slugs kept for ad-hoc probe |

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

Search-audit CSVs are partitioned by **search time**. Share lists are the current portal snapshot; `git log -p <county>/data/<agency>` is the history. Kent and Ottawa dumps were grafted from the old `*-co-mi-flock` repos (now archived).

## Columns (search audits)

| Column | Meaning |
|---|---|
| `id` | Flock search UUID |
| `userId` | redacted by the portal (`***`) |
| `searchDate` | UTC timestamp of the search |
| `networkCount` | networks/devices included in that search |
| `offenseType` | stated search reason |
