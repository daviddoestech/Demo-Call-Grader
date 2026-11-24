---
name: "demo-call-grader"
description: "Grade recorded SaaS sales demos and discovery calls against a proven rubric: letter grades, timestamped wins and fixes, scripts, and a scorecard. Use when asked to grade, review or coach sales calls or demos."
---

# Demo Call Grader

Grades recorded sales demos for anyone selling SaaS over video calls. Output is short, specific and timestamped: what worked, the one fix that matters most, and the exact words to say next time.

## 1. Find the calls

Work out which calls to grade from the request ("my latest demo", "this week", a link, a shop or company name).

Pull transcripts from whatever the user has connected, in this order:
1. A call recorder tool (Fathom, Gong, Chorus, Fireflies, Zoom, Google Meet, Avoma, Nooks, Claude Meetings, etc.). List meetings in the date range, filtered to the user's own recordings, then fetch each transcript with timestamped links when the tool offers them.
2. A pasted transcript or uploaded file.
3. If nothing is connected, ask the user to connect their recorder or paste the transcript. Do not grade from an AI summary alone without saying so.

Skip internal meetings (standups, 1:1s, webinars). If a recording is under 3 minutes or clearly cut off, mark it **Not gradable** and tell the user to check their recorder settings.

For 3 or more calls, grade them in parallel with subagents (2 to 3 calls each) and have each return only the graded fields below, so full transcripts stay out of the main context.

## 2. Set up the rubric

On first use, ask once (skip anything already known from context or memory):
- What do you sell, and who is your ideal customer? (used to judge fit)
- Current pricing and guarantee or trial terms
- Target call length (default 30 to 35 minutes)
- Selling style, if any (default: Chris Voss tactical empathy: labeling, mirroring, calibrated "what" and "how" questions)
- Which 1 or 2 habits are you working on right now? Weight those most heavily.

## 3. The rubric

Score each call on these habits. Speaker labels in transcripts are often swapped, so judge who said what by content.

| # | Habit | What good looks like |
|---|---|---|
| 1 | Upfront contract | States the time and agenda in the first 2 minutes: "I've got 30 minutes. I'll ask a few questions, show the 2 or 3 things that matter, then we decide next steps. Fair?" |
| 2 | Qualify fit early | Confirms the prospect matches the ideal customer (system, size, use case) before demoing. Not a fit: shorten the call, stay helpful, ask for referrals. |
| 3 | Discovery before demo | Asks how they do it today, who does it and how long it takes before sharing the screen. |
| 4 | Price the pain in dollars | Turns time or errors into money: "10 hours a week times your $140 hourly rate is about $1,400 a week." Says the number back. Keeps the math simple enough to survive a check. |
| 5 | Their rule, built live | Gets one of their non-negotiables and configures it on screen, so the demo is about their business, not a generic tour. |
| 6 | Ask before show | Shows 2 or 3 features tied to stated pain. No monologue longer than about 2 minutes. Checks in with "What questions does that raise?" |
| 7 | Define the win | Asks "What would you need to see in the first 30 days to call this a win?" and gets a baseline number. |
| 8 | Price with confidence | States price, terms and guarantee clearly. No discount offered at first pushback. |
| 9 | Label objections | Names the fear before answering: "It sounds like you're worried the team won't use it." Pauses. Then a calibrated question. |
| 10 | Book the next step live | Calendar invite sent while still on the call, with every decision maker on it. "I'll reach out" or "ping me" does not count. |
| 11 | Stop at the buying signal | When they ask about rollout, price or onboarding, stops demoing and moves to next steps. |
| 12 | Call length | Within the target. Edge-case questions are parked for onboarding instead of tested live. |

Also weigh the "will it work for us" question: buyers usually assume the product is good. The strongest calls name the prospect's specific obstacle, show how they get results anyway, and cite a similar customer who did.

### Grading scale
- **A:** Closed or booked a firm next step on the calendar, priced the pain in dollars, under target length.
- **B:** Strong discovery and demo, but missed one of: dollar pain, calendar-booked next step, length.
- **C:** Missed two or more of the top habits, or let a warm buyer leave with no date.
- **D:** No discovery, no next step, or significant fit or tone problems.
- **Not gradable:** Recording too short or missing.

Adjust the letter up or down one step for outcome quality (for example, a fast and honest disqualification of a poor fit can be a B).

## 4. Output

Keep it short. Lead with the answer.

**Single call:**
- One line: grade, length, outcome.
- **Wins:** 1 or 2, each with a timestamp link and a short verbatim quote.
- **#1 fix:** the moment (timestamp link), what happened, and the exact script to use next time.
- Optional: one more fix, only if it is clearly worth it.

**Several calls:** a scorecard table first, then patterns.

| Demo | Min | Fit | Next step on calendar | $ pain | Grade |
|---|---|---|---|---|---|

Then:
- **What's working** (1 to 2 lines)
- **The pattern costing deals** (1 to 2 lines with the counts, e.g. "4 of 5 calls ended without an invite")
- **Habit for next week** with a script

Rules:
- Quote the prospect and seller verbatim where it helps. Never invent quotes, numbers or timestamps.
- Say which grades come from full transcripts and which from AI summaries or estimated lengths.
- Correct yourself plainly if an earlier grade or number was wrong.
- Use the seller's own terms for their product and customers.

## 5. Sensitive content check

Before the user shares or forwards any recording, flag anything that should not go out:
- The recorder kept running after the call ended and captured private conversation.
- Personal details: phone numbers, emails, health, family or financial matters.
- Internal company details: team size, roadmap, model or vendor names, weaknesses the seller admitted, other customers' data shown on screen.
- Pricing or discounts that differ from the official numbers (also check that teammates are quoting the same pricing).

List each with a timestamp and say "trim or don't share." Never save meeting content to memory unless asked.

## 6. Optional extras

- **Pre-call tip:** for an upcoming demo on the calendar, send a 3-line tip: record, qualify early, the one habit to focus on.
- **Running scorecard:** keep a living doc or sheet with each graded call (date, account, length, next step, dollar pain, grade) and update it as new calls are graded.
- **Cold calls:** if a dialer is connected, the same approach works for cold calls: opener, where "not interested" calls go sideways, and turning "send me info" into a set time.
- **Check-ins:** if the user asks you to keep an eye on their day, schedule a review a few minutes after each demo ends on their calendar.