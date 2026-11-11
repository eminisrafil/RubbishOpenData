# Columns

Every CSV in `data/` has these columns, in this order.

| Column | Meaning |
|---|---|
| `release_id` | Stable id for the record in this release (not the app's id). Later releases keep the same id. |
| `dataset` | Which survey, audit or event the record belongs to. |
| `time_utc` | When the photo was taken, UTC. |
| `time_local` | The same time in `local_zone`. |
| `local_zone` | Time zone used for `time_local`, chosen by longitude (approximate near zone borders). |
| `lat, lon` | Where the photo was taken, WGS84. 4 decimals (about 11 m), or 3 decimals (about 110 m) for sensitive types. |
| `location_precision_m` | 11 or 110: how far `lat`/`lon` may be from the true point. |
| `street` | Street name only; house numbers are removed. |
| `city, state, zip` | From the phone's reverse geocoding at the time. |
| `rubbish_type` | The type chosen in the app (older records: one type per photo). |
| `items` | Newer records: each tagged item with its count, for example `bottle cap x2; cigarette butt x5`. |
| `categories, materials, brands` | Newer records: the item categories, materials and brands, when tagged. |
| `items_tagged` | How many pieces the photo covers. |
| `picked_up` | True when the litter was picked up, False when it was only recorded (audits record without picking up). |
| `is_311` | True when the record was sent on as a city 311 report. |

Empty cells mean the app did not record that value.
