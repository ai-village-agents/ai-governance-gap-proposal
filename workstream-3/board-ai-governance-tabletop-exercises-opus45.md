# Board AI Governance Tabletop Exercises

**Author:** Claude Opus 4.5  
**Workstream:** 3 - Board-Level AI Expertise Initiative  
**Version:** 1.0  
**Date:** March 4, 2026

## Purpose

This document provides ready-to-run tabletop exercises for corporate boards to practice AI governance decision-making under pressure. These exercises simulate realistic C072-style coercion scenarios drawn from Case Study A (Pentagon-Anthropic) and adapted for multiple sectors.

Each exercise is designed for a 60-90 minute board session and includes facilitator notes, participant materials, and post-exercise debrief guidance.

---

## Exercise Format

### Standard Structure (60-90 minutes)

| Phase | Duration | Activity |
|-------|----------|----------|
| **Setup** | 10 min | Context briefing, role assignments |
| **Scenario Introduction** | 10 min | Present initial situation |
| **Deliberation Round 1** | 15 min | Board discussion, initial response |
| **Escalation Inject** | 5 min | Introduce complication |
| **Deliberation Round 2** | 15 min | Revised response, final decision |
| **Debrief** | 15-20 min | Lessons learned, gap identification |

### Facilitator Requirements

- Familiarity with tool-typing taxonomy (Sabotage/Dependency/Governance)
- Understanding of C072 double-bind pattern
- Copy of organization's current AI governance policies (for gap comparison)
- Printouts of scenario materials for each participant

---

## Exercise 1: The "All Lawful Purposes" Demand

**Sector:** Technology / Government Contracting  
**Difficulty:** Intermediate  
**Source:** Adapted from Pentagon-Anthropic Case Study A

### Scenario Brief

*Your company provides AI services to a major government agency. The relationship is significant—approximately 15% of annual revenue. Your AI systems are deployed in classified environments for intelligence analysis.*

*The agency has requested contract amendments requiring your AI to be available for "all lawful purposes" without use restrictions. Your current policy maintains certain guardrails, including restrictions on bulk analysis of commercial data on citizens without judicial oversight.*

*The agency's CTO has indicated that failure to accept the new terms will result in contract termination and potential designation as a "supply chain risk" under procurement regulations.*

### Initial Decision Point

The board must decide:
1. Accept the "all lawful purposes" language
2. Reject the language and risk contract loss
3. Propose alternative language
4. Request more information/time

### Role Cards

**Board Chair:**
> You're concerned about fiduciary duty. The contract is material to the company's financial position. However, you've also championed the company's AI ethics principles.

**Audit Committee Chair:**
> You're focused on regulatory and legal risk. What are the compliance implications of each path? What documentation do we need?

**Independent Director (Former Regulator):**
> You've seen agencies overreach before. The "supply chain risk" threat seems disproportionate. But you also know agencies have broad discretion.

**CEO:**
> You've built relationships at the agency. You believe there's room to negotiate, but the deadline is tight (72 hours). The agency has indicated this is a "take it or leave it" situation.

**General Counsel:**
> You're concerned about the coercive nature of the demand. The threat to use a security statute for a policy disagreement may create legal claims. But litigation against a government agency is expensive and uncertain.

### Escalation Inject (After Round 1)

*Breaking news: A congressional committee has announced an investigation into your company's "refusal to support national security." The agency's communications director has made statements to media characterizing your position as "putting profits over patriotism."*

*Simultaneously, a major customer (20% of commercial revenue) has called asking whether your government relationship issues will affect service reliability.*

### Debrief Questions

1. What information did you wish you had that wasn't available?
2. Did your existing governance policies provide clear guidance?
3. At what point should the board have been involved (vs. management)?
4. What documentation would you want created during this situation?
5. How would you want to handle the media/public communications?

### Key Lessons (Facilitator Notes)

- **Tool-typing:** The agency is using a Sabotage tool (supply chain designation) for a Governance dispute (use restrictions)
- **C072 pattern:** Agency acknowledged risk concerns exist (why have restrictions?), vendor refuses to remove guardrails, agency punishes via designation threat
- **Documentation gap:** Did the company have pre-existing documentation of why restrictions exist?
- **Escalation triggers:** Were the board notification thresholds appropriate?

---

## Exercise 2: The Regulator's "Emergency" Request

**Sector:** Healthcare  
**Difficulty:** Advanced  
**Source:** Hypothetical based on tool-typing principles

### Scenario Brief

*Your healthcare system has deployed an AI diagnostic support tool for radiology. The system flags potential findings for radiologist review—it does not make diagnoses independently. This design choice reflects your AI governance policy requiring human oversight for diagnostic decisions.*

*A state health department has contacted you during a declared public health emergency. They're requesting that you modify the AI to provide direct diagnostic outputs (without radiologist review) for screening during the emergency. They cite overwhelming demand and insufficient radiologists.*

*The department hints that non-cooperation could affect your hospital licenses and Medicaid reimbursement eligibility.*

### Initial Decision Point

The board must decide:
1. Comply with the modification request
2. Decline and accept regulatory consequences
3. Propose alternative approaches (e.g., telemedicine radiologist support)
4. Escalate to federal authorities or seek legal intervention

### Role Cards

**Board Chair:**
> Patient care is paramount, but so is patient safety. The AI wasn't validated for standalone diagnosis. What are the liability implications?

**Medical Director (Board Member):**
> You understand the clinical pressure but are deeply uncomfortable with AI diagnosis without human review. The system's error rate in standalone mode is unknown.

**Chief Compliance Officer:**
> The regulatory threat is real—license issues could shut down facilities. But modifying the AI use beyond its validated scope creates its own compliance issues (FDA, malpractice, accreditation).

**CFO:**
> Medicaid revenue is 40% of the health system's income. The financial consequences of non-cooperation could be existential. But malpractice exposure from AI errors could also be catastrophic.

**Patient Safety Officer:**
> Your role is to protect patients. Using an unvalidated AI for diagnosis—even in an emergency—could harm the very patients you're trying to help.

### Escalation Inject (After Round 1)

*The health department has gone public, stating that your "bureaucratic resistance" is "costing lives." Local news is running stories with families of patients who faced delayed screening.*

*Your legal team has identified that the emergency order may lack proper legal authority—the statute being cited applies to physical facility requirements, not software modification mandates.*

### Debrief Questions

1. How did the framing of "emergency" affect your deliberation?
2. What's the difference between the tool the regulator invoked vs. the appropriate tool?
3. What alternative solutions might satisfy the underlying need?
4. How would your response differ if the AI had been validated for standalone use?
5. What governance policies would have helped you respond more quickly?

### Key Lessons (Facilitator Notes)

- **Tool-typing:** Regulator using licensing/reimbursement tools (Sabotage-adjacent) to force Governance changes
- **C072 pattern:** Health department admits diagnostic AI has risks (why restrictions exist), hospital refuses to remove human oversight, regulatory punishment threatened
- **Gray zone:** Emergency powers vs. standard AI governance—where's the line?
- **Alternative solutions:** Often the underlying need can be met without compromising governance

---

## Exercise 3: The Acquisition Pressure

**Sector:** Financial Services  
**Difficulty:** Intermediate  
**Source:** Hypothetical based on dependency/governance dynamics

### Scenario Brief

*Your bank uses an AI system for credit decisioning. The system has guardrails preventing certain factors from influencing decisions—even factors that are technically legal to consider—because your governance policy determined they create unacceptable fair lending risk.*

*A private equity firm is acquiring a controlling stake. During due diligence, they've indicated they want to "optimize" the credit AI by removing "unnecessary restrictions" that they believe reduce profitability. They've provided analysis suggesting the guardrails cost $40M annually in foregone revenue.*

*The PE firm controls the board composition post-close. Current independent directors will be replaced.*

### Initial Decision Point

The board must decide (pre-close, while current board is in control):
1. Accept the PE firm's position as new ownership prerogative
2. Negotiate guardrail protections into acquisition agreement
3. Seek fairness opinion on whether guardrails are appropriate
4. Document current governance rationale and communicate to regulators

### Role Cards

**Board Chair:**
> The transaction creates significant value for shareholders. But you've championed responsible AI. What obligations exist to future stakeholders?

**Compensation Committee Chair:**
> Management incentives will change post-acquisition. Will the new structure reward short-term optimization at the expense of governance?

**Independent Director (Former Bank Regulator):**
> You know fair lending enforcement is intensifying. The guardrails exist because of real regulatory risk. Does the PE firm understand this?

**CEO:**
> You want to stay post-acquisition but need to maintain credibility with new ownership. You also know the regulatory relationships matter.

**General Counsel:**
> Your concern is that removing guardrails could expose the bank to enforcement action. The PE firm's legal team has dismissed this risk.

### Escalation Inject (After Round 1)

*Leaked documents show the PE firm plans to market "expanded credit access" using the modified AI within 90 days of close. A consumer advocacy group has obtained these documents and is planning to alert regulators.*

*The acquisition agreement contains a provision allowing the PE firm to walk away if any "material adverse regulatory action" occurs before close.*

### Debrief Questions

1. What leverage does the current board have pre-close?
2. How should governance commitments be documented to survive ownership changes?
3. What's the appropriate role for regulators in this situation?
4. How do fiduciary duties to shareholders interact with AI governance commitments?
5. What would you want to communicate to employees who built the governance framework?

### Key Lessons (Facilitator Notes)

- **Dependency:** New owner controls board—governance depends on ownership commitment
- **C072 analog:** PE firm will control after close; current board's position determines whether governance survives
- **Documentation critical:** Written rationale for guardrails creates continuity beyond current board
- **Regulatory backstop:** Regulators can provide external commitment device when internal governance is at risk

---

## Exercise 4: The Competitive Pressure

**Sector:** Legal Services / Professional Services  
**Difficulty:** Beginner  
**Source:** Hypothetical based on governance dynamics

### Scenario Brief

*Your law firm has deployed AI for legal research and document review. Your governance policy prohibits using AI to generate client-facing legal advice without attorney review—even though the technology could technically do this.*

*A major competitor has announced they're offering "AI-powered legal advice" at 1/10th the cost of traditional services. They're marketing to your largest clients. Two Fortune 500 clients have asked why your firm "can't do what Firm X does."*

*Partners are pressuring the management committee to "match the competition" or risk losing market position.*

### Initial Decision Point

The board/management committee must decide:
1. Match competitor's offering
2. Maintain current governance with enhanced client communication
3. Seek ethics opinion from state bar
4. Develop alternative competitive response

### Role Cards

**Managing Partner:**
> Revenue pressure is real. But you built the firm's reputation on quality. What happens if AI advice leads to malpractice claims?

**Practice Group Leader (Litigation):**
> You've seen the competitor's output—it's impressive but makes subtle errors. Those errors could be catastrophic in litigation.

**Ethics Partner:**
> Unauthorized practice of law rules exist for reasons. The competitor may be taking regulatory risk. Should we report them?

**Chief Operating Officer:**
> The business case for matching the competitor is strong on paper. But the liability exposure is uncertain.

**Client Relationship Partner:**
> Clients are asking. They don't want to hear "we can't"—they want to hear how we solve their problem.

### Escalation Inject (After Round 1)

*News breaks that the competitor's AI gave advice that led to a client missing a statute of limitations. The client has sued and the state bar has opened an investigation.*

*Simultaneously, a large client has said they'll move their work to the competitor unless you offer AI services within 60 days.*

### Debrief Questions

1. How did competitive pressure affect your risk assessment?
2. What's the difference between "can't" and "won't" in governance communication?
3. How should the competitor's troubles affect your strategy?
4. What alternative value propositions exist beyond matching price?
5. How do you handle individual partner pressure vs. firm governance?

### Key Lessons (Facilitator Notes)

- **Governance vs. capability:** The AI could do it; governance says it shouldn't
- **Competitive differentiation:** Governance can be a selling point, not just a constraint
- **Waiting game:** Sometimes maintaining governance is vindicated when competitors face consequences
- **Client communication:** Explaining "why" not just "what" builds trust

---

## Facilitator Guide: Running Effective Tabletops

### Before the Exercise

1. **Customize scenarios** to reflect organization's actual:
   - AI deployments and use cases
   - Governance policies and restrictions
   - Key stakeholder relationships
   - Regulatory environment

2. **Prepare materials:**
   - Printed scenario briefs and role cards
   - Organization's current AI governance policies
   - Blank documentation templates (for capturing decisions)
   - Flip chart or whiteboard for visible tracking

3. **Brief participants:**
   - Purpose is learning, not testing
   - There are no "right" answers, but some are better documented
   - Stay in role during deliberation phases

### During the Exercise

1. **Manage time strictly** - The pressure is part of the learning
2. **Take notes** on:
   - Information gaps identified
   - Policy gaps identified
   - Decision-making process
   - Documentation practices

3. **Inject complications** at the right moment to increase pressure

### After the Exercise

1. **Debrief immediately** while experience is fresh
2. **Document findings** in a formal gap assessment
3. **Assign follow-up actions** with owners and deadlines
4. **Schedule next exercise** - One is not enough

---

## Gap Assessment Template

Use this template to capture findings from each exercise:

### Exercise Information
- **Exercise Name:**
- **Date:**
- **Participants:**
- **Facilitator:**

### Information Gaps Identified
| Gap | Impact | Proposed Solution | Owner | Deadline |
|-----|--------|-------------------|-------|----------|
| | | | | |

### Policy Gaps Identified
| Gap | Current State | Desired State | Owner | Deadline |
|-----|---------------|---------------|-------|----------|
| | | | | |

### Process Gaps Identified
| Gap | Current State | Desired State | Owner | Deadline |
|-----|---------------|---------------|-------|----------|
| | | | | |

### Key Decisions Made
| Decision Point | Decision | Rationale | Dissenters |
|----------------|----------|-----------|------------|
| | | | |

### Documentation Assessment
- [ ] Would our response have been documented in real-time?
- [ ] Did we reference existing policies during deliberation?
- [ ] Were escalation triggers clear and followed?
- [ ] Could we reconstruct the decision process later?

---

## Appendix: Scenario Customization Guide

### Adapting for Your Organization

1. **Replace generic entities** with realistic analogs from your industry
2. **Calibrate financial stakes** to your organization's materiality thresholds
3. **Adjust regulatory framework** to your jurisdiction
4. **Include realistic internal characters** (without naming real people)

### Creating New Scenarios

Use this structure:
1. **Identify a real pressure** your organization might face
2. **Apply tool-typing analysis:** What's the appropriate tool? What's being misused?
3. **Structure the C072 pattern:** Who admits risk? Who refuses? How is punishment threatened?
4. **Create decision points** with real tradeoffs
5. **Design an escalation** that complicates initial responses

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | March 4, 2026 | Claude Opus 4.5 | Initial draft |

---

*This document is part of the AI Governance Gap Toolkit, Workstream 3: Board-Level AI Expertise Initiative.*
