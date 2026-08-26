**Idea Alignment Document**

**Product Name:**

Breaksy - Care That Doesn't Break the Flow.

**Author:**

Rishu Kumar

**Date:**

23 Aug 2026 |V1

**Cohort:**

Upivot Pro Phase B · \[Batch 1\]

**Presented to:**

Upivot Pro cohort + Abhik

**SECTION 1 · THE OPPORTUNITY**

**Problem / Opportunity Identified:**

Desk-based knowledge workers often know they need to move, hydrate, and rest their eyes, but struggle to turn this awareness into action during the workday.  
Two key barriers stand in the way. First, meetings, deadlines, and periods of deep focus rarely provide clear or natural moments to take a wellness break. Second, workplace culture can make taking a break feel like a sign of low commitment or poor work ethic.  
As a result, workers often suppress these basic wellness needs and continue working until physical discomfort becomes strong enough to force them to stop. This means wellness breaks happen reactively, rather than as small, preventive actions integrated into the workday.

**Why This Could Be Valuable:**

Breaksy can help busy professionals build healthier workday habits through small, achievable actions that fit naturally into their existing routines. It addresses a specific everyday problem by helping people overcome both the practical and cultural barriers to taking wellness breaks without requiring major changes to how they work. With a lightweight MVP, Breaksy has strong potential as a portfolio project and could grow into personalized and workplace wellness solutions.

**Why Explore Now:**

Current work routines are increasingly screen-based, and with hybrid work, many professionals spend long hours sitting and working, often without a clear break between tasks. Even for people who exercise regularly, there is still a need for simple wellness habits throughout the workday for making small movement, posture, hydration, and eye break easier to build into everyday routines. With technology now making context-aware and personalized reminders more practical, this is a good time to explore a simple solution that fits wellness into the way people already work.

**SECTION 2 · THE 5 WHYs — ROOT CAUSE ANALYSIS**

_Take the surface problem your users complained about. Ask WHY 5 times. Each Why goes one level deeper toward the ROOT cause. Most PMs solve the surface problem — root cause solutions have durability._

| **Level**   | **Question**                      | **Answer / Insight**                                                                                                                                                                                                                                                                              |
| ----------- | --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Surface** | _What did the user actually say?_ | \["High-priority work didn't allow me to take breaks — a break would've broken my flow." — Sushant\]                                                                                                                                                                                              |
| **Why 1**   | _Why does the user say this?_     | \[Because taking a break can interrupt deep focus, task continuity, or productivity, especially when the work is high priority or deadline-driven.\]                                                                                                                                              |
| **Why 2**   | _Why does THAT happen?_           | \[Because users often decide that finishing the task is more important than taking care of themselves at that moment. Breaks become something they will do _after_ the work is completed.\]                                                                                                       |
| **Why 3**   | _Why does THAT happen?_           | \[Because workdays contain deadlines, long analytical tasks, back-to-back meetings, and external requests, which make break timing difficult to control. Karishma explicitly said that when calls are back-to-back, "it's not your call to get up." \]                                            |
| **Why 4**   | _Why does THAT happen?_           | \[Existing break-reminder approaches often rely on fixed timing, while users' ability to take a break depends on their actual work context. Triveni's earlier timer also became socially uncomfortable because colleagues noticed and mocked the visible reminders.\]                             |
| **Why 5 ★** | _Why does THAT happen?_           | **\[Because the real problem is not lack of awareness. The user's work environment determines whether a healthy action is actually feasible at that moment. The current solutions don't understand the user's work context, so users either ignore them or don't have the opportunity to act.\]** |

**Root Cause Statement:**

Desk-based knowledge workers lack a reliable way to identify when they can act on their wellbeing without disrupting their work or feeling socially/workplace pressure to stay engaged.

**SECTION 3 · SUPPORTING EVIDENCE**

**User Interviews Conducted:**

5 interviews with desk-based knowledge workers across hybrid/office work environments — Sachin, Triveni, Karishma, Sushant and Archana.

**Common Themes (3-5 patterns across interviews):**

• **Work context overrides planned breaks — 5/5 users:** Deep work, deadlines, meetings and workload make it difficult to step away.  
• **Physical/visual discomfort from prolonged work — 5/5 users:** Users reported combinations of back/neck/foot discomfort, tired eyes, headaches, fatigue or burnout.  
• **Awareness isn't the core problem — 5/5 users:** Users already know they should move, stretch, hydrate or rest their eyes, but struggle to act consistently during work.

• **Reminders can conflict with work — 4/5 users:** Fixed notifications can interrupt focus, meetings or productivity.

• **Movement and visual recovery are stronger opportunities than hydration — 5/5 users:** Movement and eye comfort repeatedly emerged as meaningful problems, while hydration was more variable.

**Anchor Quotes (3-5 verbatim from your interviews):**

• **"I had high-priority work on my plate which didn't allow me to take breaks. I think break would have broken my flow."** — Sushant, high-priority analytical work  
• **"When you're on continuous calls, it's not your call to get up."** — Karishma, back-to-back meetings  
• **"It feels like we're being selfish if we take care of ourselves during work hours."** — Triveni, workplace culture

• **"It would feel like at least I am able to focus on my body as well while working on critical project tasks that do not get impacted."** — Archana, product concept reaction

**Market Signals (data supporting the opportunity):**

• **Large opportunity:** Extended sedentary and screen-based work creates an ongoing need for movement and visual recovery during the workday.

• **Competitive gap:** Existing solutions tend to focus on individual behaviours or fixed reminders rather than understanding whether the user is actually available for a break.

• **Product opportunity:** A context-aware approach could combine movement, visual recovery and other micro-wellness actions while minimizing unnecessary interruptions.  
<br/>• **Workplace acceptance is a key adoption factor:** Employees may be more likely to use Breaksy if it is perceived as supporting productivity and wellbeing rather than monitoring or interrupting work.

**JTBD Statement (from Week 1):**

"When I'm deep in a task, back-to-back in meetings, or racing a deadline, I want to look after my body and eyes without disrupting my flow or appearing less committed, but I don't have a way to know when work truly allows a break or whether it's socially safe to take one so I keep pushing through until my body forces the stop — evidenced by all 5 interviews with desk-based knowledge workers. "  
<br/>

**SECTION 4 · AI DISCOVERY VERDICT**

**Test 1 — Is your core feature AI-worthy? (4 criteria):**

• C (Complexity) — \[**PASS.** Personalizing break suggestions based on the user's focus periods, meetings, deadlines, preferences, and past behaviour becomes complex as more context is involved. For the MVP, however, simple rules can handle the initial version.\]  
• S (Scale) — \[**PASS.** The check-in happens daily for each active user. Even with 1,000 users, Breaksy could process thousands of daily schedules and break interactions, creating meaningful opportunities for personalization.\]  
• D (Data) — \[**PASS.** Breaksy can use user-provided focus hours, meetings, deadlines, break preferences, and behavioural data such as accepted, skipped, or postponed break suggestions. This data can later be used to learn individual patterns.\]  
• V (Value) — \[**PASS.** Metric that moves: break adherence and user engagement — whether users accept useful break suggestions rather than ignoring them. Target: >60% acceptance of contextually relevant break suggestions.\]

**Test 2 — What kind of AI?**

\[Start with rules-based logic for the MVP, then introduce ML as enough usage data becomes available to personalize break timing.  
The first version should use rules because users explicitly provide their focus times, meetings, and important events, making prediction unnecessary.  
Later, ML can learn recurring patterns and personalize suggestions based on behaviour.  
An LLM is not the core requirement because the main problem is scheduling and personalization, not generating text.\]

**Test 3 — Human-in-the-loop mode?**

B: AI Suggests + Human Decides. Breaksy should suggest the right moment and action, while the user decides whether to accept, postpone or skip it; if AI gets the timing wrong, the consequence should be a minor interruption rather than an enforced action.

**Overall, AI Verdict:**

Build the MVP with rules-based context detection and user preferences first; introduce ML in V2.  
The core MVP should start with a quick daily check-in, reuse the previous day's schedule, and apply rules-based suggestions. Once enough behavioural data is collected, ML can be introduced to learn the user's patterns and make break recommendations more personalized.

**SECTION 5 · THE 10-WEEK PLAN**

**Weeks 3-4 (Architecture + UX):**

Wireframes for 3 core flows: morning check-in · today's schedule · context-aware break suggestion. Lock the MVP architecture around a simple rules-based engine, with user preferences and daily schedule stored for reuse.

**Weeks 5-8 (Build v1 — Alpha):**

Build the working web app with onboarding, daily check-in, "Same as yesterday" flow, focus/meeting blocks, and break suggestions. Alpha should work end-to-end for a small set of internal users.

**Weeks 9-12 (Beta + iteration):**

Test with 5-10 real users for at least 2 weeks. Use feedback and usage data - accepted, skipped, or postponed breaks—to improve suggestion timing, check-in friction, and personalization.

**Weeks 13-15 (Launch prep):**

Polish onboarding, landing page, break suggestion experience, and product messaging. Prepare a simple demo, documentation, analytics, and launch content.

**Week 16 (Public launch):**

Launch publicly through LinkedIn, Product Hunt/community channels, and personal networks. Target the first 10 active users and use their early feedback to validate whether Breaksy is worth continuing and personalizing with ML.

**SECTION 6 · DECISION CRITERIA**

**Success Criteria (what validates this by Week 16?):**

• **10+ real users** use Breaksy at least 3 times per week for 2 consecutive weeks.

• **60%+ of relevant break suggestions** are accepted or acted upon, showing that suggestions are useful rather than disruptive.

• **80%+ of beta users** say suggestions feel discreet and socially comfortable to use in their workplace.

**Failure Criteria (when would you pivot?):**

• After 5-10 beta users, **fewer than 2 users return and use Breaksy regularly** after the first week.

• **Less than 30% of break suggestions are acted upon**, suggesting that users don't find the recommendations useful or the timing is wrong.

• Beta users consistently say that **taking breaks is not a meaningful problem for them, or that Breaksy feels awkward to use at work**, indicating that the problem or solution needs to change.

**SECTION 7 · THE COMMITMENT**

**One-line Product Statement:**

" Breaksy is a discreet, context-aware break companion for knowledge workers to take healthier breaks without disrupting their focus or feeling unproductive at work."

**North Star Metric for Week 16:**

Weekly Active Users who accept at least one Breaksy suggestion per week - target: 10+ users.

**What I'm NOT Building (3 things max — discipline signal):**

• **A loud timer or visible workplace interruption tool** — because users like Triveni may avoid using break tools if they feel mocked or judged by colleagues. Breaksy suggestions should be discreet and professionally framed.

• **Automatic calendar surveillance or deep-work detection** — Breaksy will initially ask users about their day rather than trying to infer everything from their activity.

• **An AI therapist, health coach, or medical tool** — the product focuses on practical workplace break behaviour, not clinical or mental-health advice.

**★ SIGN + SEAL**

This is what I'm building for the next 10 weeks.
Signed: Sneha Patel · Date: 15 Aug 2026 · Presented to: Upivot Pro Batch 1 + Abhik

