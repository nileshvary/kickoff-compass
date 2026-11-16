# Changelog

## Unreleased (2026-11-16)
- Docs: updated the compatibility section. No changes to the skill or the prompt.
- Removed the "Share your result" issue form.

## 1.1.0 (2026-11-15)
- Install is now one line: `npx skills add nileshvary/kickoff-compass`, plus `/kickoff-compass` switches
  (`continue`, `quick`, `all-at-once`).
- `SKILL.md` cut from 233 to about 130 lines; the working rules after "go" moved to `references/building.md`.
- YAML header rewritten as a folded block, so it parses in strict YAML readers and installers.
- Sharper trigger: does not run for scripts, single files or small fixes, even if the word "build" appears.
- Resume: if the person's reply answers every open question, it goes straight to the proposal.
- Facts are labelled official source, third-party (vendor-written), sources disagree, or estimate; clear wording
  when the AI cannot search the web.
- New question module: records, payments tracking and messaging channels.
- README rebuilt: install first, a demo image, the chat-app prompt behind a copy button, commands table.
- "Share your result" issue form, so people can report how it behaved in ChatGPT, Gemini and other AIs.
- Downloadable `kickoff-compass.zip` on the release page.
- README: a highlighted "Start here" box with the chat-app prompt shown open, so it cannot be missed.

## 1.0.0 (2026-11-14)
First public release.
- Size check: small tasks skip the interview.
- Beginner / intermediate / expert modes with length budgets.
- Fixed first-reply order: playback → honest first thing → questions → approaches → risks → draft plan → close.
- Ranked questions with lettered options, recommended answer first, "1A, 2C" or "OK" replies.
- Build / configure / buy approaches, with plan layouts for each.
- Pushback pattern for risky requirements.
- Fact checking with certainty labels.
- Question bank for 15 project types, review checklist, plain-words glossary.
- Works with any AI: full skill for Agent Skills-compatible coding agents, plus a paste-in prompt for ChatGPT, Gemini, Claude.ai and other chat apps.
- Save and resume: progress notes in ~/.kickoff-compass/ and a "Where we are" section in docs/PLAN.md, so work continues days later without repeating questions.
- Works like a hired professional: discovery interview in short rounds, then a proposal (options, risks, plan, time and cost), sign-off, phase-by-phase progress reports and a handover.
- Tested across beginners, intermediates and experts, on three model sizes, in both the skill and paste-in versions.
