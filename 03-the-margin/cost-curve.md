# Cost Curve & Pricing Strategy

##

## Features Table
|Feature | Complexity | Model Tier | Cost/Req | Volume % | Weighted | Justification/WHy
|--------------|----------------|-------|-------|-------|-------|----------------|
| 1) Read the Contract PDF Rule Parsing | Medium | Mid | $0.02 | 10% | $0.002 | LEADER: This is a Must Have. Airline/Agency Contracts have a lot of rules and some are nested and very specific. Looking to hit 85% quality on reading the contract and proper parsing |
| 2) User to modify and fix the rules or expand nuances AI might miss | N/A | N/A | N/A | N/A | N/A | LEADER: This is a Must Have. User Quality Varified. Ok if updating or modifying 15% of rules, particularly complex. This is a heavy set-up usage for new customers or new contracts. |
| 3) Matches the contract rules / terms with the performance data we already have | N/A | N/A | N/A | N/A | N/A | Below are the 3 known use cases to use AI with the data. Common Needs that all Quarterly Reviews Handle. They have a need/must know, nice to know, interesting insights providing value
| 3A) Repeatable QBR metrics and review (Cheap AI; Some User); | Simple | Small | $.01 | 45% | $.0045 | LEADER: This is a Must Have. Common Needs (The Need / Must Know) that all Quarterly Reviews Handle. A person or set of persons job is to exclusively do this today for all airlines/Travel Agency contracts. Doing this well, means these roles can focus on the Nice to Have and Value generating insights. |
| 3B) QBR deeper analysis and trends review (Cheap); | Simple | Mid | $0.02 | 25% | $0.009 | Killer: Value Generating & Interesting Insights and Value Adds of QBR |  
| 3D) Future Scenario analysis and contract renegotiation preparation | Complex | Frontier | $0.09 | 10% | $0.009 | Killer: Preparation and tradeoff analysis to gain more revenue through contracts  |
| **Blended** |  |  |  | 100% | $0.0245 | Majority of Usage is in the Simple and Small repeatable models. Risk if more usage goes to future scenarios. |  


## Cost Model

| Cost Category | Per-User/Month | Notes |
|--------------|----------------|-------|
| Inference (primary model) | | |
| Inference (cascading/triage) | | |
| Infrastructure | | |
| Data/storage | | |
| Human-in-the-loop | | |
| **Total AI COGS** | | |


# Margin Calculator, Module 3

## Inputs
- Avg requests/user/month: 500
- Blended cost/request: $0.02
- Revenue/user/month: $70
- Non-AI COGS/user/month: $10

## Current Margin
- AI COGS/user: $10.00
- Total COGS/user: $20.00
- Gross margin: 71.4% ($50.00/user)

## Cascading Strategy
<!-- Cheap model → frontier model routing logic -->
-- Want a multi - Provider Routing based on the activity.
Could add an initial set up costs for the initial contract reading.
Consider diluting the model type, based on usage amount to try to curb costs from over usage by customers. This would be a by month/by user usage on potential output. 
Size for us matters in organizations. 

**Triage model:**
**Frontier model:**
**Routing rule:**
**Expected cascade ratio:**

## Pricing Model

**Current pricing:**
**Proposed AI pricing:**
**Model:** seat-based / usage-based / outcome-based / hybrid

Pricing Strategy Block, Module 3

Pricing Strategy
- Strategy posture: Maximize
- Pricing model: Seat / Access
- Unit of work metered: Reports Generated
- Base fee ($/month): 10000 (Note: This is an average for all companies, but pricing would be variable to the size of an organization and the amount of data that flows through us; the larger the company the more money)
- Price per unit: $0
- Estimated units/user/month: 50
- Implied revenue/user/month: $10000.00

Decision Note
Why this pricing structure fits the buyer and the value delivered: It mimics the pricing position and structure of the original product this will be enhancing. Since this product is an Add-On to a current product and does not service all users, mimicking a pricing strategy of the original to start. Additional this would be a revenue generating and margin generating analysis for customers driving the value higher.


## Stress Tests


## Stress Test
| Scenario | AI COGS | Margin |
|----------|---------|--------|
| 3x Cost  | $30.00 | 42.9% ($30.00) |
| 2x Usage | $20.00 | 57.1% ($40.00) |

## Board One-Pager
<!-- Before/After: Old SaaS revenue vs. AI usage revenue for your product -->

**Before (traditional SaaS):**
Before Revenue: $2 Million for the data and reporting tool
Manual Data Entry and Manual report running to pair actual data (what was actually sold) to what was in the contract and if they will fulfill the terms of the contract based on the various routes, market share. Highly Manual, and most focus is placed on the need/must haves of the QBR.
**After (AI-enabled):**
After AI: $5 Million for Analysis and Scenarios. 
Providing Value in the Analysis and Scenarios. Ability to increase commission by finding either overachieving routes, undervalued routes, or areas Travel Agency makes an Airline Network profitable by serving less Airline focused routes. Ability to do it faster and find the diamonds in the rough helps bring focus to the more interesting areas
**Net margin shift:**
$3 Million increase. The Contract analysis and Intelligence pairing with the data increases the value. Ability to focus on less of the needs/must dos as they are repeatable and focus on the revenue & driving value increasing aspects leads this to significantly increase value.
