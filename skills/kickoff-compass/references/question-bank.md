# Question bank

A **menu, not a checklist**. Consider the Core groups for every project, add the module(s) matching the project
type, then drop, rank and cap as SKILL.md Step 2 says. Every question you ask needs lettered options with the
recommended one first (or *(No default)* for facts only the person knows). Hints in *(italics)* are suggested
defaults, not text to paste.

Contents: Core (C1–C6) · AI chatbot/assistant · AI agent with tools · Knowledge / RAG · Automation / workflow ·
Web app / SaaS · Selling & subscriptions · Records, payments tracking & messaging channels · Dashboard / data · Mobile app · API / backend · ML model ·
Decisions about people (hiring, credit, housing, grading) · Health & wellness · Security tool · Browser extension ·
Game

---

## CORE — ask for every project

### C1. Goal and people
- What problem does this solve, in one sentence? Who has that problem today?
- Who will use it: just you, your team, customers, the public?
- Is this a learning project, a demo/portfolio, an internal tool, or a real product people will pay for?
- What does "success" look like in 1 month? (e.g. "10 people use it weekly", "I can demo it in an interview")
- How is it done today, and roughly how long does it take? *(This gives the baseline for success measures.)*
- Have you tried existing tools for this? What was missing? *(Check yourself first. If a strong product exists,
  ask instead: "Should we trial X before building anything?")*
- Where are you (country or state)? *(No default. Ask it first whenever law, money, health, hiring or sensitive
  personal data is involved; see SKILL.md Step 2.)*

### C2. User journey
- Walk me through what a user does, step by step, from first opening it to getting the result.
- What is the ONE most important thing a user must be able to do? (This becomes the first demo.)
- Do users need to log in? Are there different kinds of users (admin vs normal)?

### C3. What they see
- Where does it live: website, phone app, desktop app, chat (Slack/Teams/WhatsApp), command line, no UI?
- Any look you like? Name 1–2 products whose feel you want, or brand colours/logo.
- Which pages or screens are must-haves for version 1?

### C4. Data
- What information goes in, and where does it come from? (typed by users, files, another system, the web)
- Does any of it involve personal or sensitive data? (names, emails, health, money, IDs, passwords)
- How long should data be kept? Who may see it?

### C5. Constraints
- Budget: free only, a few dollars a month, or more?
- Deadline or pace?
- Your computer: Windows / Mac / Linux? Limited disk space or an old machine? (Check it yourself where possible.)
- Must it work offline or stay entirely on your own machine?
- Any tools, languages or vendors you must use or must avoid?
- (Company projects) Existing infrastructure to reuse? Security/legal approvals needed? Who owns it after launch?
- (Safety-critical content: health, allergies, money, legal) What must always go to a human instead of the AI?

### C6. Setup and ownership
- Where should the project folder live? Do you want it on GitHub (private or public)?
- Who provides accounts and API keys? *(Recommend: the person creates them and enters keys in a private place
  themselves, such as a `.env` file or the tool's own settings; never in chat.)*
- Where will it run later: just your computer, a cloud host, an app store?
- How do you want to work: approve each phase, or let me run through several?

---

## MODULE: AI chatbot / assistant
- What should it know, and what should it NOT talk about?
- Which AI model/provider? Any you can't use (cost, privacy, company policy)? *(Recommend a cheap fast model for tests.)*
- Should it remember past conversations?
- Tone and persona? Languages?
- What happens when it doesn't know: say so, hand off to a human, search?
- Streaming (word-by-word) replies needed? *(Usually no for v1.)*
- How will you judge good answers? (a test set of example questions with expected answers)

## MODULE: AI agent with tools
- What actions can it take (send email, edit files, call APIs, browse, pay)? List them.
- Which actions are dangerous and need human approval first? *(Recommend: anything that sends, deletes, pays or publishes.)*
- Should tools be fake (mock) while building? *(Strongly yes.)*
- What must it never do, no matter what a user or a web page says? (prompt-injection boundary)
- Limits: max steps, max cost, max time per task?
- Does it talk to other agents? Are their messages trusted?

## MODULE: Knowledge / RAG (AI answering from your documents)
- Build or buy? *(Many suites now include AI search over their own documents; a short trial against real
  questions sets the bar to beat.)*
- What documents (type, how many, how big), and how often do they change? How fresh must answers be?
- How will we judge answer quality? *(Recommend: 50-100 real past questions, each with its known correct source.)*
- Which areas must be excluded outright (HR, legal, security)?
- Who may see which documents? (permissions must follow into answers)
- Should answers cite sources?
- Is any content confidential enough that it must not go to a cloud AI provider? Is there company approval
  (data-processing / zero-retention terms) to send it?
- How do we map a chat/app user to their identity in the source system? *(Recommend: refuse if unmapped.)*
- How fast must a permission change take effect?
- Where are answers shown? *(A reply in a shared channel leaks to everyone in it.)*
- What gets logged for audit, without storing raw questions or answers?

## MODULE: Automation / workflow
- What triggers it (a schedule, an email, a form, a file)?
- What are the exact steps, and what's the final output?
- What should happen when a step fails: retry, alert, stop?
- Which apps does it connect to, and do you have admin access to them?

## MODULE: Web app / SaaS
- Accounts: email/password, Google login, magic link, none?
- Payments needed now or later?
- Single user, team accounts, or many separate customers (multi-tenant)?
- Mobile-friendly required?
- Landing/marketing page now or later? *(Usually later.)*

## MODULE: Selling & subscriptions
- When do payments come in? *(Usually after real users show they want it.)*
- Price idea, and does the cost per user (AI usage, hosting) fit under it? *(Measure in Phase 0.)*
- Selling through app stores? *(They take a share and have their own rules; verify current terms.)*
- Refunds, cancellations, free trial? Tax and invoicing where you sell?
- Privacy policy and terms needed? *(Yes, if you collect any personal data or sell to the public.)*

## MODULE: Records, payments tracking & messaging channels (who paid, lists, bookings, WhatsApp/SMS/email)
- What exactly must be tracked (who, what, when, how much), and where does it live today (paper, phone, sheet)?
- Who may see or change the records? *(Recommend: only the owner. Keep amounts and personal details minimal.)*
- Does the system only record, or also message people? *(Recommend: record and draft; a human sends anything about
  money or changes.)*
- Which channel do customers use (WhatsApp, SMS, email, Instagram)? *(Automating a personal WhatsApp account can
  break its terms; business tools have their own rules. Verify before planning on it.)*
- Are any customers children? *(Then keep only what's needed, and put parent details only where required.)*
- What is the cost of a mistake here (wrong amount, missed booking)? *(Sets how much human checking is needed.)*

## MODULE: Dashboard / data
- Which numbers matter most, the first 3–5 things someone looks at?
- Where does the data come from and how fresh must it be (live, every few seconds, daily)?
- Who views it, and can they change anything or only look?
- Export needed (CSV, PDF)?

## MODULE: Mobile app
- iPhone, Android, or both? App store release or just your own phone for now?
- Needs camera, location, notifications, offline mode?
- *(Often recommend a mobile-friendly web app first: faster and free to ship.)*

## MODULE: API / backend
- Who calls it: your own frontend, other developers, other services?
- Authentication method? Rate limits?
- Expected traffic now vs later?

## MODULE: ML model (training your own)
- Do you already have labelled data? How much?
- Could an existing AI model + good prompting solve it instead? *(Often yes; say so.)*
- How will you measure accuracy, and what's "good enough"?
- GPU available, or CPU only?

## MODULE: Decisions about people (hiring, credit, housing, insurance, grading, benefits)
- Where are the people affected? *(No default. Rules on automated decisions and discrimination vary by place.)*
- Does a person make the final decision? *(Recommend: yes. The AI sorts and explains, a person decides; no
  automatic rejection in version 1.)*
- Who writes the criteria? *(Recommend: a person writes clear must-haves; the AI compares against them only.)*
- Are people told AI is involved, and can they ask for a human review? *(Often legally required; good practice.)*
- How do we test fairness? *(Recommend: the same case with different names/genders/ages must get the same result.)*
- Who approves sending personal data to an AI service, and how long is it kept?
- Could applicants game it (hidden text, keyword stuffing)? *(Test for it.)*

## MODULE: Health & wellness (habits, mood, sleep, fitness, diet, pets' health)
- What must it never do? *(Recommend: no medical, mental-health or diet prescriptions; a fixed, kind message
  pointing to a professional or helpline for serious topics.)*
- Who computes the patterns? *(Recommend: plain code counts and compares; the AI only words the result.)*
- Where does the data live, and can users delete it all? *(Recommend: minimal data, a "delete everything" option.)*
- Does it fall under health-data rules where you operate? *(Verify; stricter rules can apply.)*

## MODULE: Security tool
- What are you protecting, from whom? (threat model in one paragraph)
- Watch-only first, or block from day one?
- Fail open or fail closed when the tool itself breaks?
- What must never be logged? (raw secrets, personal data)
- How will you prove it works? (attack test set + safe set to measure false alarms)
- Which frameworks to map to? (e.g. OWASP Top 10 lists)

## MODULE: Browser extension
- Which browsers? Which websites does it act on?
- What permissions does it need? *(Ask for the minimum; stores reject over-broad ones.)*
- Does it send page content anywhere? (privacy)

## MODULE: Game
- Genre, platform, single or multiplayer?
- Your own idea and art, or inspired by something? *(Build original: don't copy an existing game's name, characters or art.)*
- Smallest playable version?
