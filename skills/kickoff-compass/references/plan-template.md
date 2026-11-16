# Plan template

Use it twice:
- **Draft** in the proposal (or, for experts, in the first reply): only what the length budget allows (beginners: the phases table, success
  measures and out-of-scope). The playback already covers the brief, so don't repeat it.
- **Final**, after the answers: the full layout below, saved at "go" (see building.md).

Pick the layout for the path: **Build** (new software) or **Configure / Buy / Advice** (existing tools).

## Build layout

*Use this when new software is built. With a beginner, describe Phase 0 in plain words ("set up a safe
workspace and a way to check your work") and leave out terms like version control and CI.*

```markdown
# <Project name>: Plan

## Where we are            (read first at the start of every session; update before stopping)
- Current phase: <# and name> · Status: <not started | in progress | blocked | done>
- Last thing done: <one line, date>
- Next step: <one concrete action>
- Open questions / blockers: <list, or "none">

## Brief
- Problem: who has it, and what it costs them today (baseline)
- Idea: one-line pitch
- Users: who, and the ONE thing they must be able to do
- Already out there: what was checked, and why we still build
- Version 1: the smallest thing that proves the idea

## How one <request / order / message> travels through it
1. ...

## Building blocks          (beginners/intermediate only; experts: fold into the technical section)
- What people see:  ...
- Engine room (backend):  ...
- Memory (database): what's stored, and what is never stored
- The brain (AI): model(s), its job, how answers are tested
- The locks (security): logins, secrets kept private, what's never logged, human approval for risky actions
- Where it lives: now → later

## Approach chosen
<options considered> → chosen: <X>, because <reason>

## Phases
| # | Phase | What you get | Done when |
|---|---|---|---|
| 0 | Foundation + spikes | new folder, version control, secrets kept out of it, tests, CI; spikes on riskiest assumptions | <checkable> |
| 1 | <smallest useful thing> | ... | ... |
| … | <visible demo within first third> | ... | ... |
| N | Docs + handover | ... | someone new runs it from the docs alone |
| later | Upgrades | ... | decided later |

## Success measures (what users notice; baseline → target)
## Out of scope (for now)
## Risks (risk → what we'll do)
## Decisions log (Q → A, date)
## Coverage
| Area | Clear / Assumed / Open | Note |
|---|---|---|
| Scope · Users · Legal · Data & privacy · AI behaviour · Security · Cost · Deployment | | |

---
## Technical section   (beginners: skip · intermediate: 2-4 lines · experts: the main body)
- Stack and why; architecture and data flow; data model
- Security: auth, secrets, input validation, logging policy, threats (incl. prompt injection if AI reads outside text)
- Dependencies: pinned versions, checked against advisories
- Testing: unit, integration, abuse/attack cases, safe cases, quality evals
- Technical targets (speed, cost, size), marked as estimates until measured
```

## Configure / Buy / Advice layout

```markdown
# <Project name>: Plan

## Where we are     (as above: read first each session, update before stopping)
## Brief            (as above; "Already out there" becomes the shortlist)
## Options compared (2-3 tools: price from the official site, fit, gaps, data/privacy terms)
## Decision         (chosen tool or approach, and why; what would make us switch)
## Steps
| # | Step | What you get | Done when |
|---|---|---|---|
| 0 | Prep & checks | content gathered, baseline measured, prices and rules verified, 1-2 tools trialled | <checkable> |
| 1 | <first visible result> | ... | ... |
| … | Pilot | real use with a small group | <measured against the baseline> |
| N | Handover | how-to for changing settings and content | someone else updates it from the how-to |
## Success measures · Out of scope · Risks · Decisions log
```

## Phase rules
- Secrets stay out of version control from the very first commit.
- Risky unknowns go in Phase 0 (does tool X work here? what does it really cost? what do the rules say?).
- Each phase fits in about one to a few sessions and produces something testable.
- "Done when" is checked by running or trying something, never by opinion.
