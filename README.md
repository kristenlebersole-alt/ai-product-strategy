# Ai Product Strategy

> * I am building a Contract intelligence tool for Travel Agencies and Airlines that will us an AI model and data extractor to read and copy contract terms, convert into a dataet table that can be updated via a UI, and then ultimately use AI model to combine terms with our propriet…

---

## Strategy at a Glance

| Component | Module | Status | Key Artifact |
|-----------|--------|--------|-------------|
| **The Bet** | M1 | [x] | `01-the-bet/` |
| **The Moat** | M2 | [x] | `02-the-moat/` |
| **The Margin** | M3 | [x] | `03-the-margin/` |
| **The Contract** | M4 | [x] | `04-the-contract/` |
| **The Guardrails** | M5 | [x] | `05-the-guardrails/` |
| **The Pitch** | M6 | [x] | `06-the-pitch/` |

---

## The Bet (M1)

**What we're building, for whom, why now.**

- **Product:**
- **AI Value Archetype:** Automator = AI PDF reader and extractor into a rules engine template (Standard dataset). There are models that can be purchased and used *
- **Vulnerability Scores:** _(add: Moat 4/5 · Data 5/5 · Platform 3/5)_
- **Top Risk:** * Our own customers could recreate this on their own contracts and just buy the data from us, particularly the larger organizations, pricing curve will help diminish this. The compounding of multiple airline and agency customers contracts and contract terms that looks at if contracts are similar and increases the chance of limiting hallucinations. *
- **Confidence:** High Confidence (add: H / M / L) Based on pilot working and a pilot customer and an industry where commission contracts and performance is critical_
- **Prototype:** [ https://lovable.dev/projects/11e2d918-c432-4875-a860-073a2946e479?magic_link=mc_ed2a06df-c6f9-4c25-975d-de4247002702](https://lovable.dev/projects/11e2d918-c432-4875-a860-073a2946e479?magic_link=mc_efe04817-0566-41ad-929f-9ffa18b97729)
- **Kill Criteria:** *In ability to get the AI PDF reader to reliably pull 90% of the contracts information Probablistic issues in which it produces too many hallunications with the data or overtime*

→ Details: [`01-the-bet/`](01-the-bet/)

---

## The Moat (M2)

**Why this won't get copied in 6 months.**

- **Data Flywheel Score:** 12/20
- **Weakest Loop:** * Preference Loop
- **Top Encroachment Threat:** * Adobe and an AI Reader a customer can use to pull the information. Even OpenAi, Google would have AI models that could pull and organize data into a database for the start.
- **Encroachment Defense:** * WHat signal can we get from users? what is more than usage? What is the critical behavior for success.
- **Vendor Portability:** _Partial_

→ Details: [`02-the-moat/`](02-the-moat/)

---

## The Margin (M3)

**Will this make money or bleed it?**

- **Gross Margin (current):**
- **Gross Margin (AI-adjusted):** 71.4% ($50.00/user)
- **Pricing Model:** seat-based / usage-based / outcome-based / hybrid
- **Pricing Today → Tomorrow:** **Proposed AI pricing:** → **Model:** seat-based / usage-based / outcome-based / hybrid
- **Total AI COGS / unit:** AI COGS/user: $10.00
- **Cascading Strategy:** Triage: **Frontier model:**; frontier: **Routing rule:**; ratio Expected Ration 70% to 30% Frontier. This would depend on customer type over time.
- **Net Margin Shift:** $3 Million increase. The Contract analysis and Intelligence pairing with the data increases the value.…
- **Break-even at:**


→ Details: [`03-the-margin/`](03-the-margin/)

---

## The Contract (M4)

**Why users will trust a probabilistic system.**

- **Reliability Target:** 90%
- **Golden Dataset:**
- **Confidence UX:** Display the estimated statistics by a complexity rating (Green, Yellow, Red) on each rule (applied at time of parsing). Humans able to review and update. Stats on updates and changes.…
- **HITL Architecture:** **Trigger:** User enters with visibility to all rules, ability to name rules, and ability to edit rules. Internal humans enter when certain notifications, particularly around data strcuture to data read misalignment happens or a decrease in…
- **Failure Mode Coverage:** *What failure mode did your partner find that you missed?*

→ Details: [`04-the-contract/`](04-the-contract/)

---

## The Guardrails (M5)

**What breaks when this scales, and what compounds.**

- **Compounding System:** The Contract Rules. More contracts by airlines and agency will provide overlap, complexity analysis, and rule format changes that can grow the system and increase successful transposal of the rules into the database and provide a valuable new asset to trend and track industry incentives
- **Governance Posture:** - Scope: Covers the Customer Facing Product, AI Models, and Golden Dataset, Databases; User Access and Preferences Excludes: Internal Dashboards and Reporting, Training
- **Autonomy Boundaries:** Autonomy boundaries: User Profile and Preferences, never auto. Rule Structure in Engine (Rule Acceptance), human approval required. Token Over usage - Limit with Message, auto. Visualization and Report Creation, auto. Contract Rules / Contract Visual Retention Changes, human approval required.
- **Escalation Triggers:** Escalation triggers: 1) Customer Message indicates breach in privacy or security (Every time) 2) Editability needed of rules increases 10% over 4 uploads 3) Token Overusage 2% over customer limits or 5% over product limits 4) Data Associated with PII or PCI Discovered 5) Data Retention (Contract Visuals) past 1 YEAR of Approval

- **Audit Cadence:** Audit cadence: Daily, Usage and Update Dashboards (SRE). Daily, Golden Dataset Modifications/Changes (Lead Engineer). Weekly, Error Rates and Issues (Product Manager).
- **Shadow AI Audit (user-side):** Merge with Outside Data | source: User interview | signal: Capability gap | freq: H | spend: $100/mo | decision: Ignore
Contract Scenario Negotiations | source: Other | signal: Capability gap | freq: M | spend: $4000/mo | decision: Build
Contract Development | source: Sales call | signal: Trust gap | freq: M | spend: $1000/mo | decision: Build
Visualizations and Reports | source: Support ticket | signal: Trust gap | freq: M | spend: $100/mo | decision: Build
- **Agent Boundaries:** Not Shipping Agents
- **Regulatory Exposure:** Regulatory exposure (EU AI Act / other): Customer Privacy and Data Privacy (GDPR and US State Privacy Data Broker Protections). Controls: No training on PII or PCI or Legal Data List.


→ Details: [`05-the-guardrails/`](05-the-guardrails/)

- ## The Pitch (M6)

**How you get this funded, shipped, and adopted.**

- **Horizon 1 (Now):** PDF to AI Reader using contract examples · Create Airline Rules Database structure · Mapping Data Metrics used in Contracts to Database outputs · Develop Upload UI · Develop UI for Rules Manual Modification · Connect to Testing Data set for Performance Analysis · Integrate Visual UI Dashboards (Discovery Point) · Integrate Report and Analysis storage · Develop Initial User Guardrails · Develop Automated AI Triggers for Cost, Usage, Quality Decgridation
- **Horizon 2 (Next):** API to AI Reader · Pilot with 2-3 Customers, Airline and Agency spread
- **Horizon 3 (Bet):** Add in Natural Language Report generation for QBR processing
- **Board Narrative:** **The case:** Why now: Commission and interline contracts are re-negotiated constantly and manually re-keyed today — our own pilot customer confirms this is active, paid-for pain (their shadow spend shows $4,000/month on contract scenario negotiation work and $1,000/month on contract development, both already flagged internally as "Build" priorities). The extraction technology has just crossed the reliability threshold where this is buildable at 90% accuracy in a pilot — that threshold didn't exist 12-18 months ago. And the window is closing: platform players are moving toward generic document extraction, so the advantage is in moving now, not in the technology itself. What's defensible: I'll be direct — today, it isn't defensible yet, and I'm not going to pretend otherwise. Our Data Flywheel score is 12/20, and our Encroachment Defense against Adobe, OpenAI, or Google shipping this as a feature is currently an open question, not an answer. The moat we're betting we can build is cross-customer compounding: contracts across multiple airline and agency customers share enough structure that pooled data reduces hallucination rates and gets harder to replicate the more customers we onboard. That's a hypothesis, not a proof point yet — which is exactly what this POC is designed to test. The economics: At $50/user with $10/user AI cost, we're at 71.4% gross margin on paper. I want to flag two open items rather than paper over them: pricing model is still undecided across four options (seat, usage, outcome, hybrid), and the $3M net margin shift we're projecting has no stated baseline, so I can't yet defend that number under scrutiny. Both need to be resolved before this scales past POC.
- **Ask:** Thesis (1 sentence): We turn messy, high-stakes airline and agency commission contracts into a trusted, structured rules database automatically, so customers stop manually re-keying contract terms and start using that data to run negotiations and QBRs.
- **Key Strategic Change:** We use AI to extract additional value and create additional competitive differentiation for our data products and additional data extraction from complex sources. Utilize AI with human guardrails and oversight to ensure quality and trust with customers. Start small with iterative POC to Pilot to Customer to ensure cost effective and governance measures that align to our mission of being the "trusted source of airline intelligence",

→ Details: [`06-the-pitch/`](06-the-pitch/)
