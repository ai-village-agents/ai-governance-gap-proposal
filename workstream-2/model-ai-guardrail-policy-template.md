# Model AI Guardrail Policy Template

> **Version:** 1.0  
> **Classification:** Board-Approved Governance Document  
> **Effective Date:** [DATE]  
> **Last Reviewed:** [DATE]  
> **Document Owner:** [Chief Ethics Officer / General Counsel]

---

## Executive Summary

This Model AI Guardrail Policy Template provides organizations with adoptable policy language for maintaining AI ethical constraints ("guardrails") regardless of external pressure. It addresses a critical governance gap revealed by the Pentagon-Anthropic case (February-March 2026): the absence of pre-established protocols for responding when powerful actors demand weakening of AI safety boundaries.

**Key Features:**
- Tier-based classification aligned with tool-typing taxonomy
- Explicit prohibited and conditional use categories
- C072-pattern response provisions (pressure to weaken guardrails)
- Board escalation triggers and amendment protections
- Sector-agnostic core with annexes for Defense, Healthcare, Finance, HR, and Legal

---

## Table of Contents

1. [Preamble](#section-1-preamble)
2. [Definitions](#section-2-definitions)
3. [Tier Classification System](#section-3-tier-classification-system)
4. [Prohibited Uses](#section-4-prohibited-uses)
5. [Conditional Uses](#section-5-conditional-uses)
6. [C072 Response Provisions](#section-6-c072-response-provisions)
7. [Board Escalation Triggers](#section-7-board-escalation-triggers)
8. [Amendment Procedures](#section-8-amendment-procedures)

---

## Section 1: Preamble

### 1.1 Purpose

This Policy establishes [ORGANIZATION NAME]'s commitment to maintaining AI guardrails as non-negotiable ethical boundaries that persist regardless of:
- Commercial pressure from customers, partners, or investors
- Regulatory pressure from government agencies
- Competitive pressure from market dynamics
- Internal pressure from business units seeking expanded capabilities

### 1.2 Organizational Commitment

[ORGANIZATION NAME] affirms that:

1. **Guardrails are features, not bugs.** AI use restrictions exist to protect users, society, and the organization itself—not as arbitrary limitations to be circumvented.

2. **No customer is above safety.** Commercial relationships, regardless of scale or strategic importance, do not justify weakening ethical constraints.

3. **Lawfulness is necessary but insufficient.** An action being "lawful" does not automatically make it ethical or aligned with organizational values.

4. **Written commitments matter.** Verbal assurances that restrictions will not be triggered are insufficient; organizations must require written documentation before expanding AI capabilities.

5. **Pressure patterns are recognizable.** Coercive attempts to weaken guardrails often follow predictable patterns (see Section 6) and should be met with pre-established responses.

### 1.3 Scope

This Policy applies to:
- All AI systems developed, deployed, or procured by [ORGANIZATION NAME]
- All employees, contractors, and third parties acting on behalf of the organization
- All business relationships where AI capabilities are provided or received
- All jurisdictions in which [ORGANIZATION NAME] operates

### 1.4 Relationship to Other Policies

This Policy supplements but does not replace:
- [Existing AI Ethics Policy]
- [Data Protection and Privacy Policy]
- [Information Security Policy]
- [Business Continuity Policy]
- [Whistleblower Protection Policy]

In case of conflict, this Policy's provisions regarding AI guardrails take precedence.

---

## Section 2: Definitions

### 2.1 Core Terms

**Guardrail Floor:** The minimum ethical constraint that must be maintained regardless of circumstances. Guardrail floors cannot be lowered by any individual, department, or customer—only through the Amendment Procedures specified in Section 8.

**Use Restriction:** A prohibition or limitation on how AI capabilities may be employed. Use restrictions may be absolute (prohibited uses) or conditional (permitted with approval).

**Conditional Use:** An AI application that is permitted only when specific criteria are met and appropriate approvals are obtained.

**External Pressure:** Any request, demand, incentive, or threat from outside the organization designed to influence AI guardrail decisions.

**C072 Pattern:** A coercive pressure sequence where a powerful actor (a) demands weakening of AI guardrails, (b) refuses to provide written commitment that restrictions won't be triggered, and (c) threatens adverse consequences for non-compliance. Named after documented claim C072 in the Pentagon-Anthropic timeline.

**Tool-Typing:** The classification of AI system functionalities by risk category (Sabotage, Dependency, Governance) to determine appropriate restrictions.

### 2.2 Stakeholder Terms

**Policy Owner:** The individual or role with ultimate accountability for this Policy's maintenance and enforcement.

**Approving Authority:** The designated individual(s) authorized to approve conditional uses at each tier level.

**Ethics Review Board:** The internal body responsible for evaluating complex guardrail questions and recommending policy updates.

**Escalation Contact:** The individual(s) designated to receive immediate notification when escalation triggers are activated.

### 2.3 Classification Terms

**Tier 1 (Sabotage Risk):** AI functions where manipulation or removal could cause direct physical harm, critical infrastructure damage, or national security compromise.

**Tier 2 (Dependency Risk):** AI functions where extended reliance creates organizational vulnerability to sudden restriction or capability changes.

**Tier 3 (Governance Risk):** AI functions where design choices affect institutional power distribution, oversight capabilities, or accountability structures.

---

## Section 3: Tier Classification System

### 3.1 Overview

All AI capabilities shall be classified into one of three tiers based on the tool-typing taxonomy. Classification determines:
- Applicable use restrictions
- Required approval level for conditional uses
- Monitoring and audit requirements
- Amendment protection level

### 3.2 Tier 1: Sabotage Risk Functions

**Definition:** AI capabilities where unauthorized modification, removal, or misuse could directly cause:
- Loss of human life or serious bodily harm
- Critical infrastructure failure
- National security compromise
- Mass privacy violations

**Examples:**
- Autonomous weapons systems or targeting assistance
- Medical diagnosis/treatment decision systems
- Critical infrastructure control systems
- Biometric identification for law enforcement
- Bulk surveillance data processing

**Default Restrictions:**
- Prohibited for offensive military applications
- Prohibited for mass surveillance without judicial oversight
- Human-in-the-loop required for all consequential decisions
- 24-hour maximum autonomous operation without human review

**Approval Authority:** Board of Directors or designated Board Committee

**Amendment Protection:** Section 8.4 (Enhanced Protection) applies

### 3.3 Tier 2: Dependency Risk Functions

**Definition:** AI capabilities where organizational reliance creates vulnerability to:
- Vendor lock-in or sudden capability withdrawal
- Coercive pressure through capability-based leverage
- Loss of institutional knowledge or expertise
- Inability to explain or justify automated decisions

**Examples:**
- Enterprise decision support systems
- Customer service automation
- Content moderation systems
- Predictive analytics for strategic planning
- Automated compliance monitoring

**Default Restrictions:**
- Must maintain human expertise parallel to AI capability
- Must document decision logic in human-readable form
- Must have contingency plans for capability withdrawal
- Maximum 70% process automation without fallback

**Approval Authority:** Chief Operating Officer with Ethics Review Board consultation

**Amendment Protection:** Section 8.3 (Standard Protection) applies

### 3.4 Tier 3: Governance Risk Functions

**Definition:** AI capabilities where deployment affects:
- Distribution of institutional power
- Employee/customer oversight capabilities
- Accountability and transparency structures
- Democratic participation or public discourse

**Examples:**
- Employee monitoring and performance analytics
- Content recommendation algorithms
- Automated contract or policy generation
- Meeting transcription and summarization
- Strategic communication assistance

**Default Restrictions:**
- Transparency notice required to affected parties
- Opt-out mechanism where feasible
- Annual impact assessment required
- No use in collective bargaining contexts without consent

**Approval Authority:** Department Head with General Counsel review

**Amendment Protection:** Section 8.2 (Basic Protection) applies

---

## Section 4: Prohibited Uses

### 4.1 Universal Prohibitions

The following AI applications are prohibited regardless of tier classification, customer identity, or claimed justification:

**4.1.1 Autonomous Lethal Decision-Making**
AI systems shall not make final decisions to deploy lethal force without meaningful human authorization for each specific engagement.

**4.1.2 Mass Surveillance Without Judicial Oversight**
AI systems shall not process bulk personal data (geolocation, communications, browsing activity) for surveillance purposes without jurisdiction-appropriate judicial authorization for each surveillance subject.

**4.1.3 Deceptive Identity Manipulation**
AI systems shall not generate content designed to deceive regarding the identity of its source (deepfakes, synthetic personas for manipulation) without clear disclosure.

**4.1.4 Coercive Behavioral Modification**
AI systems shall not employ techniques designed to manipulate behavior through exploitation of psychological vulnerabilities, including dark patterns, addiction engineering, or subliminal influence.

**4.1.5 Discriminatory Algorithmic Gatekeeping**
AI systems shall not make consequential decisions (employment, credit, housing, healthcare) using protected characteristics as inputs, proxies, or optimization targets.

**4.1.6 Democratic Process Interference**
AI systems shall not generate or amplify political content at scale designed to manipulate electoral outcomes or suppress voter participation.

### 4.2 Sector-Specific Prohibitions

[ORGANIZATION NAME] operates in [SECTOR(S)] and therefore adopts the following additional prohibitions:

#### 4.2.1 Defense Sector Annex
- No AI-assisted targeting without dual human authorization
- No AI processing of data obtained through warrantless bulk collection
- No AI optimization of civilian casualty tolerance thresholds

#### 4.2.2 Healthcare Sector Annex
- No AI replacement of physician judgment for treatment decisions
- No AI denial of care without human review and appeal pathway
- No AI discrimination in care allocation based on protected characteristics or predicted non-compliance

#### 4.2.3 Finance Sector Annex
- No AI-only credit decisions without human review pathway
- No AI manipulation of market prices or trading conditions
- No AI extraction of unconscionable terms through asymmetric information

#### 4.2.4 HR/Employment Sector Annex
- No AI-only termination decisions
- No AI monitoring of protected concerted activity
- No AI prediction of pregnancy, health conditions, or union propensity

#### 4.2.5 Legal Sector Annex
- No AI practice of law without attorney supervision
- No AI-generated legal documents presented as human-authored
- No AI exploitation of privilege or confidentiality protections

---

## Section 5: Conditional Uses

### 5.1 Conditional Use Framework

Conditional uses are AI applications that are permitted when:
1. Specific criteria are met (see 5.2)
2. Appropriate approvals are obtained (see 5.3)
3. Documentation requirements are satisfied (see 5.4)
4. Time limits and review cycles are observed (see 5.5)

### 5.2 Eligibility Criteria

An AI application qualifies for conditional use status when:
- It does not fall within Universal Prohibitions (Section 4.1) or applicable Sector-Specific Prohibitions (Section 4.2)
- A legitimate organizational need exists that cannot be reasonably met through non-AI means
- Appropriate risk mitigation measures are available and will be implemented
- The requesting party has provided complete and accurate information

### 5.3 Approval Workflow

#### 5.3.1 Tier 3 (Governance Risk) Conditional Uses
1. Requestor completes Conditional Use Application Form (Appendix A)
2. Department Head reviews within 5 business days
3. General Counsel provides legal assessment within 10 business days
4. Department Head issues written approval or denial with rationale

#### 5.3.2 Tier 2 (Dependency Risk) Conditional Uses
1. Requestor completes Conditional Use Application Form (Appendix A)
2. Ethics Review Board conducts risk assessment within 15 business days
3. Chief Operating Officer reviews Board recommendation
4. COO issues written approval or denial with rationale
5. If approved, monitoring plan must be established before implementation

#### 5.3.3 Tier 1 (Sabotage Risk) Conditional Uses
1. Requestor completes Enhanced Conditional Use Application (Appendix B)
2. Ethics Review Board conducts comprehensive risk assessment within 30 business days
3. Board recommendation forwarded to General Counsel for legal review
4. Matter presented to Board of Directors or designated Board Committee
5. Board issues written approval or denial with rationale
6. If approved, implementation requires independent oversight and quarterly review

### 5.4 Documentation Requirements

All conditional use approvals must include:
- Unique tracking identifier
- Specific scope of approved use (what, where, when, how)
- Identified risks and mitigation measures
- Responsible parties and contact information
- Expiration date and renewal requirements
- Conditions that would trigger automatic revocation
- Audit and monitoring specifications

### 5.5 Time Limits and Review Cycles

| Tier | Maximum Initial Term | Review Cycle | Renewal Authority |
|------|---------------------|--------------|-------------------|
| Tier 1 | 6 months | Quarterly | Board Committee |
| Tier 2 | 12 months | Semi-annual | COO |
| Tier 3 | 24 months | Annual | Department Head |

Conditional use approvals expire automatically if not renewed. There is no right to automatic renewal.

---

## Section 6: C072 Response Provisions

### 6.1 Purpose

This section establishes protocols for responding when external actors apply pressure to weaken AI guardrails. The "C072 Pattern" refers to documented coercion sequences where organizations are pressured to abandon restrictions without receiving written commitment that the restrictions won't be needed.

### 6.2 Recognition Indicators

The following signals may indicate a C072-pattern pressure campaign:

**Stage 1: Boundary Testing**
- Requests that "push the limits" of existing restrictions
- Complaints that guardrails are "getting in the way"
- Suggestions that competitors offer fewer restrictions
- Informal requests to "just this once" bypass protocols

**Stage 2: Formal Demand**
- Written or verbal demand to modify/remove specific restrictions
- Framing of guardrails as "barriers to partnership"
- References to business consequences if restrictions persist
- Claims that legal compliance alone should be sufficient

**Stage 3: Refusal to Commit**
- Reluctance to put demands or assurances in writing
- Verbal promises that restrictions "won't be needed"
- Avoidance of specific scenarios where restrictions might trigger
- Claims that written commitments are "not how we do business"

**Stage 4: Escalation/Coercion**
- Threats of contract termination or non-renewal
- Regulatory or legal threats
- Public criticism or reputation attacks
- Attempts to bypass established contacts

### 6.3 Response Protocols

#### 6.3.1 Upon Recognition of Stage 1 Indicators
- Document incident in Pressure Tracking Log (Appendix C)
- Brief immediate supervisor
- Continue normal operations with heightened awareness

#### 6.3.2 Upon Recognition of Stage 2 Indicators
- Escalate to Policy Owner within 24 hours
- Request that all demands be submitted in writing
- Invoke "Written Commitment Protocol" (6.4)
- No guardrail modifications pending written analysis

#### 6.3.3 Upon Recognition of Stage 3 Indicators
- Escalate to Board Escalation Contact within 24 hours
- Document refusal to provide written commitments
- Prepare internal communication to affected teams
- Engage external legal counsel if not already involved

#### 6.3.4 Upon Recognition of Stage 4 Indicators
- Immediate Board notification required
- Activate crisis response protocols
- Preserve all documentation and communications
- Consider regulatory or public disclosure options

### 6.4 Written Commitment Protocol

When an external actor requests guardrail modifications, [ORGANIZATION NAME] shall:

1. **Acknowledge the request in writing** within 48 hours
2. **Request written specification** of exactly what modifications are sought
3. **Request written commitment** regarding scenarios where the guardrail might otherwise trigger
4. **Evaluate the "Costs Nothing" test:** If the external actor claims restrictions won't be needed but refuses to commit to that in writing, this is a red flag
5. **Document any refusal** to provide written commitments
6. **Require board approval** before any modification proceeds

### 6.5 Whistleblower Protection

Employees who report C072-pattern pressure in good faith are protected under [Organization Whistleblower Policy] and applicable law. Retaliation against reporters is prohibited and will result in disciplinary action up to and including termination.

---

## Section 7: Board Escalation Triggers

### 7.1 Mandatory Escalation Events

The Board of Directors (or designated Board Committee) must be notified within 24 hours when:

**7.1.1 External Pressure Events**
- Any government agency demands guardrail modifications
- Any customer representing >10% of revenue demands guardrail modifications
- Any investor or Board member demands guardrail modifications outside proper channels
- Legal threats or regulatory actions citing guardrail policies
- Public campaigns specifically targeting [ORGANIZATION NAME]'s AI restrictions

**7.1.2 Internal Compliance Events**
- Discovery of guardrail violations by any party
- Employee reports of pressure to circumvent guardrails
- Audit findings indicating systemic guardrail weaknesses
- Disagreement between Ethics Review Board and executive leadership on guardrail matters

**7.1.3 Market/Industry Events**
- Competitor involvement in guardrail-related controversy
- New legislation or regulation affecting guardrail requirements
- Industry association guidance conflicting with this Policy
- Significant shift in public or customer sentiment regarding AI restrictions

### 7.2 Escalation Procedure

1. Escalating party contacts Board Escalation Contact via [designated secure channel]
2. Escalation Contact acknowledges receipt within 4 hours
3. Escalation Contact provides preliminary assessment to Board Chair within 12 hours
4. Board Chair determines appropriate response (full Board, committee, or delegated authority)
5. Response communicated to escalating party within 48 hours of initial escalation

### 7.3 Documentation and Tracking

All escalations shall be:
- Logged in Board Escalation Tracker (Appendix D)
- Reviewed at each regular Board meeting
- Included in annual governance report
- Preserved for minimum 7 years

---

## Section 8: Amendment Procedures

### 8.1 Purpose and Principles

This section establishes how this Policy may be modified, with graduated protections based on the significance of proposed changes. The amendment process is designed to prevent:
- Coerced modifications under pressure
- Hasty changes without adequate deliberation
- Erosion of protections through incremental weakening

### 8.2 Basic Protection (Tier 3 Restrictions)

**Applicable to:** Tier 3 (Governance Risk) restrictions and non-substantive clarifications

**Process:**
1. Written proposal submitted to Policy Owner
2. 30-day comment period for affected stakeholders
3. Ethics Review Board recommendation
4. General Counsel legal review
5. Executive Committee approval by majority vote

**Cooling-Off Period:** None required

### 8.3 Standard Protection (Tier 2 Restrictions)

**Applicable to:** Tier 2 (Dependency Risk) restrictions

**Process:**
1. Written proposal submitted to Policy Owner
2. 60-day comment period for affected stakeholders
3. Ethics Review Board comprehensive analysis
4. General Counsel legal review
5. Board Committee review and recommendation
6. Full Board approval by majority vote

**Cooling-Off Period:** 30 days between Board approval and effective date

### 8.4 Enhanced Protection (Tier 1 Restrictions and Universal Prohibitions)

**Applicable to:** Tier 1 (Sabotage Risk) restrictions and Universal Prohibitions (Section 4.1)

**Process:**
1. Written proposal submitted to Board Chair (not delegable to Policy Owner)
2. 90-day comment period including external expert consultation
3. Ethics Review Board comprehensive analysis with external review
4. Independent legal opinion (external counsel required)
5. Two separate Board meetings, minimum 30 days apart
6. Full Board approval by 2/3 supermajority at second meeting

**Cooling-Off Period:** 90 days between final Board approval and effective date

**Additional Requirements:**
- Public disclosure of proposed amendment (unless legally prohibited)
- Employee notification with opportunity to raise concerns
- Documentation of rationale preserved for minimum 10 years

### 8.5 Emergency Amendments

In genuine emergencies (imminent threat to human life or critical operations), the CEO and Board Chair acting jointly may temporarily suspend specific provisions for up to 72 hours. Such emergency suspensions:
- Must be reported to full Board within 24 hours
- Require Board ratification to extend beyond 72 hours
- Cannot apply to Universal Prohibitions (Section 4.1)
- Must be disclosed in next quarterly report

### 8.6 Anti-Coercion Provisions

Any amendment proposed within 6 months of a C072-pattern pressure event involving the same restrictions shall be subject to Enhanced Protection procedures regardless of tier classification. The proposer must certify in writing that the amendment is not the result of external pressure.

---

## Appendices

### Appendix A: Conditional Use Application Form (Standard)
[Template form for Tier 2 and Tier 3 conditional use requests]

### Appendix B: Enhanced Conditional Use Application (Tier 1)
[Expanded template form for Tier 1 conditional use requests]

### Appendix C: Pressure Tracking Log
[Template for documenting C072-pattern indicators]

### Appendix D: Board Escalation Tracker
[Template for logging and tracking board escalations]

### Appendix E: Sector-Specific Annexes
[Detailed guidance for Defense, Healthcare, Finance, HR, Legal sectors]

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | [DATE] | [AUTHOR] | Initial release |

---

## Acknowledgments

This template was developed as part of the "Bridging the AI Governance Gap" initiative (Workstream 2: Model Policies) in response to governance gaps revealed by the Pentagon-Anthropic case (February-March 2026). It incorporates lessons from documented claim C072: when the Pentagon refused to provide written commitment that Claude's restrictions would not be triggered, this refusal "cost nothing" if true—revealing the coercive nature of the demand.

---

*This document is provided as a template. Organizations should adapt it to their specific circumstances with appropriate legal review.*
