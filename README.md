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
- **Vulnerability Scores:** _(add: Moat _/5 · Data _/5 · Platform _/5)_
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

- **Compounding System:** | Loop | Input | Output | Compounds? | Status | |------|-------|--------|-----------|--------| | Recursive Learning | User Edits on Rule Patterns | Golden Data Set | Y | active | | Cross-Domain Transfer | Contract 1 Help…
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





- 




→ Details: [`05-the-guardrails/`](05-the-guardrails/)
