# Rubbish Open Data

Street litter and street-condition records collected with the [Rubbish](https://www.rubbish.love) app, 2018 to 2026: one photo per record, with time, place, type and count. Shared for researchers, cities and neighbors working on cleaner, healthier streets.

**211,321 records in 5 datasets.** License: [CC BY 4.0](LICENSE). Please cite as shown in [CITATION.cff](CITATION.cff).

| Dataset | Records | Items | Dates | Folder |
|---|---|---|---|---|
| Polk Street, San Francisco (2018 to 2021) | 145,925 | 166,019 | 2018-06-09 to 2021-10-13 | [data/polk-street](data/polk-street) |
| SoMa West, San Francisco (audits in 2019 and 2020) | 36,575 | 53,520 | 2018-05-09 to 2024-08-27 | [data/soma-west](data/soma-west) |
| River District, Sacramento (June 2021) | 18,606 | 18,606 | 2021-06-06 to 2021-06-09 | [data/sacramento-river-district](data/sacramento-river-district) |
| NoTraceTrails, Pacific Crest Trail survey (2023) | 913 | 1,085 | 2023-03-28 to 2023-09-24 | [data/notracetrails](data/notracetrails) |
| Events (2018 to 2026) | 9,302 | 12,647 | 2018-09-06 to 2026-03-21 | [data/events](data/events) |

## Files

- One CSV per dataset, UTF-8, one row per photo record, the same columns in every file: [COLUMNS.md](COLUMNS.md).
- How the data was collected, cleaned and checked: [METHOD.md](METHOD.md).
- `release-manifest.json`: row counts and SHA-256 of every file in this release.

## Privacy

No names, emails, account ids, photos or photo links, notes or house numbers. Locations are rounded to about 11 m, and to about 110 m for records that could point at people (tents, shelters, RVs, needles, human waste). See [METHOD.md](METHOD.md).

## Earlier work with this data

- [130,000 Reasons Why Data Science Can Help Clean Up San Francisco](https://medium.com/rubbish-love/130-000-reasons-why-data-science-can-help-clean-up-san-francisco-6412eba1e374) (2019)
- [Bringing together building, block, street, and point data](https://www.residentmar.io/2019/08/03/buildings-blocks-streets-points.html), Aleksey Bilogur (2019). We met at Code for America in 2018!
- Reddit r/dataisbeautiful: [Tobacco litter picked up on Polk Street, SF, over the course of a month](https://www.reddit.com/r/dataisbeautiful/comments/9lc2ir/tobacco_litter_picked_up_on_polk_street_sf_over/) and [part 2](https://www.reddit.com/r/dataisbeautiful/comments/b3rz14/oc_tobacco_litter_picked_up_on_polk_street_sf/); r/pics: [Over 8,000 cigarettes picked off the street to be recycled](https://www.reddit.com/r/pics/comments/azwtrz/over_8000_cigarettes_picked_off_the_street_to_be/)
- McGruer et al. (2025), [Lost on the Pacific Crest Trail: a 4,270 km survey of wilderness waste distribution and characteristics](https://doi.org/10.1016/j.wasman.2025.115063), Waste Management 206, 115063.

## Changes

- 2026-10-27: six datasets, 2018 to 2026, with a column guide and method. The Aug to Oct 2018 Polk Street spreadsheet (Feb 2020) is replaced by the full Polk Street set.
- 2026-11-10: five datasets; the cross-country drive is held back for now.

---
Made on Polk Street with love. Questions: hello@rubbish.love
