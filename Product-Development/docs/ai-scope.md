# AI Scope Statement — Desk Wellness Nudge App (Simple Version)

## The one-line summary

> Out of 6 parts of this product, only **1 needs AI** (reading messy replies like "Done" or "No"). The other 5 are simple rules or fixed content — no AI needed, and adding AI would only make them harder to trust.

## Quick answer table

| # | Part of the product | Needs AI? | What runs it | Who's in control |
|---|---|---|---|---|
| 1 | Sitting-duration timer | No | A simple clock | **A** — runs on its own |
| 2 | Checks if you're on a call/in focus mode | No | Calendar lookup | **A** — runs on its own (you can correct it if wrong) |
| 3 | Seated stretch suggestions | No | A fixed list | **A** — runs on its own |
| 4 | Nudge wording | No | A fixed list, rotated | **A** — runs on its own (a person wrote & approved the list once) |
| 5 | Reading your reply ("Done," "No," etc.) | **Yes** | Lightweight AI (LLM) | **B** — AI decides the easy ones, a person checks the confusing ones |
| 6 | Learning your ideal nudge frequency | Not yet | (Future: simple ML) | **B** — AI would suggest, you'd approve — nothing auto-changes |

**A** = runs by itself, no person checks it in the moment. **B** = AI makes a call, but a person reviews the unclear ones (or approves before it takes effect).

---

## Why only 1 out of 6 needs AI

If you ask "is my whole product AI?" the answer is always yes — because that's what you want to hear. Asking about each piece on its own instead gives honest answers, and most pieces turn out not to need AI at all.

---

## Each part, explained simply

**1. Sitting-duration timer** — Just counts minutes since your last break. A stopwatch doesn't need to be smart.

**2. Call/focus-time check** — Looks at your calendar to see if you're busy. This is a lookup, not a guess — no AI needed.

**3. Seated stretch suggestions** — A short list of stretches you can do without leaving your chair (this is what worked for Karishma in the test). Just picks one from the list.

**4. Nudge wording** — The message you get ("Quick stretch?"). It just needs to not repeat itself and not sound bossy — a rotating list of pre-written lines does this fine.

**5. Reading your reply** — This is the one that actually needs AI. People reply in all kinds of ways — "Done," "No," "Having lunch," or messages that only make sense with context. A simple keyword rule can't handle that, but the AI doesn't have to guess alone: if it's confident, it decides; if the reply is genuinely unclear, a real person looks at it — the same way you personally judged the tricky replies during the manual test.

**6. Learning your ideal frequency** — Not built yet. There's a real pattern here (some people wanted more nudges, some wanted almost none) but 6 people over 4 days isn't enough data to trust a model with it yet. When it is built, it will only ever suggest a change — you'd have to approve it, never automatic.

---

## The one AI part, in plain terms

- **What it does:** reads your reply and figures out if you actually took the break.
- **When it's confident:** it just logs the answer — no delay.
- **When it's not confident:** it flags the reply for a person to check, instead of guessing.
- **Why this matters:** during the manual test, about 1 in 8 replies were genuinely hard to read even for a human. The AI should treat those the same way — hand them off, not fake confidence.
