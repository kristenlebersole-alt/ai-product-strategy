# Three-Horizon Roadmap & Board Pitch

## Roadmap

### Horizon 1 — Now (0-3 months)
*Quick wins. Ship with existing capabilities.*

| Initiative | Metric | Confidence | Why it Ships Now |
|-----------|--------|-----------|--------------------|
| PDF to AI Reader using contract examples | Bet | H | Core archetype, already pilot-validated — execution, not exploration |
| Create Airline Rules Database structure	| Bet| H | Named directly in your AI Value Archetype; the rules engine has nowhere to write without it |
| Mapping Data Metrics used in Contracts to Database outputs	| Contract| H | This is the schema that defines "correct" output — closes your currently-blank Golden Dataset field |
| Develop Upload UI	| Bet| H | Table-stakes surface, no open hypothesis |
| Develop UI for Rules Manual Modification	| Contract| H | Builds the HITL/Confidence UX (Green/Yellow/Red review) you've already fully specified |
| Connect to Testing Data set for Performance Analysis	| Contract| H | Directly closes your flagged-open Failure Mode Coverage gap |
| Integrate Visual UI Dashboards (Discovery Point)	| Contract| H | Extension of the Confidence UX spec, and matches a live shadow-AI "Build" signal (Visualizations and Reports) |
| Integrate Report and Analysis storage	| Guradrails| H | Required infra for your own Data Retention escalation trigger (1-year rule) and Governance Posture scope, which already names "Databases" in-scope |
| Develop Initial User Guardrails | Guardrails | M | Required Infrastructure for User AI Decision Making |
| Develop Automated AI Triggers for Cost, Usage, Quality Decgridation | Governance | H | Initial reporting to track ad account for Kill Criteria |



### Horizon 2 — Next (3-9 months)
*Bets. Requires new capabilities or integrations.*

| Initiative | Metric | Confidence | Hypothesis |
|-----------|--------|-----------|
| API to AI Reader | Margin | M | Secondary Delivery Method for Contracts; Larger accounts will pay a premium for programmatic access, expanding revenue beyond seat pricing | 
| Pilot with 2-3 Customers, Airline and Agency spread | Bet/Moat | M | Contract Variation, Compounding Effect; 	Contracts across airline and agency customers share enough structure that cross-customer data compounds and measurably reduces hallucination rate — this is the exact mechanism you named as your updated Top Risk defense | 

### Horizon 3 — Bet (9-18 months)
*Moonshots. High uncertainty, high potential.*

| Initiative | Metric | Confidence | What must be true first |
|-----------|--------|-----------|-----------|
| Add in Natural Language Report generation for QBR processing | Moat| L | 	Demand signal today is thin ($100/mo spend in your own shadow audit) — needs the pilot (H2) to surface whether QBR reporting is a genuine workflow-lock-in point or a nice-to-have|

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
