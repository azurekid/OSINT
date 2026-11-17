# OPERATION ESPRIT: Participant Case Log

```
    /\_/\
   ( ◣_◢ )       OPERATION BLACKCAT
    > ^ <        Digital Investigation Division
   /_____\       Investigator copy — do not share outside your team
```

**Case reference:** DI-2026-0518 · Read the [case briefing](README.md) first.

## Rules of engagement

- Use open-source intelligence only. Public platforms and public web pages are in scope.
- Do not contact any person or business, post, comment, or create accounts.
- Everything online that relates to this case is fictional. Real businesses and landmarks appear only as places; do not disturb them.
- Some platforms are not well indexed by search engines. If a search returns nothing, go to the platform and navigate it directly.
- Record **where** you found every answer. Findings without a source do not count.

## Evidence pack

| File | Description |
|---|---|
| [`campus_photo.jpg`](campus_photo.jpg) | Preserved copy of the deleted Flickr upload |
| [`cell_tower_log.csv`](cell_tower_log.csv) | Carrier tower records for both devices, keyed by IMEI |
| [`suspect_gps.gpx`](suspect_gps.gpx) | GPS history recovered from the first device's cloud backup |
| [`buyer_gps.gpx`](buyer_gps.gpx) | GPS history from the handset recovered at Paddy Coyne's Irish Pub |

### Data conventions

- `cell_tower_log.csv` timestamps are **local Pacific time (PDT, UTC−7)**. Rows are not guaranteed to be in chronological order.
- GPX timestamps are **UTC**. Convert before comparing them with the tower log.
- Coordinates are decimal degrees (WGS84). Tower coordinates are the tower position, not the handset position.
- The GPX files can be opened with [gpx.studio](https://gpx.studio), Google Earth, or QGIS.

## Phase 1 Photo forensics (`campus_photo.jpg`)

Inspect the file's embedded metadata (for example with `exiftool`).

- [ ] 1.1 Camera make and model
- [ ] 1.2 GPS coordinates (decimal degrees)
- [ ] 1.3 The campus landmark shown in the photo
- [ ] 1.4 The `Artist` field
- [ ] 1.5 When the photo was taken

## Phase 2 Digital footprint

Work from the photo outward to the person behind it.

- [ ] 2.1 The Flickr username of the uploader
- [ ] 2.2 Which building does the uploader refer to as the place "where history sleeps"?
- [ ] 2.3 Which iconic animal sculpture at a Seattle public market appears in the uploader's photos?
- [ ] 2.4 What is the slogan of the business at the centre of the market exchange?
- [ ] 2.5 What is that business called?
- [ ] 2.6 The uploader's Instagram handle
- [ ] 2.7 Which two Seattle locations does the Instagram account place the uploader at between 22 and 24 March?
- [ ] 2.8 The uploader's blog URL

## Phase 3 Travel reviews

- [ ] 3.1 Which Seattle music venue did the subject review?
- [ ] 3.2 What time did the subject say they left?
- [ ] 3.3 Which Redmond restaurant did the subject review?
- [ ] 3.4 What did the subject say makes that restaurant "convenient"?
- [ ] 3.5 Which Bellevue pub did the subject review?
- [ ] 3.6 What does the pub's own website say about its current service status?

## Phase 4 Blog intelligence

- [ ] 4.1 Title of the 22 March blog post
- [ ] 4.2 What artifact does the post describe, and what do you know about it?
- [ ] 4.3 Which street is named by the secondary commenter?
- [ ] 4.4 Which unit number is named?
- [ ] 4.5 What phrase is used to confirm the second meeting?

## Phase 5 Telemetry analysis

- [ ] 5.1 Which East Link station is nearest the 08:52 ping on 25 March?
- [ ] 5.2 At what time does a device ping the tower near Building 34?
- [ ] 5.3 On which street is the Bellevue tower located?
- [ ] 5.4 When does the SeaTac ping occur, and what does it suggest?
- [ ] 5.5 Plot both GPX tracks. At which locations do the two devices overlap in time and place?
- [ ] 5.6 In which city does the second device's track begin?

## Phase 6 Final report

- [ ] 6.1 Name the storage facility where the stolen item is being held.
- [ ] 6.2 Give the unit number.
- [ ] 6.3 Reconstruct the suspect's timeline from 24 March to the SeaTac ping, with a source for each entry.
- [ ] 6.4 Summarise the suspect's identity and online footprint (names, aliases, accounts).

Several towers and places in the evidence look alike. Check each against the whole record before you commit to it.

## Timeline worksheet

| Date / time (state the timezone) | Location | Source | Activity |
|---|---|---|---|
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |

## Flag submission

When you have located the storage facility, build your flag from:

1. the street name of the storage facility, and
2. the unit number.

Format: lowercase words separated by underscores, then `_unit` and the number, inside `BC{...}`. For example, a facility on *Example Ave SW* in *unit 7* would be written `BC{example_ave_sw_unit7}`.

**Team name:** ______________________  **Flag:** `BC{ ______________________ }`

Hint cards are available from the facilitator, at a points cost.

---

*"History is just another vault. Someone always has the keys."*
