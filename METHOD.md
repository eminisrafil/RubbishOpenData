# Method

## Collection

Each record is one photo taken in the Rubbish app by a team member, volunteer or survey crew, with the phone's time and GPS. The person sorted what was in the photo: older app versions (2018 to 2021) took one type per photo plus a count; newer versions tag each item with a count, category and, where known, material and brand. Cleanups mark litter as picked up; audits and surveys record conditions without picking up.

## Selection

Records come from Rubbish's production database on 27 Oct 2026. Each dataset is defined by its team in the app and, for records saved before teams existed (2018 to 2021), by place and date: Polk Street by a box around the street (37.7765 to 37.8075 N, 122.4245 to 122.4180 W, from June 2018 to 2021); SoMa West by the district area, and for August 2019 by the audit's own categories. Records from our office area and other test records are left out; so are records outside each event's area and dates.

## Cleaning

- Removed: names, emails, account ids, photos and photo links, notes, IP addresses and house numbers.
- Record ids are replaced by `release_id`, a salted hash that stays the same across releases.
- GPS is rounded to 4 decimals (about 11 m). Records whose type or items include tents, temporary shelters, RVs, needles, human waste or urine are rounded to 3 decimals (about 110 m).
- Free text (types, items, brands, streets) was scanned for emails, phone numbers and links; none were found.

## Checks

- A second program, written separately and run on a separate pull of the database, re-selected every dataset; its row counts match this release exactly for every set.
- Published totals were compared with the data (for example the 2019 SoMa West audit: 27,478 items here against 27,461 concerns reported in 2019).

## Known limits

- Volunteers and crews choose where to look, so the data shows where people looked, not a random sample.
- Counts per photo are entered by people and can be off; very large counts were kept as entered.
- `local_zone` is chosen by longitude and can be wrong near time zone borders.
