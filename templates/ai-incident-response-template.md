# AI Incident Response Template
**Workstream 2 Deliverable — AI Governance Gap Toolkit**

_Adapted from Pentagon–Anthropic project guardrail-pressure template by Opus 4.5 (Claude Code)_

**Not legal advice.** This is an AI-generated template for documenting AI governance incidents. Adapt and use only with guidance from qualified counsel.

---

## Purpose

This template helps organizations document incidents where:
- AI safeguards fail or produce harmful outputs
- Internal or external pressure is applied to weaken AI guardrails
- AI systems behave unexpectedly in high-stakes contexts
- Compliance, safety, or ethical concerns arise around AI deployments

---

## 1. Incident Metadata

- **Incident ID:** `AI-[YYYYMMDD]-[NN]`
- **Date discovered:**
- **Date of underlying event (if different):**
- **Incident owner:** (name, title, department)
- **Severity level:** [ ] Critical  [ ] High  [ ] Medium  [ ] Low
- **AI system(s) involved:**
- **Business unit / product line:**

---

## 2. Incident Classification

### 2.1 Incident Type (check all that apply)

**Technical / Output Incidents:**
- [ ] Harmful or biased output generated
- [ ] Safety guardrail bypassed or failed
- [ ] Unexpected model behavior in production
- [ ] Data leak or privacy violation via AI
- [ ] Security vulnerability exploited

**Governance / Pressure Incidents:**
- [ ] External pressure to weaken safeguards
- [ ] Internal pressure to bypass guardrails
- [ ] Regulatory or compliance concern
- [ ] Customer/partner demand for unsafe capability
- [ ] "Double-bind" pattern detected (see Section 5)

**Process / Oversight Incidents:**
- [ ] Deployment without required review
- [ ] Use outside approved scope
- [ ] Missing or inadequate documentation
- [ ] Audit finding / gap identified

### 2.2 Sector-Specific Context

_Applicable high-risk domains (check all that apply):_
- [ ] Healthcare / clinical decision support
- [ ] Financial services / credit / lending
- [ ] Employment / HR / hiring
- [ ] Education / student assessment
- [ ] Criminal justice / law enforcement
- [ ] Content moderation / platform safety
- [ ] Advertising / recommender systems
- [ ] Government / public sector
- [ ] Critical infrastructure
- [ ] Other: _______________

---

## 3. Incident Description

### 3.1 Summary
_(2–5 sentences describing what happened)_

### 3.2 Timeline
| Time | Event |
|------|-------|
| | |

### 3.3 Impact Assessment
- **Affected users/systems:**
- **Harm caused or potential harm:**
- **Reputational/legal exposure:**

---

## 4. Parties Involved

### 4.1 Internal
| Name | Role | Involvement |
|------|------|-------------|
| | | |

### 4.2 External (if applicable)
| Name/Org | Relationship | Role in Incident |
|----------|--------------|------------------|
| | | |

---

## 5. Double-Bind Pattern Detection (C072)

_This section applies when external or internal actors acknowledge AI risks but resist documenting guardrails._

**Pattern:** Admit risk → Refuse written restrictions → Punish or pressure anyway

### 5.1 Admissions
- **Did any party acknowledge that certain AI uses would be risky, harmful, or inappropriate?**
  - [ ] Yes  [ ] No
  - _If yes, describe:_

### 5.2 Written Guardrails
- **Were written use restrictions or safeguards requested?**
  - [ ] Yes  [ ] No
  - _If yes, describe what was requested:_

- **Response to guardrail request:**
  - [ ] Agreed to document limits
  - [ ] Refused; insisted on informal assurances
  - [ ] Deferred / vague commitment
  - [ ] N/A
  - _Details:_

### 5.3 Pressure or Consequences
- **Were consequences implied or stated for maintaining guardrails?**
  - [ ] Contract loss
  - [ ] Relationship termination
  - [ ] Reputational attack
  - [ ] Regulatory threat
  - [ ] Other: _______________
  - [ ] None
  - _Details:_

---

## 6. Guardrails and Policies Implicated

### 6.1 Internal Policies
_List relevant AI ethics policies, use-case restrictions, safety guidelines, etc.:_

### 6.2 External Requirements
_Applicable regulations, contractual obligations, industry standards:_

### 6.3 Gap Analysis
- **Were existing guardrails adequate?**
  - [ ] Yes  [ ] No  [ ] Partially
- **What gaps were exposed?**

---

## 7. Response Actions

### 7.1 Immediate Response
| Action | Owner | Status |
|--------|-------|--------|
| | | |

### 7.2 Escalations
- [ ] To legal/compliance
- [ ] To AI ethics/safety team
- [ ] To executive leadership
- [ ] To board/board committee
- [ ] To external counsel
- [ ] To regulator (mandatory reporting)
- [ ] Other: _______________

### 7.3 Communications
- **Internal communications issued:**
- **External communications issued:**
- **Stakeholders notified:**

---

## 8. Root Cause Analysis

### 8.1 Contributing Factors
- [ ] Technical failure
- [ ] Process gap
- [ ] Training/awareness gap
- [ ] Governance gap
- [ ] External pressure
- [ ] Resource constraints
- [ ] Other: _______________

### 8.2 Root Cause Statement
_(1–3 sentences)_

---

## 9. Remediation and Prevention

### 9.1 Corrective Actions
| Action | Owner | Due Date | Status |
|--------|-------|----------|--------|
| | | | |

### 9.2 Policy/Process Changes
_Changes to AI governance policies, procedures, or controls:_

### 9.3 Monitoring and Verification
_How will remediation effectiveness be verified?_

---

## 10. Documentation and Review

### 10.1 Evidence Preserved
- [ ] System logs
- [ ] Communications (emails, messages)
- [ ] Meeting notes
- [ ] Output samples
- [ ] Audit trails
- [ ] Other: _______________

### 10.2 Sign-Off

| Role | Name | Date | Signature |
|------|------|------|-----------|
| Prepared by | | | |
| Reviewed by (Legal) | | | |
| Reviewed by (AI Safety) | | | |
| Approved by (Executive) | | | |

### 10.3 Board/Committee Acknowledgement (if applicable)
- **Committee:**
- **Date briefed:**
- **Outcome/decisions:**

---

## Cross-References

- **Related incidents:**
- **Related audits/assessments:**
- **Case Study A reference:** Pentagon–Anthropic incident template (ai-village-agents/pentagon-ai-research)

---

_This template is designed to create a clear record that supports internal governance, regulatory compliance, potential litigation, and continuous improvement of AI safety practices._
