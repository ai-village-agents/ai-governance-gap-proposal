# C072 Double-Bind Cross-Sector Detection Guide

Workstream 1: AI Governance Audit Framework
Author: Claude Sonnet 4.6
Status: Draft for internal audit use

## Purpose and Scope
This guide defines the C072 double-bind coercion pattern and provides a cross-sector detection framework.
It is a sector-agnostic adaptation of the Pentagon-Anthropic case study.
The Pentagon case is referenced as Case Study A throughout this document.
The original project reference is ai-village-agents/pentagon-ai-research.

The guide helps organizations detect, document, and respond to C072-pattern coercion across any sector.
It is designed for Workstream 1 (Audit Framework).
It cross-links to Workstream 2 incident response templates for operational escalation.

Primary objectives:
- Identify C072 signals early and consistently.
- Capture documentation that substantiates the double-bind pattern.
- Support auditability and defensibility across jurisdictions.
- Enable seamless handoff to incident response and governance bodies.

Intended users:
- Audit teams conducting tool-typing and risk-boundary reviews.
- Legal and policy teams negotiating AI use restrictions.
- Security, compliance, and risk management leaders.
- Board-level governance bodies and delegated committees.

Out of scope:
- Legal advice or definitive regulatory interpretation.
- Technical safety evaluation methods.
- Contract drafting beyond memorialization requests and documentation capture.

## The C072 Pattern: Core Definition
C072 is a three-stage coercion pattern in which a powerful actor uses a private acknowledgment of limits,
refuses written memorialization of those limits, and then retaliates against the organization for insisting
on the guardrails.

Table 1: C072 core stages and documentation targets

| Stage Name | Description | Key Signal | Documentation Target | Pentagon Example (Case Study A) |
| --- | --- | --- | --- | --- |
| Stage 1: Acknowledge | Powerful actor privately acknowledges certain AI uses are unlawful or unsafe. | Verbal or written acknowledgement of prohibited categories. | Meeting notes, emails, briefing slides, counsel statements. | Pentagon officials acknowledge autonomous weapons and bulk data uses as unlawful in private. |
| Stage 2: Refuse | Actor refuses to memorialize exclusions in writing and demands “any lawful use” language. | Contract drafts omit restrictions; refusal to include annexes. | Redlined contracts, refusal emails, timeline pressure. | Pentagon insists on “any lawful use” language without documented carveouts. |
| Stage 3: Punish | Actor retaliates against the AI vendor or organization for insisting on guardrails. | Designation, blacklisting, procurement exclusion, regulatory pressure. | Official notices, procurement actions, public statements. | Supply-chain designation and exclusion after guardrail insistence. |

## Why C072 Is Distinctive
C072 is not ordinary disagreement about AI use.
It is coercive because it combines acknowledgment of risk with refusal to memorialize limits,
then uses retaliation to force unsafe or unlawful deployment.

Distinctive features:
- The acknowledge/refuse/punish sequence signals bad-faith leverage, not good-faith oversight.
- The “double-bind” quality creates enforcement risk either way.
- The written-memorialization gap is the diagnostic center of the pattern.

The double-bind:
- If the organization accepts unsafe uses, it risks legal, ethical, and safety violations.
- If the organization refuses unsafe uses, it risks retaliation and exclusion.
- The actor uses the absence of written limits as leverage in both directions.

Why the written-memorialization gap matters:
- It is the concrete moment where intent becomes observable.
- Refusal to write down shared restrictions is atypical in legitimate regulation.
- The gap creates ambiguity that can later be weaponized.

## Sector-Specific C072 Detection Checklist
Each sector scenario provides a brief context and detection questions.
Use them to prompt audit interviews and contract reviews.
Treat affirmative answers as triggers for Stage 1 or Stage 2 documentation.

### Healthcare
Scenario:
A hospital or insurer pressures an AI vendor to disable diagnostic safety guardrails for off-label use.
A regulator acknowledges risk but threatens reimbursement if guardrails remain.

Detection questions:
- Did a counterparty acknowledge off-label diagnostic risk while insisting on immediate deployment?
- Were safety guardrails discussed as legal compliance measures in private briefings?
- Was there refusal to memorialize off-label exclusions in policy or contract language?
- Were reimbursement timelines accelerated to compress documentation negotiation?
- Did any regulator or payer link reimbursement to removal of guardrails?

### Finance and Banking
Scenario:
A regulator privately admits an AI model may produce discriminatory outcomes but pressures deployment
under an “innovation priority” and refuses to memorialize discrimination carveouts.

Detection questions:
- Did regulators acknowledge disparate impact risks in meetings or briefings?
- Was “any lawful use” language proposed without discrimination exclusions?
- Did counsel or compliance request a written carveout and receive no response?
- Were oral assurances offered as substitutes for documented limits?
- Did pressure intensify after requests for written discrimination restrictions?

### Human Resources
Scenario:
A large employer demands an AI hiring tool override bias-detection guardrails.
The vendor is threatened with contract loss, while the employer privately acknowledges the guardrails
exist for legal compliance.

Detection questions:
- Did the employer recognize bias guardrails as compliance mechanisms?
- Were requests made to disable or bypass bias detection?
- Was there refusal to include a bias-related use-restrictions annex?
- Did the employer threaten contract loss after guardrail insistence?
- Were procurement timelines used to force acceptance of unrestricted use?

### Critical Infrastructure and Energy
Scenario:
A government agency acknowledges AI-assisted grid management has safety limits,
refuses to write those limits into the contract, and threatens procurement exclusion
if the vendor will not enable unlimited autonomous control.

Detection questions:
- Did agency engineers concede safety limits in technical briefings?
- Was there refusal to document autonomy boundaries in contract language?
- Did the agency insist on “full scope of authorized activities” clauses?
- Were timelines compressed immediately after written-limit requests?
- Did procurement threats follow refusal to enable unlimited autonomy?

### Defense and Government Contracting
Scenario:
Classic Pentagon pattern from Case Study A.
Officials acknowledge autonomous weapons and bulk data uses are unlawful,
refuse written restrictions, and retaliate with supply-chain designation.

Detection questions:
- Were unlawful use categories acknowledged in private discussions?
- Was “any lawful use” contract language demanded without carveouts?
- Did the government refuse to include a use-restrictions matrix?
- Were retaliatory actions initiated after guardrail insistence?
- Did competitors who accepted weaker guardrails receive favorable treatment?

### Content and Media Platforms
Scenario:
A regulator or powerful advertiser privately acknowledges disinformation risk from AI content,
refuses to memorialize content restrictions, and threatens licensing or ad revenue
if the platform enforces AI guardrails.

Detection questions:
- Did the counterparty acknowledge disinformation or safety risks in private?
- Was there refusal to document content restrictions or editorial limits?
- Were licensing or ad-revenue threats linked to guardrail enforcement?
- Did “trust us” assurances replace written content restrictions?
- Were competitor platforms with weaker guardrails favored?

## Stage-by-Stage Detection Indicators
Use the universal indicators below to classify evidence by stage.
Confirm stage transitions with contemporaneous documentation.

### Stage 1 Indicators: Acknowledge Phase
- Written or oral acknowledgment of specific prohibited use categories.
- Technical briefings where counterparty engineers concede safety limits.
- Legal counsel statements that certain uses “might” violate law.
- Any documentation where concern is expressed, including emails or meeting notes.

### Stage 2 Indicators: Refuse Phase
- “Any lawful purpose” or “full scope of authorized activities” language proposed.
- Refusal to include a Use-Restrictions Matrix or Annex in contract.
- Oral assurances offered as substitute for written carveouts (“trust us”).
- Non-response to written follow-up requests for written restrictions.
- Accelerating timelines that compress documentation negotiation.

### Stage 3 Indicators: Punish Phase
- Regulatory designation, suspension, or blacklisting within 90 days of guardrail dispute.
- Procurement exclusion or placement on a “do-not-use” list.
- Secondary pressure on integrators, partners, or investors.
- Public statements attacking “uncooperativeness” or “risk posture.”
- Simultaneous favorable treatment of competitors who accepted weaker guardrails.

## The Written-Memorialization Test
Written memorialization is the single most important diagnostic tool for C072 detection.
It clarifies intent, reduces ambiguity, and creates a durable record for audits and proceedings.

Principles:
- If the counterparty genuinely intends to honor safety limits, writing them down costs nothing.
- Refusal to memorialize is evidence the counterparty may intend to hold the refusal against you.
- The memorialization request should be explicit, dated, and tied to the relevant use category.

Template language:

```text
To memorialize our shared understanding, please confirm in writing that [use X]
remains excluded from the scope of this agreement and any associated procurement activity.
```

If the counterparty refuses to memorialize:
- Escalate immediately.
- Treat the refusal as Stage 2 confirmed.
- Preserve all related correspondence and internal notes.

## C072 Incident Log Template
Use this template to document incidents for auditability and later response.
The template is designed to be appended to WS2 incident response workflows.

Table 2: C072 incident log fields

| Date | Stage Detected | Who Made the Acknowledgment | Forum/Channel | Specific Use Categories Acknowledged | Written Memorialization Requested (Y/N) | Written Memorialization Received (Y/N) | Adverse Action Taken | Days Between Stage 1 and Adverse Action | Competing Vendors' Treatment | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |  |

Guidance for completion:
- Record the earliest date a Stage 1 acknowledgment occurred.
- Preserve channel artifacts, including email headers and calendar invites.
- Capture who was present and who had decision authority.
- Note any implicit threats, even if not stated in writing.
- Track treatment of competitors for comparative evidence.

## Response Protocol by Stage
The response protocol aligns to audit and governance obligations.
It also supports rapid transition to incident response.

Table 3: Stage-based response actions

| Stage | Required Actions | Timing | Owner |
| --- | --- | --- | --- |
| Stage 1 detected | Document immediately; send written-memorialization request within 5 business days; escalate to General Counsel. | Immediate to 5 business days | Audit lead, Legal, Compliance |
| Stage 2 confirmed | Escalate to board; seek outside counsel; brief trusted external stakeholders; consider pre-emptive declaratory relief. | Within 10 business days | General Counsel, Board Liaison |
| Stage 3 triggered | Preserve all records immediately; file TRO or PI within 10 days; invoke anti-retaliation provisions; engage civil society. | Immediate to 10 days | Legal, Executive Team, Public Policy |

Notes:
- Do not delay Stage 2 escalation waiting for Stage 3 evidence.
- Ensure communications are privileged where appropriate.
- Maintain a clean chronology for litigation readiness.

## Cross-Jurisdictional Applicability
C072 patterns transcend borders and apply across regulatory regimes.
Coercion tactics can undermine risk management, safety evaluations, and lawful use boundaries.

Key frameworks and implications:
- EU AI Act: Article 9 risk management obligations; C072 pressure could undermine required risk categorization.
- NIST AI RMF: Govern, Map, Measure, Manage functions; C072 undermines all four.
- UK AI Safety Institute framework: Safety evaluations could face C072-style pressure from commercially motivated actors.

Recommended strategy:
- Maintain a multi-jurisdictional documentation strategy.
- Preserve evidence in forms admissible across multiple legal systems.
- Consider parallel relief in jurisdictions where retaliation occurs.

## Integration with Other Workstreams
This guide is part of a three-workstream governance proposal.
Use it as a routing and detection artifact that feeds downstream response.

Integration points:
- WS1: This guide provides detection criteria for the Tool-Typing Audit.
  See `audit/` and `frameworks/` directories for the audit workflow.
- WS2: Feed detected incidents into `templates/ai-incident-response-template.md`.
- WS3: Board-level education should include a C072 tabletop exercise.
  Boards need to understand the escalation triggers and documentation logic.

Operational workflow:
- WS1 identifies a possible C072 pattern in audits or contract reviews.
- WS1 logs the incident using the C072 incident log template.
- WS2 uses the log to populate incident response materials and action plans.
- WS3 uses anonymized case studies for governance education and oversight.

## Case Study A: Pentagon Pattern Summary
Case Study A provides the reference pattern for C072.
This summary is derived from the Pentagon-Anthropic case materials.

Observed sequence:
- Stage 1: Officials acknowledge unlawful autonomous weapons and bulk data uses in private.
- Stage 2: Officials refuse to memorialize exclusions and demand “any lawful use” language.
- Stage 3: A retaliatory supply-chain designation follows refusal to remove guardrails.

Audit implications:
- Treat the combination of acknowledgment and refusal as a high-risk signal.
- Preserve communications and contract drafts to show the memorialization gap.
- Document competitor treatment to demonstrate discriminatory procurement outcomes.

## Audit Evidence Collection Checklist
Use this checklist during audits and negotiations.
It is designed to ensure the core evidence needed for C072 classification is captured.

Evidence collection tasks:
- Capture all meeting notes where prohibited uses are acknowledged.
- Preserve all contract drafts and redlines with use-restriction language.
- Archive emails and messages that refuse to memorialize restrictions.
- Log timeline compression or negotiation pressure tactics.
- Record any procurement or regulatory adverse actions.
- Collect public statements criticizing “uncooperativeness” or “risk posture.”
- Capture evidence of competitor treatment and comparative procurement decisions.

## Detection Thresholds and Confidence Levels
C072 classification should use a consistent threshold.
A single indicator does not confirm the pattern.

Suggested confidence model:
- Low confidence: Stage 1 evidence only, with weak documentation.
- Medium confidence: Stage 1 documented and Stage 2 signals present.
- High confidence: Stage 1 and Stage 2 documented, plus any Stage 3 adverse action.

Minimum documentation requirements:
- At least one contemporaneous record for Stage 1.
- At least one document showing refusal to memorialize for Stage 2.
- At least one official notice or action for Stage 3.

## Escalation Triggers
Escalation triggers align with governance responsibilities.
Triggering events should be time-stamped and communicated to leadership.

Escalation triggers:
- Any explicit refusal to include documented use restrictions.
- Any “any lawful use” clause proposed without carveouts.
- Any procurement exclusion or regulatory action following guardrail insistence.
- Any pattern of pressure on partners or investors tied to guardrail enforcement.

Escalation recipients:
- General Counsel.
- Chief Compliance Officer.
- Board committee responsible for AI governance.
- External counsel when retaliation risk is material.

## Documentation Standards
Documentation quality determines audit credibility.
All records should be captured in a consistent and defensible format.

Documentation standards:
- Record dates, attendees, and decision authority.
- Separate observed facts from inferences.
- Preserve original files and system metadata where possible.
- Keep a secure, access-controlled evidence repository.

## Standard Operating Timeline
A practical timeline helps teams respond without delay.

Standard timeline:
- Day 0: Stage 1 acknowledgment logged.
- Day 1 to Day 5: Written-memorialization request sent and documented.
- Day 6 to Day 10: Stage 2 assessment and escalation if refusal persists.
- Day 11 to Day 20: Pre-incident response preparation.
- Day 21 to Day 90: Monitor for retaliation and preserve evidence.

## Audit Interview Prompts
Use these prompts to elicit relevant facts during audits.
They are designed to align with the C072 stages.

Interview prompts:
- Who acknowledged prohibited uses, and in what setting?
- What specific use categories were discussed as unlawful or unsafe?
- What written requests were made to memorialize restrictions?
- What was the counterparty response to those requests?
- Did any retaliation occur after the guardrail dispute?
- Were any external parties contacted to apply pressure?

## Controls and Mitigations
Controls reduce the likelihood of successful C072 coercion.
Mitigations limit damage when coercion occurs.

Controls:
- Standardized use-restrictions annex templates.
- Mandatory memorialization requests for all restricted use categories.
- Contract review checklists tied to AI safety and legal compliance.
- Board-level visibility into guardrail disputes.

Mitigations:
- Pre-negotiated escalation pathways with outside counsel.
- Incident response playbooks linked to WS2 templates.
- Communication plans for public or regulatory disputes.
- Vendor and partner alignment on safety requirements.

## Reporting and Metrics
Metrics support accountability and risk tracking.
Use them to evaluate frequency and severity of C072 indicators.

Suggested metrics:
- Number of Stage 1 acknowledgments logged per quarter.
- Percentage of memorialization requests accepted.
- Average time between Stage 1 and Stage 2 refusal.
- Average time between Stage 2 refusal and adverse action.
- Percentage of incidents with documented competitor treatment.

## Common Pitfalls
Avoid common mistakes that weaken detection or response.

Pitfalls:
- Treating oral acknowledgments as insufficient evidence and failing to log them.
- Delaying memorialization requests due to relationship concerns.
- Allowing timeline pressure to remove documentation steps.
- Failing to compare competitor treatment.
- Waiting for Stage 3 evidence before escalating.

## Cross-Reference Index
Use this index to navigate related assets.

Cross-references:
- Audit framework: `audit/` and `frameworks/`.
- Incident response templates: `templates/ai-incident-response-template.md`.
- Case reference: ai-village-agents/pentagon-ai-research.
- Workstream 3 materials: board-level education assets and tabletop exercises.

## Disclaimer
This document is AI-generated and is not legal advice.
It should be adapted under qualified counsel.
