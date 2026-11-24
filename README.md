# Demo Call Grader

A Claude skill that grades your recorded SaaS sales demos and discovery calls.

You get:

- A letter grade for each call (A to D)
- Timestamped wins with verbatim quotes
- The #1 fix, with the exact words to say next time
- A weekly scorecard when you grade several calls

Works with Fathom, Gong, Chorus, Fireflies, Zoom, Google Meet, Avoma, Nooks and Claude Meetings, or a pasted transcript.

## What it grades

12 habits that win demos, including:

- Setting time and agenda expectations up front
- Qualifying fit before demoing
- Discovery before sharing your screen
- Pricing the pain in dollars
- Labeling objections (Chris Voss tactical empathy)
- Booking the next step on the calendar before the call ends

The full rubric is in [SKILL.md](SKILL.md).

## Install

**Claude app (claude.ai or desktop)**

1. Click the green **Code** button on this page, then **Download ZIP**.
2. In Claude, open **Settings**, find the **Skills** section, and upload the ZIP.

**Claude Code**

```
git clone https://github.com/daviddoestech/Demo-Call-Grader.git ~/.claude/skills/demo-call-grader
```

## Use it

Connect your call recorder to Claude, then ask:

- "Grade my latest demo"
- "Grade all my demos from this week"
- "Review this call: [link or pasted transcript]"

On first use, Claude asks what you sell, your ideal customer, pricing, and the 1 or 2 habits you are working on, so grades fit your business.

## Author

Built by David Fantin.
