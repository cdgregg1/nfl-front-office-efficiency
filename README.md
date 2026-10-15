# NFL Front Office Spending Efficiency Analysis

## The Question

Which NFL front offices get the most win-value out of the post-rookie
contract window? And which teams waste the least money on players they
misjudged?

## Purpose

Most cap efficiency content online just ranks teams by spend versus wins,
which doesn't really show why a team ends up looking good or bad. This
project looks specifically at the decision point every front office faces
with their own draft picks — years 5 through 7 of a player's career, right
after the rookie deal ends — to see which teams consistently make the correct
call in the longterm and which ones don't. The goal isn't just to rank the five teams
against each other, it's to actually explain what's driving the difference:
timely extensions, letting good players walk for nothing, dead cap from
players a team misjudged, and so on. Based on the data collected so far, this approach 
is already surfacing real differences in how front offices handle this decision — where a team is doing well,
and where it's actually costing itself value.

## Overview

Five teams were picked to represent a spread of public front-office
reputations, so the project can test whether the data actually backs that
reputation up or not. For each team, every player drafted (or signed as a
UDFA) in 2017, 2018, or 2019 is tracked through their transition window, and
the front office's decision — extend, tag, trade, or let walk — gets logged
along with the contract terms involved. Full reasoning behind the team
selection and the exact rules used are in `METHODOLOGY.md`.

## Tech Stack

- [**Airtable**](https://airtable.com/invite/l?inviteId=invmEQyD3DefBzldd&inviteToken=aaa62090eb7a2627e19493eb344aa59c4f859d95b595028f75a8dcb088570daf&utm_medium=email&utm_source=product_team&utm_content=transactional-alerts) — where the player and contract data actually gets built 
- **SQLite / DB Browser for SQLite** — for querying and comparing across teams
- **Excel** — used for cleaning and cross-checking data during collection

## Methodology

The full methodology — why these five teams, how the transition window is
defined, the outcome categories, and how the data was collected and
verified — is documented in [`METHODOLOGY.md`](./METHODOLOGY.md).

## Findings

See [`FINDINGS.md`](./FINDINGS.md) for the running log of patterns found so
far. This gets updated as each team's data is finished, so it's not a final
conclusion yet — more of a working log of what's showing up in the data.

## Progress

| Team | Players | Contracts | Status |
|------|---------|-----------|--------|
| Eagles | 55 | 19 | Complete |
| Chiefs | 18 | 20 | Complete |
| Saints | 19 | 17 | Complete |
| Browns | — | — | In Progress |
| Cardinals | — | — | In Progress |

## Intended Output

Once all five teams are done, the findings will get pulled together into a
team-by-team breakdown showing:
- **What's working** — decision patterns that reliably kept or extracted
  value from transition-window talent
- **What isn't** — recurring patterns where value was lost, whether that's
  letting a good player walk for nothing or delayed decisions that led to
  dead cap
