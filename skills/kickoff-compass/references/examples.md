# Examples (format only)

These show the **format**. Never copy their content: drop any question the person has already answered, and
write options from their situation. Scenario used here: a dog-grooming salon owner who wants online booking with
an AI assistant that answers questions.

## Contents
- Interview round 1 (first reply, beginner)
- Interview round 2 (follow-up)
- Pushback on a risky requirement
- Approaches with a conditional recommendation
- Phases table (configure path) with checkable "Done when"
- Progress report after a phase

## Interview round 1 (first reply, beginner)

> Think of me as the builder you've just hired. First, a short interview so I build the right thing.
>
> **What I understood:** you want customers to book grooming online, and an assistant to answer the questions
> that keep your phone ringing. *Example:* a customer opens your page at 10pm, picks "full groom, small dog",
> chooses Saturday 9am, and gets a confirmation and a reminder the day before; you see it in your calendar.
> *Assuming:* one salon, two groomers, customers pay in the salon. *Missing:* your price list and opening hours.
>
> **Honest first thing:** salon booking apps already do most of this, so we probably don't need to build
> anything from scratch.
>
> **1. What should the assistant handle first?**
> - **A. Booking and rescheduling, plus price questions (recommended):** these are most of your calls.
> - B. Everything, including questions about pets' health
> - C. Booking only
>
> **2. Which country is the salon in?** *(No default: it decides which privacy and payment rules apply.)*
>
> **3. When a customer mentions a pet's health problem, what should happen?**
> - **A. The assistant says "please mention this to the groomer" and flags the booking for you (recommended):**
>   it must not give animal health advice.
> - B. It answers from a fact sheet
>
> *Reply like "1A, 2: Ireland, 3A", or just "OK" to take my recommendations, but please answer question 2
> directly.*
>
> After one or two quick rounds like this, I'll bring you a proposal: options, risks, a step-by-step plan, and
> rough time and cost. I've saved where we are; just say "continue my dog salon project" any time.

## Interview round 2 (follow-up)

> Thanks: booking and prices first, Ireland, and health questions go to you. Got it.
> Two things your answers raised:
>
> **4. Customers sometimes don't turn up. What should happen?**
> - **A. The system flags no-shows and you decide whether to charge, with one tap (recommended)**
> - B. No fee
> - C. Charge a fee automatically (see my warning below)
>
> **5. Do you already use a calendar or booking tool?**
> - **A. A paper diary or phone calendar only (recommended guess)**
> - B. Yes: ___
>
> *Reply like "4A, 5A", or "OK". That's all I need; next comes the proposal.*

## Pushback on a risky requirement

> You asked for the assistant to **charge a no-show fee automatically**. I'd advise against doing that in
> version 1:
> - A wrong charge (for a customer who did cancel by phone) costs you a customer, and may trigger a dispute.
> - Payment rules differ by country, and storing card details brings strict security duties.
>
> **Safer option (recommended):** the system flags no-shows, and you decide whether to charge, with one tap.
> I've kept automatic charging as option C in question 4, so it's your call with the risks in view.

## Approaches

| | A. Booking app + its built-in assistant (recommended) | B. Booking app + custom AI helper | C. Build your own |
|---|---|---|---|
| What | An existing salon booking service, set up well | The same app, plus a small AI program for questions | A new website and booking system |
| Pros | Live in days; payments and reminders included | Answers any wording; your own tone | Exactly what you want |
| Cons | Monthly fee; less control over answers | Extra setup and a small monthly AI cost | Weeks of work; you maintain it |
| Effort / cost (estimates) | 1-2 days / ~$20-60 a month | A few sessions / +$5-20 a month | Weeks / most expensive |

**Recommendation:** go with **A**, and add B later only if customers' questions aren't answered well. If you need
features no booking app has, we'd look at C.

## Phases (configure path)

| # | Phase | What you get | Done when |
|---|---|---|---|
| 0 | Prep & checks | Price list, service list, today's baseline (calls per day), 2 booking apps trialled | Trial notes with prices from the official sites; baseline counted for one week |
| 1 | Booking live (visible) | Customers book online; reminders sent | A friend books, reschedules and cancels; all three show in your calendar within a minute |
| 2 | Questions answered | Assistant answers prices, hours, what to bring | 18 of 20 real past questions answered correctly; every health mention flagged to you |
| 3 | Handover | A one-page guide: change prices, hours and answers | You change the opening hours yourself using only the guide |

## Progress report after a phase

> **Phase 1 done: online booking is live.**
> - **Done:** booking page set up with your 6 services and both groomers; reminders switched on.
> - **Proof:** my test booking, reschedule and cancel all appeared in your calendar within 40 seconds.
> - **Next:** Phase 2, the question-answering assistant.
> - **Needed from you:** about 20 questions customers have asked you recently (no names or numbers).
