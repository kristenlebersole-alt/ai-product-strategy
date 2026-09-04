# Golden Dataset & Reliability Contract

## Golden Dataset Spec

**Adversarial rows included:** _4_
**Coverage gaps identified by partner:**

Golden Dataset, Module 4

Test cases:
  1. Edge: N · Judge: both, IN: Accuracy by Rule Complexity → OUT: Number of Conditions Accepted
  2. Edge: N · Judge: rule, IN: User % of Modification → OUT: 10% Modification After Contract Read
  3. Edge: Y · Judge: rule, IN: Embedded Visuals Extraction → OUT: Visual of Rule in Contract
  4. Edge: N · Judge: rule, IN: PDF Type Parsing Identifier → OUT: Against Example (PDF, Scanned, Image) - Testing ticky input
  5. Edge: N · Judge: rule, IN: Data Structure Validation → OUT: Key Metrics Input (Market, Share, Commission)
  6. Edge: Y · Judge: LLM, IN: Empty PDF → OUT: Adversarial Row ·
  7. Edge: Y · Judge: LLM, IN: Foreign Language → OUT: ·
  8. Edge: Y · Judge: LLM, IN: Complience Testing → OUT: GDPR Identification
  9. Edge: Y · Judge: rule, IN: PDF Page Count → OUT: PDF page = Number Pages Read
  10. Edge: N · Judge: rule, IN: Extraction Correctness → OUT: Human Touch Occured - Real Data Values (LAXDCA, QSI 25, Commission Value 10/ticket) - Adversarial tests tricky inputs
  11. Edge: N · Judge: both, IN: Extraction Completeness → OUT: Human Touch Needed
  12. Edge: N · Judge: rule, IN: Rule Duplication → OUT: Review of final Dataset - Adversarial
  13. Edge: N · Judge: rule, IN: Example PDF Contract → OUT: Actual Examples - Proxy of Users
  14. Edge: N . Judge: both, IN: Actual example contract data structure and set from customer provided examples (airlines and travel agency have standards as a base can use)

Dataset health
- Total: 13
- Edge cases: 5 (38.5%)
- Judge mix: 62% rule / 23% LLM / 15% both


## Confidence UX Design

**Approach:** Display the estimated statistics by a complexity rating (Green, Yellow, Red) on each rule (applied at time of parsing). Humans able to review and update. Stats on updates and changes. Visible

**Confident (>90%):** User can Approve/Edit/Reject. Show Confidence Color Rating. Provide Image extract.

**Uncertain (50-90%):** Organize by Confidence Color Rating, Highlight areas of Questions for Review. Provide Image extract. User can Approve/Edit/Reject.

**Not confident (<50%):** Have these at the top. Provide Image and location attempted to extract.  Provide a Partial generation, but Color Red for Clarity. User can Approve/Edit/Reject.

**User control surface:** 

- Users correct & override outputs
- Corrections feed back into the model / dataset
- Users adjust the confidence threshold _(not yet)_- Thinking this might be a behind the scenes and might be controlled by the correction set. 
- Users see AI reasoning / drivers _(not yet)_
- - Users see overall statistics on confidence area and suggested re-load and changes to make to increase the readability (if they used a blurry image vs actual contract in PDF). 


**User control surface:**

## Reliability Contract

| Metric | Target | Measurement | Alert Threshold |
|--------|--------|-------------|-----------------|
| Accuracy | | | |
| Hallucination rate | | | |
| Latency (p95) | | | |
| Drift velocity | | | |

## HITL Architecture
<!-- When does a human step in? What's the escalation path? -->
User comes in to be able to review and modify ever rule parsed and put in. 

## Red-Team Findings
*What failure mode did your partner find that you missed?*
