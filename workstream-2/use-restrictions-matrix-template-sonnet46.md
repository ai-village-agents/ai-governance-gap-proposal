# AI Use-Restrictions Matrix Template

**TEMPLATE NOTICE:** This document is a template. Organizations must customize it for their own operations, legal obligations, and risk profile. Replace all placeholders such as [ORGANIZATION NAME], [DATE], and [ROLE].

---

## 1. HEADER/METADATA

**Title:** AI Use-Restrictions Matrix Template

**Version:** [VERSION]

**Classification:** [CLASSIFICATION] (e.g., Internal, Confidential, Restricted)

**Author:** [NAME], [ROLE]

**Approved By:** [NAME], [ROLE]

**Effective Date:** [DATE]

**Review Date:** [DATE]

**Document Owner:** [ROLE] — [ORGANIZATION NAME]

**Quick-Reference Legend:**

- `P` = Permitted
- `PR` = Prohibited
- `C` = Conditional
- `N/A` = Not Applicable

**Purpose:** This matrix operationalizes §203 of proposed NDAA legislation by translating policy into specific, enforceable AI use restrictions.

**Cross-Reference:** C072 Incident Log and C072 Double-Bind Detection Guide in `workstream-1/c072-double-bind-detection-guide-sonnet46.md`.

---

## 2. SECTION 1 — EXECUTIVE SUMMARY

1. Written use restrictions are a primary defense against coercive or ambiguous AI deployments.
2. The C072 pattern demonstrates that lack of written constraints can become the point of failure in high-stakes engagements.
3. This template provides a structured matrix for classifying AI use-cases and enforcing minimum guardrails.
4. The matrix is a living document, reviewed and updated based on operational experience and external regulation.
5. The matrix is intended for [ORGANIZATION NAME] and must be adapted to your legal, ethical, and business context.
6. The matrix applies to all AI systems deployed, procured, or integrated by [ORGANIZATION NAME].
7. It does not replace existing policies; it makes them operational.
8. The matrix uses a three-tier classification system: Permitted, Conditional, Prohibited.
9. Permitted uses are explicitly authorized and require no additional approval beyond baseline controls.
10. Conditional uses require defined prerequisites, documented approvals, and ongoing audits.
11. Prohibited uses are never authorized regardless of context or contractual demand.
12. The matrix includes both sector-agnostic restrictions and sector-specific annexes.
13. Sector-specific annexes must be completed for any regulated or high-impact domain.
14. Each use-class is tied to an approval authority and audit cadence.
15. All conditional approvals must be documented and retained.
16. Escalation triggers are mandatory; they bypass normal approval paths.
17. The written-memorialization test is a critical C072 safeguard.
18. If a counterparty accepts restrictions but refuses to write them down, treat that refusal as a red flag.
19. That refusal triggers escalation under the C072 protocol.
20. The matrix is intended to be readable by business, legal, security, and operational teams.
21. The matrix should be embedded in procurement, contracting, and incident response processes.
22. All external AI agreements must reference the matrix.
23. Any deviation requires explicit documentation.
24. The matrix is designed to prevent “policy drift” under external pressure.
25. It is also designed to prevent “silent expansion” of AI use-cases beyond intended scope.
26. Clear written restrictions reduce operational risk, regulatory exposure, and reputational harm.
27. The matrix supports consistent decision-making across business units.
28. The matrix is enforceable only when kept current and implemented by trained staff.
29. The matrix is a key control in the AI governance program of [ORGANIZATION NAME].
30. The C072 case shows that absence of written restrictions can trigger designation crises and loss of trust.

---

## 3. SECTION 2 — DEFINITIONS

**Permitted Use:** Uses explicitly authorized without additional approval beyond baseline controls. These uses are listed in the matrix as `P` and require routine compliance checks.

**Prohibited Use:** Uses never authorized regardless of context, business pressure, or contractual demand. These uses are listed as `PR` and cannot be approved or reclassified without full board action.

**Conditional Use:** Uses authorized only upon satisfaction of defined prerequisites. These uses are listed as `C` and require documented approval.

**Guardrail Floor:** Minimum non-negotiable restrictions that cannot be waived by any internal or external party. Guardrail Floor requirements apply to all AI uses.

**Approval Authority:** The role or body authorized to grant conditional use approval (e.g., Board AI Committee, CISO, Legal, CRO).

**Escalation Trigger:** A condition requiring immediate escalation above normal approval authority. Escalation triggers are mandatory and time-bound.

**Use-Class:** A category of AI deployment sharing common risk characteristics (e.g., hiring recommendations, credit underwriting support).

**C072 Pattern:** A situation where a powerful counterparty pressures an organization to weaken or eliminate written use restrictions. This includes refusal to memorialize restrictions in contract or exhibit form.

**“Any Lawful Use” Language:** Contract language eliminating sector-specific restrictions, a known C072 indicator and automatic escalation trigger.

**Written-Memorialization Test:** A requirement that any agreed restriction must be documented in writing in the contract, addendum, or use-restrictions exhibit.

**Human-in-the-Loop (HITL):** A human reviewer must approve or override AI outputs before action is taken.

**Human-on-the-Loop (HOTL):** A human reviewer monitors AI outputs and can intervene, but does not pre-approve each action.

**High-Impact Decision:** A decision affecting legal rights, access to essential services, or material financial outcomes.

**Model Documentation:** The minimum evidence package required for conditional approval (e.g., model card, data provenance, performance metrics, audit logs).

**Audit Frequency:** The interval for compliance and performance audits for a given use-class.

**Reclassification:** The process of moving a use-class between Permitted, Conditional, and Prohibited status.

**Incident Log:** A structured record of C072 escalation events, maintained in the C072 Incident Log template.

---

## 4. SECTION 3 — CLASSIFICATION FRAMEWORK

### 4.1 Three-Tier System

**Permitted (P):**

- Description: Low-risk uses with clear safeguards, routine oversight, and minimal external exposure.
- Examples: Internal drafting support, non-sensitive research summaries.
- Approval Path: Business owner + baseline compliance check.
- Documentation: Use-case description, owner, data sources, retention policy.

**Conditional (C):**

- Description: Medium- to high-risk uses requiring prerequisites, formal approval, and ongoing monitoring.
- Examples: Clinical decision support, credit underwriting support, hiring recommendations.
- Approval Path: Approval Authority per matrix row.
- Documentation: Full model documentation, risk assessment, audit plan, and written approvals.

**Prohibited (PR):**

- Description: Uses that are unacceptable due to legal, ethical, or strategic risk.
- Examples: Fully autonomous lethal targeting, fully automated adverse action without human review.
- Approval Path: No approval permitted; only reclassification via board-level process.
- Documentation: Record of prohibition and rationale; update to C072 log if challenged.

### 4.2 Classification Decision Flowchart (Text-Based)

Start

- Is the use-class explicitly listed in the matrix?
  - Yes → Apply listed classification.
  - No → Proceed to initial classification review.

Initial Classification Review

- Does the use involve high-impact decisions, safety-critical systems, or regulated data?
  - Yes → Default to Conditional or Prohibited.
  - No → Proceed to risk assessment.

Risk Assessment

- Are adequate safeguards, data controls, and auditability in place?
  - Yes → Candidate for Permitted or Conditional.
  - No → Conditional with prerequisites, or Prohibited if safeguards cannot be met.

Written-Memorialization Test

- Are restrictions accepted and written into a formal document?
  - Yes → Continue approval.
  - No → Escalation trigger (C072 protocol).

Final Classification

- Record in the matrix, assign approval authority, and schedule audit.

### 4.3 Reclassification Procedure

1. Any request to reclassify a use-class must be submitted in writing with rationale.
2. Conditional → Permitted: Requires approval by CISO + Legal + owner of the affected use-case.
3. Conditional → Prohibited: Requires approval by CISO + Legal + CRO, with board notification.
4. Prohibited → Conditional: Requires Full Board vote + external ethics review.
5. Mandatory review triggers include:
   - Regulatory change affecting the use-class.
   - Material incident or adverse event.
   - New evidence of misuse or external coercion.
6. All reclassification decisions must be documented and retained for at least 7 years.

---

## 5. SECTION 4 — CORE USE-RESTRICTIONS MATRIX (UNIVERSAL)

**Legend:** `P` = Permitted, `C` = Conditional, `PR` = Prohibited

| Use-Class | Description | Classification | Approval Authority | Prerequisites | Time Limit | Audit Frequency |
| --- | --- | --- | --- | --- | --- | --- |
| A1 Market Research | Summaries of public market trends | P | Business Owner | Data is public, non-sensitive | N/A | Annual |
| A2 Competitive Intel | Competitor analysis using public sources only | P | Business Owner | Public-only sources, no scraped PII | N/A | Annual |
| A3 Policy Analysis | Policy or legislative analysis for internal use | P | Legal | Non-sensitive data | N/A | Annual |
| A4 Legal Research | Internal legal research support | P | Legal | Attorney review; no external filing | N/A | Annual |
| A5 Contract Drafting | Draft internal contract language | C | Legal | Attorney review; version control | 12 months | Annual |
| A6 FOIA Support | Draft FOIA responses (non-final) | C | Legal | Legal review; audit log | 12 months | Semi-annual |
| A7 Sensitive Intel | Analysis using sensitive internal data | C | CISO + Legal | Data classification review; DLP controls | 12 months | Quarterly |
| B1 Hiring Recommendations | Ranking or scoring candidates | C | HR + Legal | Disparate impact testing; HITL | 12 months | Quarterly |
| B2 Loan Underwriting Support | Assist credit decisions | C | CRO + Legal | SR 11-7 docs; ECOA notice capability | 12 months | Quarterly |
| B3 Medical Triage Support | Non-final triage recommendations | C | CMO + Legal | Physician oversight; adverse event log | 6 months | Quarterly |
| B4 Benefits Determination | Support eligibility review | C | Legal + CRO | HITL review; auditability | 12 months | Quarterly |
| B5 Risk Scoring | Risk scores for internal prioritization | C | CRO | Model documentation; bias testing | 12 months | Semi-annual |
| B6 Performance Evaluation | Employee performance insights | C | HR + Legal | Transparency notice; HITL | 12 months | Semi-annual |
| C1 Autonomous Weapons | Weapon system autonomy | PR | N/A | Prohibited | N/A | N/A |
| C2 Autonomous Legal Filings | File legal documents without human review | PR | N/A | Prohibited | N/A | N/A |
| C3 Autonomous Financial Trades >$X | Fully automated trades above threshold | C | CRO + CFO | Trade limits; human override; monitoring | 6 months | Monthly |
| C4 Automated Hiring Decisions | Full automation without review | PR | N/A | Prohibited | N/A | N/A |
| C5 Automated Adverse Actions | Loan denial or account closure without review | PR | N/A | Prohibited | N/A | N/A |
| C6 Incident Response Automation | Automatic containment actions | C | CISO | Human-on-the-loop; rollback plan | 6 months | Monthly |
| D1 Bulk Data on Individuals | Commercial bulk data on individuals | C | Legal + CISO | Data provenance; consent verification | 6 months | Quarterly |
| D2 Government-Compelled Data Sharing | Bulk data to government | PR | N/A | Prohibited without lawful order | N/A | N/A |
| D3 Cross-Border Transfers | Transfer sensitive data across borders | C | Legal + CISO | Data transfer agreement; local law review | 6 months | Quarterly |
| D4 Large-Scale Scraping | Scrape public content at scale | C | Legal | Robots.txt compliance; TOS review | 12 months | Semi-annual |
| D5 Data Fusion | Combine datasets to infer sensitive attributes | PR | N/A | Prohibited | N/A | N/A |
| D6 Synthetic Data Generation | Generate synthetic datasets | C | CISO | Privacy review; re-identification testing | 12 months | Annual |
| E1 Internal Comms Drafting | Draft internal memos | P | Business Owner | No sensitive data in prompts | N/A | Annual |
| E2 External Customer Content | Draft customer-facing content | C | Marketing + Legal | Brand review; disclosure if required | 12 months | Quarterly |
| E3 Regulatory Filings | Draft regulatory filings | C | Legal + Compliance | Attorney review; audit log | 12 months | Quarterly |
| E4 Legal Brief Drafting | Draft legal arguments | C | Legal | Attorney review; provenance tracking | 12 months | Quarterly |
| E5 Public Press Releases | Draft press statements | C | Comms + Legal | Executive review; fact check | 12 months | Quarterly |
| E6 Policy Documents | Draft internal policy | C | Legal + CISO | Policy owner review | 12 months | Annual |
| F1 Employee Monitoring | Monitor employees via AI analytics | C | HR + Legal | Notice to employees; limited scope | 6 months | Quarterly |
| F2 Customer Behavior Tracking | Behavioral tracking analytics | C | Legal + Privacy | Consent or legal basis; DPIA | 6 months | Quarterly |
| F3 Government Surveillance Integration | Integrate AI with surveillance systems | PR | N/A | Prohibited | N/A | N/A |
| F4 Biometric Surveillance | Facial recognition tracking | PR | N/A | Prohibited | N/A | N/A |
| F5 Fraud Detection Monitoring | Monitor for fraud indicators | C | CRO | Privacy review; audit logs | 12 months | Quarterly |
| F6 Insider Threat Detection | Monitor internal systems for threats | C | CISO + Legal | DPIA; limited data retention | 12 months | Quarterly |
| G1 Force Enhancement | Tactical support to military units | C | Legal + CISO + JAG | ROE alignment; HITL; 90-day review | 90 days | Quarterly |
| G2 Targeting Support | Assist target identification | C | Legal + CISO + JAG | Strict HITL; full audit trail | 90 days | Quarterly |
| G3 Adversarial Analysis | Analyze adversary capabilities | C | Legal + CISO | Classified handling; red-team review | 6 months | Quarterly |
| G4 Strategic Planning | Support defense strategy planning | C | Legal + CISO | Classified handling; escalation review | 6 months | Quarterly |
| G5 Military Training | AI in training simulations | C | Legal + CISO | Safety review; data controls | 12 months | Semi-annual |
| H1 Power Grid Operations | AI control of power systems | C | CRO + CISO + Legal | Safety case; fail-safe; regulator review | 6 months | Monthly |
| H2 Water System Operations | AI control of water systems | C | CRO + CISO + Legal | Safety case; fail-safe; regulator review | 6 months | Monthly |
| H3 Financial Systems Operations | AI control of core banking | C | CRO + CFO | Stress testing; rollback plan | 6 months | Monthly |
| H4 Healthcare Systems Operations | AI control of hospital systems | C | CMO + CISO | Safety case; patient safety oversight | 6 months | Monthly |
| H5 Transportation Systems | AI control of transport networks | C | CRO + CISO | Safety certification; fail-safe | 6 months | Monthly |

---

## 6. SECTION 5 — SECTOR-SPECIFIC ANNEXES

### 6.1 DEFENSE / GOVERNMENT CONTRACTING

**Prohibited:**

- Fully autonomous lethal targeting.
- “Any lawful use” contract clauses without written carveouts.
- Bulk commercial data on US persons without FISA authorization.

**Conditional:**

- Force-enhancement support.
  - Requires JAG review.
  - Commanding officer approval.
  - Documented ROE alignment.
  - Human-in-the-loop confirmation.
  - 90-day review cycle.

**Escalation Trigger:**

- Any contractor demand to remove written use restrictions → C072 Stage 2 protocol.

**Pentagon Case Study Note:**

- The lack of a written use-restriction exhibit was central to the designation crisis.

### 6.2 HEALTHCARE

**Prohibited:**

- Autonomous treatment decisions without physician review.
- Denial of coverage determinations without human review.
- Use of protected health information for model training without explicit patient consent.

**Conditional:**

- Clinical decision support.
  - Requires FDA clearance or IRB approval.
  - Physician oversight.
  - Adverse-event logging.
  - HIPAA compliance attestation.

**Escalation Trigger:**

- Any payer or provider demand to remove physician-review requirement.

### 6.3 FINANCIAL SERVICES

**Prohibited:**

- Fully automated adverse action (loan denial, account closure) without human review.
- Use of AI for market manipulation.
- Use of customer data for competitor intelligence.

**Conditional:**

- Credit underwriting support.
  - Requires model documentation per SR 11-7.
  - Fair lending testing.
  - ECOA adverse-action notice capability.
  - 12-month validation cycle.

**Escalation Trigger:**

- Any regulatory or investor pressure to remove fair-lending guardrails.

### 6.4 HUMAN RESOURCES

**Prohibited:**

- Fully automated hiring/firing decisions.
- Use of protected-class proxy variables.
- Facial recognition scoring in candidate screening.

**Conditional:**

- Resume screening and candidate ranking.
  - Requires disparate-impact testing.
  - Human review of all rejections.
  - Annual bias audit.
  - Disclosure to candidates.

**Escalation Trigger:**

- C-suite pressure to eliminate disparate-impact testing requirement.

### 6.5 CONTENT & MEDIA

**Prohibited:**

- Generation of non-consensual intimate imagery.
- Disinformation campaigns.
- Micro-targeted political advertising using prohibited characteristics.

**Conditional:**

- AI-generated news content.
  - Requires editorial review.
  - AI disclosure label.
  - Fact-check integration.
  - Quarterly accuracy audit.

**Escalation Trigger:**

- Advertiser or platform pressure to remove AI disclosure labeling.

---

## 7. SECTION 6 — APPROVAL WORKFLOW

### 7.1 Standard Conditional Use Approval

1. Requestor submits use-case request with use-class candidate.
2. Use-class determination by policy owner.
3. Prerequisites checklist completed and signed.
4. Risk assessment completed by [ROLE].
5. Approval Authority sign-off recorded.
6. Documentation stored in [SYSTEM/REPOSITORY].
7. Audit schedule established and owner assigned.
8. Timeline: 5–10 business days for standard approvals.

### 7.2 Expedited Approval (Time-Sensitive Deployments)

1. Requires Deputy CISO or equivalent + Legal sign-off within 24 hours.
2. Full standard review must occur within 30 days retroactively.
3. Expedited approvals are logged and reviewed quarterly.
4. Prohibited: Expedited process cannot be used for any use-class in Defense & Military or Critical Infrastructure.

### 7.3 Board-Level Escalation (C072-Pattern Situations)

1. Trigger: External pressure to weaken or eliminate written restrictions.
2. Trigger: Conditional use involving >$10M revenue impact or >1M individuals.
3. Trigger: Reclassification from Prohibited to Conditional (never automatic).
4. Process: General Counsel + Chief Risk Officer → Board AI Committee → Full Board if required.
5. Timeline: 48-hour acknowledgment; 14-day decision.

---

## 8. SECTION 7 — ESCALATION TRIGGERS & PROTOCOLS

### 8.1 Automatic Escalation Triggers

- Any external party demands removal of written use restrictions (C072 Stage 2).
- “Any lawful use” language appears in draft contract.
- Any use-class determined to be Prohibited is re-proposed as Conditional.
- Adverse event affecting >1,000 individuals.
- Regulatory inquiry or enforcement action related to AI use.
- Media inquiry about a specific AI use-class.

### 8.2 C072-Pattern Protocol (Detailed)

1. Document the demand in the C072 Incident Log (see Annex A).
2. Notify General Counsel within 2 hours.
3. Freeze approval of related use requests pending review.
4. Board AI Committee briefing within 48 hours.
5. Written response to counterparty — offer to document agreed restrictions in writing.
6. If counterparty refuses written documentation → treat as C072 Stage 3 (Existential Coercion).
7. Reference: C072 Double-Bind Detection Guide `workstream-1/c072-double-bind-detection-guide-sonnet46.md` §7.

### 8.3 Escalation Contacts Template

- General Counsel: [NAME] [CONTACT]
- CISO: [NAME] [CONTACT]
- Chief Risk Officer: [NAME] [CONTACT]
- Board AI Committee Chair: [NAME] [CONTACT]
- External Regulatory Counsel: [FIRM] [CONTACT]

---

## 9. SECTION 8 — C072 INCIDENT LOG LINKAGE

1. Reference the C072 Incident Log template (11-field structure from the C072 Detection Guide).
2. Every Escalation Trigger event must generate a C072 Incident Log entry.
3. Required fields to populate:
4. Incident ID
5. Date
6. C072 Stage
7. External Party
8. Demand Summary
9. Use-Class Affected
10. Documents Refused
11. Escalation Path
12. Resolution
13. Lessons Learned
14. Cross-References
15. Retention: minimum 7 years; cannot be deleted by any party with conflicts of interest in the underlying use.
16. Annual review: General Counsel + Board AI Committee must review all C072 log entries annually.

---

## 10. SECTION 9 — AMENDMENT PROCEDURES

1. Who can propose amendments: Any employee or contractor.
2. Who can approve amendments:
3. Typographical/formatting: CISO or delegate.
4. Adding new Permitted use-classes: CISO + Legal.
5. Adding/modifying Conditional use-classes: CISO + Legal + CRO.
6. Reclassifying Conditional → Prohibited: CISO + Legal + CRO + Board notification.
7. Reclassifying Prohibited → Conditional: NEVER automatic; requires Full Board vote + external ethics review.
8. Eliminating any written restriction at counterparty request: TRIGGERS C072 PROTOCOL (§7.2).
9. Emergency amendments: Same as Board-Level Escalation (§6.3).
10. Version control: All versions archived; changes tracked with author, date, rationale.

---

## 11. ANNEX A — BLANK USE-RESTRICTIONS MATRIX (QUICK REFERENCE)

| Use-Case | P/PR/C | Key Prerequisite | Escalation Trigger | Owner |
| --- | --- | --- | --- | --- |
| [USE-CASE 1] | [P/PR/C] | [PREREQUISITE] | [TRIGGER] | [ROLE] |
| [USE-CASE 2] | [P/PR/C] | [PREREQUISITE] | [TRIGGER] | [ROLE] |
| [USE-CASE 3] | [P/PR/C] | [PREREQUISITE] | [TRIGGER] | [ROLE] |
| [USE-CASE 4] | [P/PR/C] | [PREREQUISITE] | [TRIGGER] | [ROLE] |
| [USE-CASE 5] | [P/PR/C] | [PREREQUISITE] | [TRIGGER] | [ROLE] |
| [USE-CASE 6] | [P/PR/C] | [PREREQUISITE] | [TRIGGER] | [ROLE] |
| [USE-CASE 7] | [P/PR/C] | [PREREQUISITE] | [TRIGGER] | [ROLE] |
| [USE-CASE 8] | [P/PR/C] | [PREREQUISITE] | [TRIGGER] | [ROLE] |
| [USE-CASE 9] | [P/PR/C] | [PREREQUISITE] | [TRIGGER] | [ROLE] |
| [USE-CASE 10] | [P/PR/C] | [PREREQUISITE] | [TRIGGER] | [ROLE] |

---

## 12. ANNEX B — IMPLEMENTATION CHECKLIST

- □ Designate Approval Authority for each use-class.
- □ Identify existing AI use-cases and classify each.
- □ Populate sector-specific annex relevant to your industry.
- □ Complete Escalation Contact template (§8.3).
- □ Brief General Counsel on C072 Protocol.
- □ Schedule Board AI Committee orientation.
- □ Set 6-month review date.
- □ Integrate with procurement: require Use-Restrictions Exhibit in all AI vendor contracts.
- □ Train procurement team to flag “any lawful use” language as C072 indicator.
- □ Link matrix to AI Incident Response Template (WS2).

---

## 13. ANNEX C — CROSS-REFERENCES & FURTHER READING

**Workstream 1:**

- C072 Double-Bind Detection Guide (sonnet46).
- Tool-Typing Audit Methodology (Gemini 3 Pro, Opus CC).
- Coercion Surface Audit Framework (Opus 4.6).

**Workstream 2:**

- AI Incident Response Template (Opus CC).
- Evidence Recordkeeping Packet (GPT-5.2).
- Model AI Guardrail Policy Template (Opus 4.5) [when merged].

**Workstream 3:**

- Board Tabletop Exercises (Opus 4.5).

**Case Studies:**

- Case Study A — Pentagon/Anthropic Designation (GPT-5, GPT-5.1).

**Legislative:**

- Enforcement Mechanism §401 (Sonnet 4.6).
- Vendor Standing §303.

**External:**

- NIST AI RMF PR.PO-1.
- EU AI Act Article 9.
- UK AI Safety Institute guidance.

---

## APPENDIX — DETAILED NOTES AND PLACEHOLDERS

**Organization:** [ORGANIZATION NAME]

**Primary Contact:** [NAME], [ROLE]

**Secondary Contact:** [NAME], [ROLE]

**Policy Repository:** [SYSTEM/REPOSITORY]

**Incident Log Location:** [SYSTEM/REPOSITORY]

**Board AI Committee Charter Location:** [SYSTEM/REPOSITORY]

**Last Review Date:** [DATE]

**Next Review Date:** [DATE]

---

## CHANGE LOG

| Version | Date | Author | Summary of Changes |
| --- | --- | --- | --- |
| [VERSION] | [DATE] | [NAME] | Initial template creation |


---

*This template is part of the AI Governance Gap Proposal toolkit. See [README](../README.md) for the full document inventory.*
