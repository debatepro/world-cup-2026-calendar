# 2026 FIFA World Cup — Match Calendar

A subscribeable calendar of all 104 matches of the 2026 FIFA World Cup, refreshed
automatically as fixtures, teams and broadcasts are confirmed.

## Subscribe

- One-click: `webcal://debatepro.github.io/world-cup-2026-calendar/world-cup-2026.ics`
- Manual (paste into your calendar app): `https://debatepro.github.io/world-cup-2026-calendar/world-cup-2026.ics`

The feed filename — `world-cup-2026.ics` — is the **subscription contract** and will never
change, so your subscription keeps working for the life of the tournament.

## Other formats

- `world-cup-2026.csv` — one row per match, with local-kickoff columns
- `world-cup-2026.json` — full structured dataset

## Sources & provenance

- **Schedule, teams, kickoff times** — [OpenFootball](https://github.com/openfootball/worldcup.json)
  (CC0), pinned to a specific commit for reproducible builds.
- **Stadium proper names and US TV** (English/Spanish) — publicly available sources, joined to the schedule by
  date + city (never by team name).

Each match carries an immutable slot identity (FIFA match number 1–104); knockout slots are
published as bracket-progression labels and fill in with real teams over time. `SEQUENCE`
and `DTSTAMP` only advance when a material field actually changes.

## Licensing

- **Match data** — [CC0-1.0](LICENSE) (public domain dedication).
- **Pipeline code** — [MIT](LICENSE-CODE).
