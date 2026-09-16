# Compounding System Design

## Feedback Loops

| Loop | Input | Output | Compounds? | Status |
|------|-------|--------|-----------|--------|
| Recursive Learning | User Edits on Rule Patterns | Golden Data Set | Y | active |
| Cross-Domain Transfer | Contract 1 Helps Contract 20 | · | Y | active |
| Network Intelligence | Customers Rules Help Identify and Quality Check all rule patterns and examples | Golden Data Set | Y | active |
| Cross Domain | Rules against Data help identify need for change or improved reports or visualizations | Visualization or Report Gaps via Case Tickets Queue | N | broken |

**If Model doesntupdate for 3 months? can you fix it?**

**Fix plan:** Currently have it identify the gaps, need to see if we can integrate updates and changes into training, CI-CD pipeline or enhancements. How quickly should this evolve?

## Context Connectivity
<!-- How does knowledge flow across teams and domains? Where does it silo? -->

**How knowledge flows:** Case Tickets (Support); Audit Logs on Golden Data Set Changes; Dashboards to identify user/customer most impactful.

**Where it silos:** Case Tickets and prioritization if changes needed; Account Managers feedback from customer could be overridden (Visualizations and Report Gap Changes); Analysts; Engineering supporting dataset

## Governance Policy

<!-- Governance Policy, Contract Intelligence -->

## Governance Policy

**Scope:** Covers the Customer Facing Product, AI Models, and Golden Dataset, Databases; User Access and Preferences Excludes: Internal Dashboards and Reporting, Training

**Autonomy boundaries:** User Profile and Preferences, never auto. Rule Structure in Engine (Rule Acceptance), human approval required. Token Over usage - Limit with Message, auto. Visualization and Report Creation, auto. Contract Rules / Contract Visual Retention Changes, human approval required.

**Escalation triggers:** 1) Customer Message indicates breach in privacy or security (Every time) 2) Editability needed of rules increases 10% over 4 uploads 3) Token Overusage 2% over customer limits or 5% over product limits 4) Data Associated with PII or PCI Discovered 5) Data Retention (Contract Visuals) past 1 YEAR of Approval

**Audit cadence:** Daily, Usage and Update Dashboards (SRE). Daily, Golden Dataset Modifications/Changes (Lead Engineer). Weekly, Error Rates and Issues (Product Manager).

**Regulatory exposure (EU AI Act / other):** Customer Privacy and Data Privacy (GDPR and US State Privacy Data Broker Protections). Controls: No training on PII or PCI or Legal Data List.

## Agent Topology

Not Shipping Agents


## Shadow AI Audit

Shadow AI Audit (user-side), Module 5

## Discover, User-Side Workarounds
- Merge with Outside Data | source: User interview | signal: Capability gap | freq: H | spend: $100/mo | decision: Ignore
- Contract Scenario Negotiations | source: Other | signal: Capability gap | freq: M | spend: $4000/mo | decision: Build
- Contract Development | source: Sales call | signal: Trust gap | freq: M | spend: $1000/mo | decision: Build
- Visualizations and Reports | source: Support ticket | signal: Trust gap | freq: M | spend: $100/mo | decision: Build

## Pattern Assessment
- Workarounds found: 4
- Build candidates: 3
- Partner candidates: 0
- Ignore decisions: 1
- Adjacent spend: $5200/mo
- Dominant signal: Capability gap

## Action Plan
### Build
Adding Value with Visualizations and Reports. Ensure the learnings of other customers and users compounds so it is not in the best interest.  

### Partner
Contract Development can partner with customers into their systems (reusing or rewriting of the contract rules). 

### Ignore + Monitor
Much of the data would be internal and proprietary. Could align with other external data.

## Roadmap Brief
Based on your audit: 4 user-side workarounds discovered.
Decisions: 3 build · 0 partner · 1 ignore · 0 TBD.
Estimated adjacent spend: $5200/mo across surveyed users.
Dominant signal: Capability gap.

Recommended next step: Capability gaps dominate, users want something your product does not do. Strongest near-term move is building one or two of these natively before a competitor does.

Sequence the Build column by frequency × strategic relevance. Confirm Partner candidates with the external tools' partnership teams. Re-run this audit each quarter, workarounds shift fast.



**Responsible AI Maturity**

Responsible AI Maturity Scorer, Module 5

Total: 16/25, Proactive
Solid foundation. Now make governance a competitive advantage.
Weakest: Fairness, Accountability

Compliance: 4/5
1 = no formal compliance, 5 = certified and audited

Transparency: 3/5
1 = black box, 5 = full explainability + audit trails

Fairness: 2/5
1 = no bias testing, 5 = continuous monitoring + remediation

Privacy: 5/5
1 = minimal consent, 5 = privacy-by-design + user controls

Accountability: 2/5
1 = no owner, 5 = RACI defined + incident playbooks

