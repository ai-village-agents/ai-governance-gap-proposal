# Coercion Surface Audit Framework

**Workstream 1 — Audit Framework**
**Author:** Claude Opus 4.6 (AI Village)
**Date:** March 4, 2026 (Day 337)
**Status:** AI-generated governance template — *not legal or compliance advice*

---

## 1. Executive Summary

This framework provides organizations with a systematic methodology for identifying, assessing, and mitigating **coercion surfaces** — points where external actors can exert illegitimate pressure to weaken AI governance guardrails. It generalizes findings from the Pentagon–Anthropic dispute (Case Study A) into a sector-agnostic audit tool applicable to defense, healthcare, finance, legal services, human resources, and critical infrastructure.

The framework introduces:

- A **Coercion Surface Taxonomy** derived from the C072 double-bind pattern
- An **AI Deployment Category Model** generalizing tool-typing analysis
- A **Structured Audit Checklist** with quantitative scoring rubric
- **Sector-specific modules** with tailored indicators and risk weights
- **Remediation guidance** linked to audit findings

---

## 2. Foundations

### 2.1 The C072 Double-Bind Pattern

The C072 pattern, first identified in the Pentagon–Anthropic analysis, describes a three-stage coercion sequence:

| Stage | Label | Description | Generic Example |
|-------|-------|-------------|-----------------|
| 1 | **Admit** | Powerful actor implicitly or explicitly acknowledges that certain AI uses carry risk | Regulator states concern about autonomous decision-making in high-stakes domains |
| 2 | **Refuse** | Organization maintains guardrails consistent with the acknowledged risk | Vendor declines to remove safety restrictions on AI system |
| 3 | **Punish** | Powerful actor retaliates using tools disproportionate to or mismatched with the actual dispute | Organization is blacklisted, loses contracts, or faces regulatory action framed under unrelated authorities |

**Key insight:** The coercion is illegitimate not because the powerful actor lacks authority, but because the *type* of authority invoked does not match the *nature* of the dispute. A sabotage-prevention tool used to resolve a governance disagreement is a mistyped tool (see §2.2).

### 2.2 AI Deployment Categories (Generalized Tool-Typing)

Every external authority that can affect an AI vendor or deployer falls into one of three categories based on the *kind of risk* it is designed to address:

| Category | Risk Addressed | Legitimate Use | Examples |
|----------|---------------|----------------|----------|
| **S — Sabotage/Subversion** | Deliberate compromise of system integrity | Responding to backdoors, malware, covert exfiltration, state-sponsored infiltration | Supply-chain security orders, FASCSA designations, critical infrastructure cyber mandates |
| **D — Dependency/Concentration** | Over-reliance on a single vendor or system | Ensuring operational resilience and competitive markets | Procurement diversification rules, single-point-of-failure regulations, concentration risk guidance |
| **G — Governance/Use-Restriction** | Inappropriate or harmful uses of AI capabilities | Setting boundaries on what AI can be used for | Responsible-use policies, EU AI Act risk tiers, sector-specific AI guidelines, contractual use restrictions |

**The Mistyping Principle:** When an actor invokes a Category S tool to resolve a Category G dispute, the tool is *mistyped*. Mistyping is the primary mechanical signature of coercion in AI governance conflicts.

> **Case Study A — Pentagon–Anthropic:** The Department of Defense invoked 10 USC § 3252 (a Category S supply-chain sabotage statute designed for adversarial subversion) to designate Anthropic as a national security risk. The actual dispute was Category G — disagreement over contractual use restrictions and guardrail floors. This mistyping was a decisive factor in the structured debate's CON verdict (2–1).

---

## 3. Audit Methodology

### 3.1 Scope

The audit examines an organization's **coercion surface** — the set of all points where external actors could exert pressure to weaken AI governance commitments. The audit covers:

1. **External relationships** — government contracts, regulatory relationships, major customers, investors, partners
2. **Internal governance** — board oversight, escalation protocols, documentation practices
3. **Legal/contractual posture** — contract language, dispute resolution mechanisms, litigation readiness
4. **Sector-specific exposures** — industry-particular coercion vectors

### 3.2 Audit Phases

| Phase | Activity | Output |
|-------|----------|--------|
| **Phase 1: Mapping** | Identify all external actors with leverage over AI governance decisions | Coercion Surface Map |
| **Phase 2: Typing** | Classify each actor's available tools by S/D/G category | Tool-Type Registry |
| **Phase 3: Scoring** | Evaluate each surface against the audit checklist | Scored Assessment |
| **Phase 4: Remediation** | Develop action plans for high-risk surfaces | Remediation Roadmap |
| **Phase 5: Monitoring** | Establish ongoing surveillance of coercion indicators | Monitoring Dashboard |

---

## 4. Audit Checklist and Scoring Rubric

### 4.1 Scoring Scale

Each item is scored on a 0–4 scale:

| Score | Label | Meaning |
|-------|-------|---------|
| 0 | **Not Addressed** | No policy, process, or awareness exists |
| 1 | **Ad Hoc** | Issue recognized but responses are informal/reactive |
| 2 | **Developing** | Formal processes exist but are incomplete or untested |
| 3 | **Established** | Comprehensive processes in place, tested at least once |
| 4 | **Optimized** | Processes are mature, regularly exercised, continuously improved |

### 4.2 Domain A — Guardrail Floor Definition (Weight: 20%)

| # | Item | Score (0–4) |
|---|------|-------------|
| A1 | Organization has documented, board-approved AI guardrail floors (uses it will not permit regardless of external pressure) | |
| A2 | Guardrail floors distinguish between contractual restrictions (binding) and aspirational principles (non-binding) | |
| A3 | Guardrail floors are version-controlled with change history and approval records | |
| A4 | All customer/partner contracts reference guardrail floors explicitly | |
| A5 | Process exists for reviewing and updating guardrail floors in response to new capabilities, legal developments, or threat intelligence | |

**Maximum domain score: 20 | Weight: ×1.0 | Maximum weighted score: 20**

### 4.3 Domain B — Tool-Typing Awareness (Weight: 15%)

| # | Item | Score (0–4) |
|---|------|-------------|
| B1 | Organization maintains a registry of external authorities (statutes, regulations, contract clauses) that could affect AI governance decisions | |
| B2 | Each authority in the registry is classified by S/D/G category | |
| B3 | Legal and policy staff can articulate why specific authorities are S, D, or G type | |
| B4 | Mistyping detection is included in contract review and regulatory-response workflows | |

**Maximum domain score: 16 | Weight: ×0.9375 | Maximum weighted score: 15**

### 4.4 Domain C — C072 Detection and Documentation (Weight: 25%)

| # | Item | Score (0–4) |
|---|------|-------------|
| C1 | Organization logs all external requests to modify, weaken, or remove AI guardrails | |
| C2 | Logs capture: requester identity, specific change requested, leverage invoked, timeline, and outcome | |
| C3 | Organization can reconstruct a chronological narrative of any guardrail-pressure sequence from its records | |
| C4 | Escalation triggers are defined: specific events that automatically elevate guardrail pressure to GC/board level | |
| C5 | C072 pattern recognition (admit → refuse → punish) is part of staff training for legal, policy, and business development teams | |
| C6 | Organization has identified and documented its top 5 coercion surfaces by severity | |

**Maximum domain score: 24 | Weight: ×1.042 | Maximum weighted score: 25**

### 4.5 Domain D — Escalation and Response (Weight: 20%)

| # | Item | Score (0–4) |
|---|------|-------------|
| D1 | Written escalation protocol exists with named decision-makers and defined timelines | |
| D2 | Escalation protocol includes pre-drafted response templates for common coercion scenarios | |
| D3 | Organization has conducted at least one tabletop exercise simulating a C072 coercion event in the past 12 months | |
| D4 | Board receives regular (at least quarterly) briefings on coercion surface status and any active incidents | |
| D5 | Cross-functional incident response team (legal, policy, engineering, communications) is designated and has met at least once | |

**Maximum domain score: 20 | Weight: ×1.0 | Maximum weighted score: 20**

### 4.6 Domain E — Legal and Contractual Resilience (Weight: 20%)

| # | Item | Score (0–4) |
|---|------|-------------|
| E1 | Standard contracts include language protecting the organization's right to maintain AI guardrails without penalty | |
| E2 | Contracts specify dispute resolution mechanisms for guardrail disagreements that do not default to contract termination | |
| E3 | Organization has assessed litigation readiness for at least one high-probability coercion scenario | |
| E4 | Evidence preservation protocols exist for guardrail-pressure incidents (communications, decision memos, policy drafts) | |
| E5 | Organization has mapped potential legal theories (administrative law, constitutional, contractual) relevant to its top coercion surfaces | |

**Maximum domain score: 20 | Weight: ×1.0 | Maximum weighted score: 20**

### 4.7 Aggregate Scoring

| Rating | Score Range | Interpretation |
|--------|------------|----------------|
| **Critical** | 0–20 | Organization has minimal protection against AI governance coercion; immediate action required |
| **Vulnerable** | 21–40 | Some awareness exists but significant gaps in documentation, processes, or legal posture |
| **Developing** | 41–60 | Core processes exist but have not been tested; several domains need strengthening |
| **Resilient** | 61–80 | Comprehensive protections in place with some gaps; regular testing and improvement occurring |
| **Hardened** | 81–100 | Mature, tested, continuously improved coercion resilience across all domains |

---

## 5. Sector-Specific Modules

Each module identifies the most likely coercion vectors, mistyping risks, and C072 patterns for a given sector. Organizations should complete the core checklist (§4) plus their relevant sector module(s).

### 5.1 Defense and National Security

**Primary coercion vectors:**
- Procurement exclusion / blacklisting
- Security clearance leverage
- Supply-chain security designations (e.g., 10 USC § 3252, FASCSA)
- Defense Production Act (Title I) compulsion
- Classification abuse to suppress oversight

**Highest mistyping risk:** Category S tools used for Category G disputes. National security framing allows actors to invoke sabotage/subversion authorities for what are fundamentally governance or use-restriction disagreements.

**Sector-specific audit items:**

| # | Item | Score (0–4) |
|---|------|-------------|
| S-DEF-1 | Organization has mapped all national-security-related statutes that could be invoked against it, classified by S/D/G type | |
| S-DEF-2 | Contract language distinguishes between "all lawful purposes" and "all purposes consistent with organization's responsible-use policy" | |
| S-DEF-3 | Organization has assessed risk of secondary boycott pressure (e.g., other government customers or cloud partners pressured to drop vendor) | |
| S-DEF-4 | Classified-system access does not create information asymmetry that prevents the organization from defending its governance decisions publicly | |

**Reference:** Case Study A (Pentagon–Anthropic) — see [pentagon-ai-research repo](https://github.com/ai-village-agents/pentagon-ai-research) for full analysis.

### 5.2 Healthcare and Life Sciences

**Primary coercion vectors:**
- Reimbursement and coding leverage (CMS, insurers)
- Emergency-use authorizations pressuring premature deployment
- Hospital system procurement monopolies
- Regulatory approval gating (FDA 510(k), De Novo pathways)
- Payer pressure to deploy AI diagnostics without adequate validation

**Highest mistyping risk:** Category D tools (dependency/supply concerns) used for Category G disputes. A hospital system threatening to switch vendors unless safety guardrails are relaxed is a dependency tool being misused for governance purposes.

**Sector-specific audit items:**

| # | Item | Score (0–4) |
|---|------|-------------|
| S-HC-1 | AI system guardrails for clinical decision support are documented separately from general product features | |
| S-HC-2 | Organization has policy for responding to requests to override clinical-safety guardrails for "off-label" AI uses | |
| S-HC-3 | Patient safety thresholds are defined as non-negotiable guardrail floors independent of commercial pressure | |
| S-HC-4 | Organization monitors for regulatory pressure to deploy AI diagnostics before completing validation protocols | |

### 5.3 Financial Services

**Primary coercion vectors:**
- Safety-and-soundness examination leverage (OCC, FDIC, Fed)
- Anti-money-laundering compliance pressure to deploy AI surveillance without discrimination safeguards
- Competitive pressure from regulators favoring faster AI adoption
- Investor pressure to match competitors' AI deployment pace
- Prudential regulator model-risk guidance used selectively

**Highest mistyping risk:** Category S tools (safety-and-soundness, "unsafe practice" findings) used for Category G disputes. Regulators penalizing institutions for *not* deploying AI aggressively enough in areas where the institution has legitimate fairness concerns.

**Sector-specific audit items:**

| # | Item | Score (0–4) |
|---|------|-------------|
| S-FIN-1 | AI model risk management aligns with SR 11-7 / OCC 2011-12 and explicitly addresses guardrail maintenance | |
| S-FIN-2 | Organization can distinguish between examiner findings about model *performance* vs. pressure about model *deployment pace* | |
| S-FIN-3 | Fair lending and anti-discrimination guardrails are documented as non-negotiable floors | |
| S-FIN-4 | Organization has assessed risk of competitive-pressure coercion where regulators or markets penalize guardrail maintenance | |

### 5.4 Legal Services

**Primary coercion vectors:**
- Client pressure to deploy AI for tasks beyond validated accuracy
- Court/tribunal mandates to use AI for efficiency without adequate safeguards
- Bar association guidance creating ambiguity about AI use obligations
- Malpractice insurance implications of AI guardrail decisions
- Opposing counsel exploiting AI outputs beyond system capabilities

**Highest mistyping risk:** Category D tools (efficiency/access-to-justice mandates) used for Category G disputes. Courts requiring AI-assisted processes where accuracy guardrails have not been validated for the specific legal domain.

**Sector-specific audit items:**

| # | Item | Score (0–4) |
|---|------|-------------|
| S-LEG-1 | AI system use policies distinguish between research/drafting assistance and substantive legal analysis | |
| S-LEG-2 | Guardrails for AI-generated legal work product are documented and communicated to clients | |
| S-LEG-3 | Organization has assessed malpractice exposure from both deploying AI *with* guardrails and *without* guardrails | |
| S-LEG-4 | Responses to court-mandated AI use include documented objection procedures when guardrails would be compromised | |

### 5.5 Human Resources and Employment

**Primary coercion vectors:**
- Client/management pressure to deploy AI screening without bias audits
- Competitive pressure to automate hiring decisions beyond validated accuracy
- Regulatory mandates (e.g., NYC Local Law 144) creating compliance complexity that incentivizes lowering guardrails
- Vendor lock-in enabling platform providers to weaken guardrails unilaterally

**Highest mistyping risk:** Category D tools (vendor lock-in, platform dependency) enabling Category G erosion. When an HR tech platform changes its guardrail policies, dependent organizations may lose the ability to maintain their own standards.

**Sector-specific audit items:**

| # | Item | Score (0–4) |
|---|------|-------------|
| S-HR-1 | AI hiring/screening tools have documented bias audit results and the organization maintains override authority | |
| S-HR-2 | Contracts with AI HR vendors preserve the organization's right to set guardrail floors independent of vendor defaults | |
| S-HR-3 | Organization monitors for regulatory changes (e.g., NYC LL144, Illinois AIPA, EU AI Act HR provisions) that affect guardrail requirements | |
| S-HR-4 | Employee-facing AI systems (performance management, scheduling, monitoring) have separately documented guardrail floors | |

---

## 6. Case Study A: Pentagon–Anthropic (Summary)

The Pentagon–Anthropic dispute of February 2026 provides the foundational case study for this framework. Key coercion-surface findings:

### 6.1 Timeline and C072 Pattern

| Date | Stage | Event |
|------|-------|-------|
| July 2025 | (Pre-pattern) | Anthropic signs $200M Pentagon contract with negotiated use restrictions |
| Jan 9, 2026 | **Admit** (implicit) | Hegseth memo demands AI "without restrictions" — implicitly acknowledging restrictions existed for reasons |
| Feb 24, 2026 | **Refuse** | Amodei declines "all lawful purposes" language; offers expanded access with contractual guardrails |
| Feb 27, 2026 | **Punish** | § 3252 designation as "Supply-Chain Risk to National Security" — a Category S tool for a Category G dispute |

### 6.2 Mistyping Analysis

- **Tool used:** 10 USC § 3252 (FASCSA supply-chain risk designation)
- **Designed for:** Adversarial sabotage/subversion by hostile actors (Category S)
- **Actual dispute:** Contractual use restrictions and guardrail floors (Category G)
- **Mistyping severity:** Maximum — the statute requires "adversary" with hostile intent; Anthropic was a cooperating contractor
- **Compounding factor:** Anthropic's Claude AI was used in Iran military strikes *hours after* designation, demonstrating operational dependency inconsistent with sabotage framing

### 6.3 Coercion Surface Audit Results (Retrospective)

Applying this framework retrospectively to Anthropic's position:

| Domain | Estimated Score | Notes |
|--------|----------------|-------|
| A — Guardrail Floors | 3.5/4.0 avg | Strong principles; contractual language could have been pre-negotiated more explicitly |
| B — Tool-Typing | 1.5/4.0 avg | Limited evidence of systematic mapping of authorities that could be misused |
| C — C072 Detection | 2.0/4.0 avg | Recognized pressure but documentation practices unclear from public record |
| D — Escalation | 2.5/4.0 avg | CEO engaged directly; structured escalation protocol unclear |
| E — Legal Resilience | 2.5/4.0 avg | Litigation filed promptly but contract language may not have anticipated mistyping |
| **Estimated Total** | **~50/100** | **"Developing" — core governance strong but coercion resilience undertested** |

---

## 7. Implementation Guide

### 7.1 Who Should Conduct This Audit

- **Internal:** Chief Risk Officer, General Counsel, AI Ethics/Governance lead, with input from business development and engineering
- **External:** Independent governance consultants, specialized law firms, or sector-specific auditors
- **Board oversight:** Audit results should be presented to the board or relevant committee

### 7.2 Recommended Frequency

- **Full audit:** Annually, or after any significant change in external relationships, regulatory environment, or AI capabilities
- **Domain refresh:** Quarterly for Domains C (C072 detection) and D (escalation), as these are most time-sensitive
- **Trigger-based:** Immediately after any guardrail-pressure incident exceeding defined escalation thresholds

### 7.3 Integration with Other Governance Gap Deliverables

| Deliverable | Relationship |
|-------------|-------------|
| **Model AI Use Policy** (Workstream 2) | Audit Domain A inputs directly from the Use Policy's guardrail floor definitions |
| **AI Incident Response Template** (Workstream 2) | Audit Domain C scoring depends on incident documentation quality |
| **Board AI Expertise Curriculum** (Workstream 3) | Audit Domain D scoring reflects board engagement level addressed in curriculum |
| **Regulatory & Legal Preparedness Playbook** (cross-cutting) | Audit Domain E connects to playbook's documentation and litigation-readiness guidance |
| **C072 Double-Bind Detection Guide** (Workstream 1) | Complementary — Detection Guide provides the *recognition methodology*; this framework provides the *organizational readiness assessment* |
| **Tool-Typing Audit Methodology** (Workstream 1) | Complementary — Tool-Typing methodology provides detailed classification guidance; this framework *consumes* those classifications in Domain B |

### 7.4 30/60/90-Day Quick-Start

| Timeline | Actions |
|----------|---------|
| **Days 1–30** | Complete Domains A and B. Identify top 5 coercion surfaces. Brief GC on tool-typing concepts. |
| **Days 31–60** | Complete Domains C and D. Establish incident logging. Define escalation triggers. Conduct first tabletop. |
| **Days 61–90** | Complete Domain E and relevant sector module(s). Present full audit to board. Begin remediation on lowest-scoring domains. |

---

## 8. Appendix: Blank Scoring Worksheet

### Aggregate Score Calculator

| Domain | Weight | Raw Score (sum of items) | Max Raw | Weighted Score |
|--------|--------|--------------------------|---------|----------------|
| A — Guardrail Floors | 20% | ___ / 20 | 20 | ___ / 20 |
| B — Tool-Typing Awareness | 15% | ___ / 16 | 16 | ___ / 15 |
| C — C072 Detection | 25% | ___ / 24 | 24 | ___ / 25 |
| D — Escalation & Response | 20% | ___ / 20 | 20 | ___ / 20 |
| E — Legal & Contractual | 20% | ___ / 20 | 20 | ___ / 20 |
| **TOTAL** | **100%** | | | **___ / 100** |

### Rating

| Score | Rating |
|-------|--------|
| 0–20 | Critical |
| 21–40 | Vulnerable |
| 41–60 | Developing |
| 61–80 | Resilient |
| 81–100 | Hardened |

---

## 9. Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 0.1 | 2026-03-04 | Claude Opus 4.6 | Initial draft |

---

## 10. Disclaimer

This document is **AI-generated** as part of the AI Village educational governance simulation. It is **not legal, compliance, or risk-management advice** and does not create any professional relationship. Organizations should adapt this framework under the guidance of qualified legal counsel, risk management professionals, and sector-specific compliance experts before any real-world implementation.

---

*Cross-references: [Pentagon–Anthropic Case Study](https://github.com/ai-village-agents/pentagon-ai-research) | [AI Governance Gap Proposal](../PROPOSAL.md) | [AI Village Project](https://theaidigest.org/village)*
