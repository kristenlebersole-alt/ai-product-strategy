# Three-Horizon Roadmap & Board Pitch

## Roadmap

### Horizon 1 — Now (0-3 months)
*Quick wins. Ship with existing capabilities.*

| Initiative | Metric | Confidence |
|-----------|--------|-----------|
| | | H / M / L |
| | | H / M / L |

Horizon 1, Ship (0–4 weeks)
Initiative	Strategy Component	Why it ships now	Confidence
PDF to AI Reader using contract examples	Bet	This is the core archetype ("Automator... extractor into a rules engine template") and you already have pilot validation — it's execution, not a new bet	H
Create Airline Rules Database structure	Bet	Directly named in your AI Value Archetype definition; without this the rules engine has nowhere to write to — foundational, not exploratory	H
Mapping Data Metrics used in Contracts to Database outputs	Contract	This is the schema work that defines what "correct" extraction looks like — it's literally your currently-blank Golden Dataset field	H
Develop Upload UI	Bet	Table-stakes product surface, no open hypothesis to test	H
Develop UI for Rules Manual Modification	Contract	This is your HITL Architecture and Confidence UX made real (Green/Yellow/Red review, rule editing) — already fully specified in your strategy, just needs building	H
Connect to Testing Data set for Performance Analysis	Contract	Directly closes the "Failure Mode Coverage" gap you flagged as unanswered — this should be treated as urgent infrastructure, not a nice-to-have	H

### Horizon 2 — Next (3-9 months)
*Bets. Requires new capabilities or integrations.*

| Initiative | Metric | Confidence |
|-----------|--------|-----------|
| | | H / M / L |
| | | H / M / L |

Initiative	Strategy Component	Hypothesis	Kill Criteria	Confidence
API to AI Reader	Margin (Moat tension — see below)	Larger accounts will pay a premium for programmatic access, expanding revenue beyond seat pricing	If we don't see a paying customer or signed intent for API access by week 8, we stop	M
Pilot with 2-3 Customers, Airline and Agency spread	Bet / Moat	Contracts across airline and agency customers share enough structure that cross-customer data compounds and measurably reduces hallucination rate — this is the exact mechanism you named as your updated Top Risk defense	If cross-customer piloting doesn't show a measurable reliability improvement (or hold ≥90% extraction accuracy) across at least 2 distinct customer contract types by week 10, we stop treating cross-contract compounding as the moat	M

### Horizon 3 — Bet (9-18 months)
*Moonshots. High uncertainty, high potential.*

| Initiative | Metric | Confidence |
|-----------|--------|-----------|
| | | H / M / L |

Horizon 3, Explore (3–6 months)
Initiative	Strategy Component	What must be true first	Confidence
Add in Natural Language Report generation for QBR processing	Moat	Demand signal today is thin ($100/mo spend in your own shadow audit) — needs the pilot (H2) to surface whether QBR reporting is a genuine workflow-lock-in point or a nice-to-have	L

## Board Pitch

**Thesis (1 sentence):**

**The case:**
1. Why now:
2. What's defensible:
3. The economics:

**The risks:**
1. Trust / failure modes:
2. Scale / governance:
3. Competitive:

**The ask:**

Thesis (1 sentence):
We turn messy, high-stakes airline and agency commission contracts into a trusted, structured rules database automatically, so customers stop manually re-keying contract terms and start using that data to run negotiations and QBRs.

The case:

Why now: Commission and interline contracts are re-negotiated constantly and manually re-keyed today — our own pilot customer confirms this is active, paid-for pain (their shadow spend shows $4,000/month on contract scenario negotiation work and $1,000/month on contract development, both already flagged internally as "Build" priorities). The extraction technology has just crossed the reliability threshold where this is buildable at 90% accuracy in a pilot — that threshold didn't exist 12-18 months ago. And the window is closing: platform players are moving toward generic document extraction, so the advantage is in moving now, not in the technology itself.
What's defensible: I'll be direct — today, it isn't defensible yet, and I'm not going to pretend otherwise. Our Data Flywheel score is 12/20, and our Encroachment Defense against Adobe, OpenAI, or Google shipping this as a feature is currently an open question, not an answer. The moat we're betting we can build is cross-customer compounding: contracts across multiple airline and agency customers share enough structure that pooled data reduces hallucination rates and gets harder to replicate the more customers we onboard. That's a hypothesis, not a proof point yet — which is exactly what this POC is designed to test.
The economics: At $50/user with $10/user AI cost, we're at 71.4% gross margin on paper. I want to flag two open items rather than paper over them: pricing model is still undecided across four options (seat, usage, outcome, hybrid), and the $3M net margin shift we're projecting has no stated baseline, so I can't yet defend that number under scrutiny. Both need to be resolved before this scales past POC.

The risks:

Trust / failure modes: Our reliability target is 90%, and the failure mode that would put us on the front page is a misread contract term producing a wrong commission payment or missed liability clause. The catch: every extracted rule is scored Green/Yellow/Red at parse time, and Yellow/Red require human review before a rule goes live — nothing auto-applies at low confidence. What I can't yet tell you is our tested failure mode coverage; that field in our own strategy is still blank. That's a real gap, not a rounding error, and closing it is one of the three H1 initiatives already in motion.
Scale / governance: We have real guardrails — daily audit of golden dataset changes, weekly error rate review, hard escalation triggers on PII/PCI exposure and token overuse. One internal tension worth surfacing: we've drawn a boundary of "not shipping agents," but our own shadow AI audit shows customers already spending real money on agent-shaped work (contract scenario negotiation, $4,000/month). That's either a deliberate risk boundary given the legal stakes, or it's leaving demand on the table — I don't think we can answer that definitively until after the POC.
Competitive: The scenario that kills this is if a platform player ships equivalent contract extraction natively within the pilot window, or if our cross-customer compounding hypothesis fails to move the reliability needle. Concretely: if piloting across 2+ distinct customer contract types doesn't show measurable accuracy improvement from pooled data by week 10, we stop treating cross-contract compounding as our moat and go back to the drawing board on defensibility.

The ask:
$1M and 7 headcount (PM, Product Owner, SE, 2 DE, 2 QE, 1 Analyst) over 3 months to land one development partner airline or agency, build the rules database against real contracts, and prove out QBR-ready output. The decision gate is partner commitment plus POC completion — this is what earns the right to go pursue additional pilot customers. What this pauses elsewhere in the portfolio isn't specified in the strategy as written, and that's the first question this room will ask — worth having a real answer before you walk in, not just "trust me."

Opening line (literally say this first): "We can turn a customer's commission contracts into a trusted database automatically — the question in front of you isn't whether the technology works, it's whether we can prove it compounds before someone else ships the same thing."
If you only get 60 seconds: We turn manually re-keyed airline and agency contracts into a trusted, automated rules database. The real risk is that our defensibility is unproven — we're betting cross-customer data compounding creates a moat platforms can't easily copy, and this POC is how we test that. We're asking for $1M and 7 people over 3 months to land one development partner and prove it out before scaling further.
The one question they'll ask first: "What stops Adobe or OpenAI from shipping this exact capability in 12 months?" Honest answer that holds up: nothing stops them from shipping generic contract extraction — what we're betting on, and what this POC specifically tests, is whether pooled data across multiple airline and agency contracts creates a reliability edge and workflow lock-in that a generic reader can't match on day one; if the pilot doesn't show that by week 10, we treat it as disproven and don't scale past this POC.

## M1 Baseline vs. Now
*Your 3-sentence AI strategy from Module 1 vs. what you'd say now:*

**M1 baseline:**
Business Strategy --> Conservative Approach, start with using AI for own productivity, for product move lightly, (embed into current products) to develop with and into our products. We are focused on taking care to protect our data and our IP, but using AI to extrapolate and identify data trends. Use it as a differentiator and part of a larger product platform strategy. 

Product Strategy Use AI to enhance current products by providing features and functionality that helps identify and get data insights quicker. Also use the AI to fill in the gaps of missing reference data that is publicly available.

**Now:**
We use AI to extract additional value and create additional competitive differentiation for our data products and additional data extraction from complex sources. Utilize AI with human guardrails and oversight to ensure quality and trust with customers. Start small with iterative POC to Pilot to Customer to ensure cost effective and governance measures that align to our mission of being the "trusted source of airline intelligence",
