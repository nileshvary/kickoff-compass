# Progress note (save and resume)

**Where:** `~/.kickoff-compass/<short-name>.md`, one file per idea (it covers the interview and the proposal). On Windows, `~` is `C:\Users\<you>`.
Create the folder if it doesn't exist. `<short-name>` is 2-4 lowercase words joined by hyphens, from the idea
(e.g. `dog-salon-booking`).

**When:** create it just before sending the first reply; update it every time you reply; set the status to
`moved` once the plan is saved in a project (SKILL.md Step 4, "On sign-off"), or to `done` / `dropped` if the person says so.

**Never store:** passwords, keys, tokens, or personal data the plan doesn't need. Write facts and decisions, not
whole conversations.

## Format

```markdown
# Kickoff: <idea in a few words>
- Short name: <short-name>          (what the person says to resume: "continue my <short-name> project")
- Status: in-progress | moved | done | dropped
- Started: <YYYY-MM-DD> · Last updated: <YYYY-MM-DD>
- Step reached: <e.g. "interview round 1 sent" | "round 2 sent" | "proposal sent, waiting for sign-off" | "signed off">
- Next step: <one concrete action, e.g. "Get answer to Q3 (country), then send the proposal">
- Level: beginner | intermediate | expert · Likely path: build | configure | buy | advice
- Moved to: <path of docs/PLAN.md or plan document, once status is moved>

## Idea in one paragraph
<their idea, in their own words where possible>

## Assumptions stated
- ...

## Facts found (with certainty)
- <e.g. "Tool X does Y, from £29/month: third-party listing, unverified"> · <e.g. "Rule Z applies: official source">

## Questions asked
| # | Status | Answer |
|---|---|---|
| 1 | answered | Ireland |
| 2 | answered | A (owner confirms) |
| 3 | open | |

## Open questions, full text   (copied exactly as sent, so they can be asked again word for word)
**3. <question>**
- **A. <option> (recommended):** <reason>
- B. <option>

## Decisions log
- <YYYY-MM-DD> Q2 → A: owner confirms every order

## Approach
- Options shown: A … / B … / C … · Recommended: … · Chosen: … (or "not yet")

## Draft plan (latest)
| # | Phase | Done when |
|---|---|---|

## Open items and blockers
- ...
```

## Resuming
1. Read the whole note.
2. Recap briefly (at most 5 short bullets): what's settled, what's open, the next step.
3. If their message answers anything or adds a new fact (their country, a new constraint), record it first, then
   check whether it changes a recommendation, a risk or Phase 0. Say so in one line if it does.
4. Continue from "Next step". Ask only the questions still open, copied from "Open questions, full text", with
   the same numbers.
5. If the last update is more than ~2 weeks old, or the plan depends on prices, rules or availability, offer to
   re-check those facts. Don't silently redo the work.
