# AI Quest 2026 — event website

## Overview

The website for **AI Quest 2026**, the two-day inter-university AI competition run by the
Data Science Club at Al Hussein Technical University on 9–10 October 2026, powered by the
Islamic International Arab Bank.

The site carried the event end to end: it opened registration, published the rules,
schedule and terms, ran the two competition pathways — the Future Jordan Hackathon and
the ML Arena — took submissions on the day, and closed by announcing the winners.

Everything lives in **one HTML file**. Markup, styles, scripts, logos, photographs, the
mascots and a hidden video clip are all embedded. No build step, no dependencies, no
server — open it in a browser and it works, or drop it on any static host and it's live.

Two versions exist:

| File | What it is |
|---|---|
| `ai-quest-2026.html` | The live site, as it ran up to and during the event |
| `ai-quest-2026-ended.html` | The after site — thank-you page, the nine winning teams, the organising team |

## Key Features

- **Single self-contained file.** Hash-based single-page router, around 3,700 lines, with
  every asset inlined as a data URI. Rename it `index.html` and upload — that is the
  entire deployment.
- **Five-step registration** with live validation: team size enforced per pathway (2–5 for
  the hackathon, 2–3 for the arena), a 10-digit phone cap, a maximum of two interests,
  per-member university so teams can mix campuses, and a required terms agreement. Teams
  get a reference code at the end.
- **Submission portal** that opens and closes on a clock, with a live countdown and draft
  answers kept in the browser so a refresh loses nothing.
- **Two-day schedule** with shared rows and split rows, so each pathway's own programme is
  visible at a glance.
- **Published judging criteria** — three judge roles and six weighted criteria, drawn as
  animated bars.
- **Winners page** — three podiums with team photographs, first place raised and carrying a
  slow light sheen, cards rising in as they scroll into view.
- **Team photo wall** — photographs at slight tilts that straighten and lift on hover, and
  open full size in a viewer with arrow-key and Escape support.
- **Original mascot system.** The club's robot characters are drawn as inline SVG in two
  colourways, animated per page, never bitmap images.
- **Themed page transitions.** Each destination arrives through its own short scene — the
  mascot raising the flag of Jordan for the hackathon, a coin flip for the sponsors, a
  planning board for the schedule.
- **Bilingual Terms & Privacy** in English and Arabic.
- **Three easter eggs**, including a hidden clip with four different ways in.
- **Accessible and responsive.** Every animation respects `prefers-reduced-motion`, the nav
  collapses to a burger menu on narrow screens, and the layout is clean from 320px to
  2560px with no horizontal overflow.

## Objectives

1. **Give the competition one authoritative home** — rules, dates, team sizes, tracks and
   terms in a single place, so every team from every campus plans against the same
   information.
2. **Make registering easy and the data clean** — validate team composition, contact details
   and consent at the point of entry rather than chasing teams afterwards.
3. **Run the event day itself**, not just advertise it — a live schedule, a timed submission
   window and published judging criteria.
4. **Represent the sponsors properly**, with the Islamic International Arab Bank present on
   every page as the presenting partner.
5. **Carry the Jordan.next() identity** into a working interface — the mascots, the pixel
   shemagh, the palette and the typography, so the site feels like the event.
6. **Outlive the competition** — close by thanking everyone, crediting the organising team
   and the ambassadors, and leaving the nine winning teams on record.
