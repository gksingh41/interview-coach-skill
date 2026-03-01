# Gaurav Kumar — Interview Story Reference Card
Last updated: 2026-02-28

---

## Quick Reference: Which Story Answers Which Question

| Question Type | Use This Story |
|---------------|---------------|
| Cost reduction / operational problem at scale | S001 |
| Retention / changing user behavior / data-driven | S002 |
| Cross-functional leadership / marketplace scaling | S003 |
| 0→1 product / ambiguity / go-to-market | S004 |
| Internal tools / multiplying team output / platform | S005 |
| Failure / wrong bet / learning / AI experience | S007 |
| Metrics / trade-offs | S001, S002, S003 |
| Stakeholder management | S003, S005 |
| Product strategy / prioritization | S002, S005 |
| Technical depth | S001, S003, S007 |

---

## S001 — Support Automation ($1.2M)

**Earned Secret:** Automation had to earn trust by solving problems before we could use it to deflect volume.

**Deliver it like this:**
> "At Rapido we had a serious cost problem. Support calls were running at 4.9 per 100 completed orders — across 2.7 million drivers, that was roughly 1.5 million calls a month. We were chasing profitability and this was one of the biggest cost lines to attack.
>
> My job was to bring that ratio down without breaking driver trust — and that second part was the real constraint. Our drivers are often semi-literate, prefer regional languages, and deeply trust phone calls because they've always been able to talk to a human. If we just built a bot and blocked calls, we'd destroy CSAT and churn supply.
>
> So the approach was: solve the problem first, then reduce the call. I built a multi-layered system — IVR for the most common, repetitive issues, rule-based chatbots for structured resolution, in-app self-serve flows, and agent-assist tools so when calls did happen, they resolved faster. The key design decision was sequencing: automation had to earn trust by actually solving problems before we gated the call option behind it.
>
> Over 18 months, we brought the contact ratio from 4.9 down to 2.2 per 100 orders — a $1.2M annual saving. CSAT held. That's the part I'm most proud of — we deflected volume without breaking the relationship with drivers."

**Use for questions like:**
- "Tell me about a time you solved a complex operational problem at scale"
- "Tell me about a time you reduced costs significantly"
- "How do you approach trade-off decisions?"
- "Tell me about a multi-layered system you built"
- "Tell me about balancing automation with user trust"

---

## S002 — BYOB Earning Models

**Earned Secret:** Even three options can overwhelm a driver who isn't financially literate — so we used their own earning data to turn a confusing choice into a personalized nudge.

**Deliver it like this:**
> "Driver retention at Rapido was hurting, and the data kept pointing to the same root cause — earnings unpredictability. Surveys, in-app feedback, and churn cohort analysis all said the same thing: drivers didn't feel in control of what they'd earn.
>
> The underlying problem was structural. Rapido had a single commission model for everyone — but our driver base was split between full-timers who could make up volatility through incentives, and part-timers who couldn't. For a driver doing 3 days a week, one bad day wiped out their week. The default model was built for full-timers and was silently churning everyone else.
>
> So we built BYOB — Build Your Own Bundle. Three earning models: fixed commission per order, fixed earnings per KM, and a minimum guarantee model for drivers who wanted salary-style predictability. We also built explainer videos and audio in regional languages so drivers could actually understand what they were choosing.
>
> But the more interesting design challenge was choice paralysis. Even three options can overwhelm a driver who's not financially literate. So we layered in persona-based recommendations — using each driver's own earning pattern to suggest the right model for them. Instead of three options, most drivers saw 'based on how you drive, this plan fits you best.'
>
> The result: 60% of drivers migrated off the default commission model. Net active days went from 8 to 10, rides per active day increased 25%. The part-timers who were quietly churning started staying."

**Use for questions like:**
- "Tell me about a time you improved user retention using data"
- "Tell me about a time you changed user behavior at scale"
- "How do you design for diverse user segments?"
- "Tell me about a trade-off you navigated"
- "Tell me about a data-driven product decision"

---

## S003 — Auto Vertical Expansion

**Earned Secret:** Captain-friendly and captain-advantageous aren't always the same thing. The feature that felt worse in the moment gave captains more earning opportunities overall. We had to help them experience it before they'd believe it.

**Deliver it like this:**
> "When Rapido's Auto vertical was early-stage, we had a core marketplace problem — low supply and low demand feeding each other in a negative loop. And our dispatch model was making it worse.
>
> We were running unicast — one order to one captain at a time. Captains could read the order, think about it, and accept. Very captain-friendly. But in a low-density market, this was killing acceptance rates because orders would time out while captains deliberated. Riders weren't getting matched, captains weren't earning, and both sides were losing trust in the platform.
>
> The solution was multicast — send one order to multiple captains simultaneously, first to accept wins. But this created a real cross-functional problem: ops was worried it would churn supply. Captains were already fragile on this vertical. If they started losing orders they wanted to accept because someone else was faster, they'd feel the platform was unfair and leave. Dispatch was also owned by a separate marketplace team, so I had to partner closely with their PM and engineers to understand the existing logic before touching it.
>
> The design insight that unlocked this was small but critical: we delayed the accept button by a few seconds — giving captains time to read the order before the race started. That one change reduced the 'I wanted that order' frustration significantly and made the feature feel fair rather than predatory.
>
> We piloted in one small city, tracked captain VoC closely alongside supply metrics, got signal that acceptance was improving without churn spiking, then scaled to 30 cities. The result: 20% increase in order pings per captain, 12% increase in net rides. Captains were getting more earning opportunities — the feature that seemed less captain-friendly was actually more captain-advantageous."

**Use for questions like:**
- "Tell me about a complex cross-functional initiative you led"
- "Tell me about a time you scaled a marketplace"
- "Tell me about a complex technical-product decision"
- "Tell me about a time you had to align multiple teams"
- "Tell me about a product that drove significant business impact"

---

## S004 — Rapido Hire (0→1)

**Earned Secret:** For a new product category, the hardest failure mode isn't adoption — it's the moment of first use, when both sides revert to familiar behavior. You have to intercept with education before the trip starts, not after it goes wrong.

**Deliver it like this:**
> "During Covid, we noticed something interesting in our ride data — about 10% of users were booking two bike rides back to back within 80 minutes. That was a signal: these users needed a return trip or multiple stops, but had no product for it. We were selling them two on-demand rides when what they actually wanted was one captain for a few hours.
>
> I validated this before building anything. Customer calls and surveys showed 70% of these users were a 'yes' or 'maybe' for an hourly rental product. That was enough signal to run a pilot.
>
> I picked a Tier 1 city, took a cohort of these repeat bookers, and launched Rapido Hire — hourly plans customers could book upfront, one captain committed to them for the duration. The product build itself was straightforward. The hard part was the human behavior on both sides.
>
> Captains had no mental model for rental. When the first drop happened, they'd complete it and leave — exactly like any on-demand ride. The customer would have to explain 'no, I booked you for an hour, you need to stay.' That created confusion, support calls, and a broken experience.
>
> The fix was intercepting before the trip started, not after it broke. When a captain accepted a Hire order, we triggered a call explaining: this is a rental booking, the customer has booked you for X hours, you stay with them. That one intervention — pre-trip education — dramatically reduced the drop-and-leave failures. We codified it into a GTM playbook and scaled to 5 cities.
>
> Result: Rapido Hire contributed ~5% of city GMV with higher ticket sizes and more predictable earnings for captains — a product that solved a real demand gap and created a new earning model at the same time."

**Use for questions like:**
- "Tell me about a product you built from scratch"
- "Walk me through how you went from zero to launch"
- "Tell me about a time you navigated ambiguity"
- "Tell me about a go-to-market challenge"
- "Tell me about a time you had to change user behavior around a new product"

---

## S005 — Pitch Center (Internal Platform)

**Earned Secret:** I became the gatekeeper not to control the product, but to understand what would break when I removed myself. Then I baked those constraints into the self-serve tool — so governance came from the product, not from me.

**Deliver it like this:**
> "At Rapido, our captain communications were running through Clevertap — low CTR, low recall, and no persistence in the app. I built Pitch Center, an in-app comms product that dramatically improved quality — better images, persistent visibility, contextually placed. CTR improved 200%.
>
> The problem was scale. When it launched, only the product team used it. But soon ops, marketing, and city teams all wanted in. Every request meant a Jira ticket, dev effort, API calls — a 48-hour TAT for something that ops needed instantly. Ad-hoc city requests were eating into planned dev work, and a last-minute campaign meant pulling a PM and engineer away from whatever they were building.
>
> Before I built the self-serve dashboard, I spent time as the gatekeeper — manually approving every pitch before it went live. I did this deliberately to understand what would break when I removed myself.
>
> Two things broke without a gatekeeper: speed and consistency. Speed because comms is need-based — a city team launching a campaign can't wait 48 hours. Consistency because every team had different design instincts, and without standards, the in-app experience would become noise.
>
> So I built both constraints into the self-serve tool. Pre-built standardized templates by comms type — so teams couldn't go off-brand even if they wanted to. And instant deployment to any city without any engineering involvement. Governance baked into the product, not enforced by a person.
>
> Result: TAT dropped from 48 hours to instant. 40% of all captain communications are now launched through the platform without any PM or dev time. The city teams that used to flood my Slack are now fully self-sufficient."

**Use for questions like:**
- "Tell me about a time you multiplied team output without adding headcount"
- "Tell me about an internal tool or platform you built"
- "Tell me about a time you reduced organizational friction"
- "Tell me about a time you identified a problem proactively and solved it"
- "Tell me about a platform product and how you approached governance"

---

## S007 — Voice AI Bet That Didn't Ship (Failure/Learning)

**Earned Secret:** In AI bets, I was iterating on what was fixable and hoping the unfixable would resolve itself. Now I test the hardest constraint first. If dialect can't work, nothing else matters.

**Deliver it like this:**
> "In 2023, while working on reducing support costs, I identified that our drivers deeply preferred human interaction over bots — they trusted a voice on the other end of a call. That made me think: what if the voice was AI? A voice bot that sounded natural enough to resolve the top call reasons without a human agent.
>
> I partnered with a third party to run a PoC. We picked the highest-volume call reasons, set a clear threshold — 60% of calls handled successfully by the bot — and started testing.
>
> Over 4-5 months, we made real progress on some problems. Noise was a major blocker early — driver environments are loud, bikes running, traffic. We worked through that. But dialect never got better. India has enormous regional language variation, and the bot would lose context mid-conversation whenever drivers spoke in local dialects or mixed languages. We were hitting 40%, not 60%. We killed the project.
>
> The honest failure was that I held on longer than I should have. I kept iterating on what was fixable — noise — and betting that dialect would improve with more time. The signal that it wouldn't was visible earlier, but I was anchored on the progress we'd made.
>
> What I'd do differently: in any AI or technology bet, test the hardest constraint first, not the easiest one. Noise was an engineering problem — solvable. Dialect was a fundamental technology limitation at the time — not solvable. If I'd run a two-week feasibility sprint specifically on dialect handling before committing to a full PoC, I'd have known in week two what took us five months to confirm."

**Use for questions like:**
- "Tell me about a failure or something that didn't go as planned"
- "Tell me about a time you made a wrong bet"
- "Tell me about a time you had to kill a project"
- "What would you do differently in your career?"
- "Tell me about a time you worked with AI/ML or voice technology"
- "Tell me about a time you set a clear success threshold upfront"

---

## Pending Stories (To Be Built)

| Story | Status | Notes |
|-------|--------|-------|
| Influence without authority | ⏳ In progress | Come back when ready — prompting helps |
| AI/Gemini KYC (S006) | ⏳ Developing | Use as "current work" signal only for now |

---

## Universal Earned Secrets (memorize these)

1. **S001**: "Automation had to earn trust by solving problems before we could use it to deflect volume."
2. **S002**: "We used each captain's own earning data to turn a confusing choice into a personalized nudge."
3. **S003**: "Captain-friendly and captain-advantageous aren't always the same thing."
4. **S004**: "Intercept with education before the trip starts, not after it goes wrong."
5. **S005**: "Governance baked into the product, not enforced by a person."
6. **S007**: "Test the hardest constraint first. If dialect can't work, nothing else matters."
