# Opportunity Solution Tree — Desk Wellness Nudge App

**Outcome:** 8 out of 10 desk workers take a movement break within 60 minutes of continuous sitting, outside their protected deep-work windows (identified via a short onboarding survey, updated weekly). Even inside deep-work windows, routine nudges are suppressed but a rare, minimal signal can still fire if sitting time crosses a significant threshold.

---

## Three themes, not seven lines

The original opportunity-mining pass (5 initial interviews: Sushant, Karishma, Sachin, Triveni, Archana) produced 7 opportunity lines. On review, several were the same underlying problem surfacing in different body parts or moments — not genuinely distinct opportunities. Collapsed to three themes:

### Theme 1 — Delayed Bodily Awareness
*Merges: sitting too long unnoticed, eye strain, forgotten hydration, posture/stretch neglect.*

All four are one root cause — focused work suppresses the body's internal signal until it's already a problem — surfacing in different body systems (back, eyes, hydration, posture).

> Sushant: *"I got headache & even pain in upper back while sitting continuously that day."*
> Karishma: *"My eyes feels like warmest part of the body."*
> Triveni: *"I check my bottle in the evening and realise I didn't drink."*

**Field-test evidence:** every nudge sent across all 6 live-test participants addressed some combination of these four, and no one ever objected to the *category* of nudge (move / hydrate / eyes / posture) — only to its timing or delivery. That confirms these four lines were one problem, not four.

### Theme 2 — Context Lock-Out
*Was: "When I'm on calls, it's not my call to get up."*

Structurally different from Theme 1 — not about failing to notice the need, but being unable to act on a need that is already known, because the person doesn't control their own schedule in that moment.

> Karishma, original interview: *"When you're on continuous calls back to back, it's not your call to get up."*

**Field-test evidence:** Karishma's Nudge 1 (12:16 PM) and catch-up Nudge 2 (1:05 PM) both failed for the identical, stated reason — *"I have back to back calls till 1pm,"* later confirmed as *"No I was continuously sitting on a call."* Two failures, one root cause, live in the test — which directly forced a mid-test design change (see `observation-log.md`).

### Theme 3 — Autonomy & Trust in the Nudge
*Merges: "feels like a manager checking on me" + "I know what I should do but can't follow through consistently."*

These look different on paper but are the same failure mode expressed two ways — loudly (explicit rejection) and quietly (fatigue/inconsistent follow-through).

> Sushant: *"If app which is already there have regular notification pattern then it seems like a manager checking my progress."*
> Archana: *"I would probably stop using it if I wasn't able to follow it thoroughly."*

**Field-test evidence — loud version:** Vandita, Day 0: *"I take breaks when I feel like it, instead of waiting for some application to tell me that break lelo."* Her compliance then fell from 80% (Day 1) to 0% by Day 3 — confirming, in real behavior, exactly what she predicted about herself.
**Field-test evidence — quiet version:** Sushant's evening nudges consistently got delayed, bundled, or ambiguous replies compared to sharp same-minute reactions earlier in the day — the same erosion of engagement, expressed as fatigue rather than rejection.

**Why this collapse matters:** the original 7 lines were organised by *what* the problem was about (body part, delivery mechanic). These 3 themes are organised by *why* they happen — which is what tells you what to build. Theme 1 is the core feature (a sensing/timing engine). Theme 2 is a hard constraint that engine must respect (check call/meeting status before nudging). Theme 3 is a design principle governing every nudge sent, not a separate feature.

---

## Top opportunity, laddered

**Top opportunity** (highest score on How many / How often / How much / Can you reach them — see original scoring):

> "I don't realize I've been sitting too long until my body starts hurting."

**Why #1 — Why doesn't the person notice they've sat too long?**
Because during deep, uninterrupted focus work, attention is fully consumed by the task, so low-grade bodily signals get deprioritised rather than acted on.

**Why #2 — Why does focus work override the signal to the point of real pain, not just minor discomfort?**
Because these focus stretches are tied to external pressure — a deadline, a report owed to leadership, a schedule of calls set by other people — so stopping doesn't feel optional. The person keeps pushing through minor signals because pausing feels costlier than the discomfort, until the signal crosses a pain threshold that can no longer be ignored.

**Why #3 — When exactly does this happen? (Not "always" — a specific moment)**
It concentrates at the tail end of an unbroken 2+ hour stretch of deadline-driven or back-to-back-call work — specifically on high-meeting-load or pre-deadline days, not on an ordinary day with natural breaks between tasks. Three pieces of evidence pin this to a moment rather than a generality:

- Sushant's own account of a 9:30 PM–3 AM continuous stretch for a report due to leadership — pain arrived only once the stretch was unbroken and deadline-bound, not on his typical evenings.
- Karishma's live test failure at exactly her back-to-back call block (till 1 PM) — the moment calls end and she's finally free is precisely when the earlier missed signal compounds.
- Archana's complete silence across all 6 nudges on Day 1 (9 AM–7 PM) — total absence of response suggests one continuous, unbroken state for the whole day, unlike days with natural meeting-driven transitions where the same person does engage.

**Answer to "when":** not every day, and not constantly — it is the closing stretch of an unbroken, externally-pressured focus block (a deadline push or a back-to-back call sequence), most often in the final hour before that block ends.

---

## Solutions (branching from the top opportunity only — breadth at Level 2, depth here)

| # | Solution | Directly addresses |
|---|---|---|
| 1 | Sitting-duration detection engine — fires once continuous sitting crosses ~60 min | Theme 1 |
| 2 | Calendar / call-status check before every nudge — suppress during deep-work or active-call state | Theme 2 |
| 3 | Seated / on-call fallback nudges (stretch options that don't require leaving the desk or being visibly "away") | Theme 2 |
| 4 | Variable, non-repeating nudge phrasing; question-framed, never command-framed | Theme 3 |
| 5 | User-adjustable frequency / a self-reporting "check in with me at end of day" mode | Theme 3 |

## Assumption tests run so far

A 4-day, 6-person manual WhatsApp field test (no build, no spend) — full raw log in `observation-log.md`. Headline: 123 nudges sent, 74 acted on (60% compliance), with the pattern of successes and failures mapping directly onto the three themes above.
