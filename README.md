# 2026 FIFA World Cup — Match Calendar

A subscribeable calendar of all 104 matches of the 2026 FIFA World Cup, refreshed
automatically several times a day as fixtures, teams and broadcasts are confirmed.

## Subscribe

- One-click: `webcal://debatepro.github.io/world-cup-2026-calendar/world-cup-2026.ics`
- Manual (paste into your calendar app): `https://debatepro.github.io/world-cup-2026-calendar/world-cup-2026.ics`

Subscribe once and you're set for the whole tournament. As group play wraps and teams earn
their spot in the knockout rounds, each match fills itself in — **when** it kicks off,
**where**, and **who** they're playing — right in the calendar you already use. No
re-checking, no re-downloading.

The feed filename — `world-cup-2026.ics` — is the **subscription contract** and will never
change, so your subscription keeps working for the life of the tournament.

## Staying up to date

The published feed is regenerated **automatically every 6 hours** and updated only when
something actually changes. Your calendar app then re-checks the feed on **its own
schedule** — typically every few hours, up to about once a day — an interval set by the app
(Apple Calendar, Google Calendar, etc.), not by this project. So new details land on their
own; there's nothing to re-import.

## Other formats

- `world-cup-2026.csv` — one row per match, with local-kickoff columns
- `world-cup-2026.json` — full structured dataset

These files are kept up to date alongside the feed, but they're **one-time downloads** — to
get the latest schedule you'll need to re-download them. Only the subscription above
refreshes on its own.

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

## Disclaimer

This is an independent, fan-created project. It is **not affiliated with, endorsed by, or
sponsored by FIFA**, the 2026 World Cup organizing committees, or any broadcast partner.
"World Cup", "FIFA World Cup" and related names are trademarks of FIFA; they are used here
only for factual identification of publicly scheduled matches.

Match schedules, kickoff times, venues and broadcast listings are factual information
compiled from publicly available sources and are provided **"as is", without warranty of
any kind**, express or implied. Details change — fixtures, times and broadcasters are
confirmed and revised over time — and no guarantee is made as to accuracy, completeness, or
timeliness. Verify against official sources before relying on any detail. To the maximum
extent permitted by law, the maintainers accept **no liability** for any loss or damage
arising from use of this calendar or its data.
