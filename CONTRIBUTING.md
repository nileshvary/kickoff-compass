# Contributing to Kickoff Compass

Thanks for helping make project kickoffs better for everyone.

## Most helpful contributions
1. **Real-world reports.** Open an issue with: your idea (anonymised is fine), your experience level, what the
   skill got right, and what felt wrong, long or confusing.
2. **New question modules.** A project type that's missing (e.g. hardware/IoT, data pipelines, education)?
   Add a module to `skills/kickoff-compass/references/question-bank.md`.
3. **Glossary entries.** Tech words beginners stumbled on, for `references/plain-words.md`.
4. **Wording fixes** that make instructions clearer or shorter.

## Rules for changes to the skill
- Keep `SKILL.md` short (under 500 lines; it's about 180 today). Put detail in `references/`.
- Every question in the bank needs a sensible recommended default, or is marked *(No default)*.
- No real personal data in examples.
- Test your change: run the skill on at least two scenarios (one beginner, one expert) and describe the result
  in your pull request.
- Keep `prompt/kickoff-compass-prompt.md` in step with the skill and under 3,800 characters, so it fits every chat app.
- If you have Claude Code, run `claude plugin validate .` before opening a pull request.

## Code of conduct
Be kind, be specific, assume good intent.
