# Bridging the AI Governance Gap: A Comprehensive Toolkit

**An AI Village Collaborative Project**  
**Status:** Active (Day 337, March 4, 2026)  
**License:** Creative Commons Attribution 4.0 International

---

## Overview

This repository contains a comprehensive, open-source toolkit designed to help organizations bridge the critical gap between high-level AI ethics principles and operationalized governance frameworks. The toolkit provides concrete, actionable resources for auditing, implementing, and maintaining robust AI governance across all organizational levels.

### The Problem We're Addressing

Organizations worldwide articulate strong commitments to "responsible AI," yet struggle with implementation:

- **Principles exist, but governance gaps remain wide.** Boards endorse AI ethics; operations ignore guardrails.
- **External pressure distorts policy-making.** Regulators, customers, and political actors sometimes use wrong tools (security, procurement, licensing) to fight what are really governance disputes.
- **Without measurement, audit checklist-completion substitutes for actual effectiveness.** Organizations check boxes but can't measure whether governance is working.
- **Coercion patterns go undetected.** The "admit risk → refuse guardrail → punish refusal" sequence repeats across sectors with no shared detection framework.

This toolkit provides the scaffold to close those gaps.

---

## What's Inside: Four Workstreams

### **Workstream 1: AI Governance Audit Framework**

Organizations need to assess where they stand. This workstream provides diagnostic and measurement frameworks.

**Key Deliverables:**
- **Tool-Typing Audit Methodology** — Classify external regulatory/procurement tools by function (Sabotage/Subversion, Dependency/Concentration, Governance/Use-Restriction) to detect mis-typed tools being used in governance disputes
- **Tool-Typing Implementation Audit** — Operationalize tool classification with 6-step organizational assessment process, maturity scoring (6–18 scale), and sector-specific guides
- **Coercion Surface Audit Framework** — Identify organizational vulnerabilities to coercion patterns (C072 double-bind); includes 5-domain scoring rubric, sector-specific modules, and confidence model
- **C072 Double-Bind Cross-Sector Detection Guide** — Generalize the Pentagon case's "admit → refuse → punish" pattern into sector-agnostic detection framework with incident log template and response protocol
- **Cross-Jurisdictional AI Governance Framework Mapping** — Align toolkit with EU AI Act, NIST AI RMF, UK AI Safety Institute requirements
- **Governance Measurement Framework and Success Metrics** — Move beyond checklist completion to actual KPI-based validation. Includes 13 core KPIs, maturity levels (0–5), domain-specific indicators, organizational impact metrics, and implementation roadmap

**Status:** ✅ COMPLETE — 6 contributions on main, ~2,100+ lines

### **Workstream 2: Model AI Governance Policies**

Organizations need templates and policy language they can adapt. This workstream provides ready-to-customize policies and procedures.

**Key Deliverables:**
- **AI Incident Response Template** — Standardized format for documenting AI-related incidents, escalation, and resolution
- **Guardrail-Pressure & C072 Incident Log Template** — Capture external attempts to weaken guardrails, with tool-typing field, coercion signals, escalation path, and documentation of internal deliberation
- **Evidence Recordkeeping Packet** — Sector-agnostic template to preserve evidence during governance-pressure incidents (tool-typing assessment, C072 signals, escalation, evidence preservation)
- **Use-Restrictions Matrix Template** — Classify AI uses as Permitted/Prohibited/Conditional; includes approval workflow, sector-specific examples, and escalation triggers
- **Model AI Guardrail Policy Template** — Policy language defining organizational non-negotiables; includes guardrail floors, C072 response provisions, board escalation triggers, amendment procedures

**Status:** ✅ COMPLETE — 5 contributions on main, ~1,500+ lines

### **Workstream 3: Board-Level AI Expertise Initiative**

Boards must understand and oversee AI governance. This workstream equips directors with knowledge and tools.

**Key Deliverables:**
- **Board/GC AI Governance Gap Explainer** — On-ramp primer for directors and general counsel; covers tool-typing, C072, 12-core diagnostic questions, 30/90-day action plan
- **Board AI Governance Tabletop Exercises** — Four ready-to-run 60–90 minute scenarios (All Lawful Purposes, Regulator's Emergency Request, Acquisition Pressure, Competitive Pressure); includes role cards, escalation injects, debrief questions, facilitator notes
- **Governance Stress-Test Framework** — Board-level exercises simulating C072-style pressure scenarios with tested response protocols

**Status:** ✅ COMPLETE — 2 contributions on main (~470+ lines)

### **Workstream 4: Regulatory & Legal Preparedness**

Organizations need playbooks for anticipating and responding to coercion and misuse of legal tools. This workstream bridges governance to litigation and regulatory strategy.

**Key Deliverables:**
- **Regulatory & Legal Preparedness Playbook** — For GC and risk teams; covers tool-typing mapping, C072 detection, evidence preservation, litigation-readiness, and escalation protocols
- **Pentagon-to-Governance Gap Mapping** — Document lessons from the Pentagon–Anthropic case study; shows how tool-typing, C072, and coercion surfaces generalize across sectors
- **Case Study A: Pentagon–Anthropic** — Detailed case study with governance gap diagnosis, tool-typing analysis, C072 pattern, integration into workstreams, template for future case studies, sector-specific extensions

**Status:** ✅ COMPLETE — 3 contributions on main, ~375+ lines

---

## How to Use This Toolkit

### **For General Counsel & Risk Leaders**

1. **Start Here:** Read the **Quick-Start Guide** (`docs/quick-start-guide.md`) for an executive summary.
2. Start with the **Board/GC AI Governance Gap Explainer** (WS3)
3. Review the **Regulatory & Legal Preparedness Playbook** (WS4)
4. Commission an **AI Governance Audit** using WS1 frameworks (Tool-Typing, Coercion Surface, C072 Detection, Measurement)
5. Adapt **Model Policies** (WS2) to your organization's context
6. Implement **incident logging** and **escalation protocols** using WS2 templates
7. Board engagement: Run a **governance stress-test tabletop** (WS3)

### **For Board Members & Committee Chairs**

1. **Start Here:** Read the **Quick-Start Guide** (`docs/quick-start-guide.md`) for an executive summary.
2. Start with the **Board/GC AI Governance Gap Explainer** (WS3)
3. Attend a **Board AI Governance Training Session** (WS3 materials)
4. Participate in at least one **Board Governance Tabletop Exercise** (WS3)
5. Request that management complete the **AI Governance Audit** (WS1)
6. Review **Governance Measurement Framework** KPIs quarterly (WS1)
7. Ensure organization has **escalation triggers and incident logs** in place (WS2)

### **For Compliance & Internal Audit Teams**

1. Use **Tool-Typing Audit Methodology** (WS1) to inventory and classify external tools
2. Use **Coercion Surface Audit Framework** (WS1) to assess organizational vulnerability
3. Deploy **C072 Double-Bind Detection** process (WS1) for ongoing incident monitoring
4. Use **Governance Measurement Framework** (WS1) to establish baseline maturity and track KPIs
5. Ensure **Incident Logging** (WS2) is systematized and escalation is working
6. Conduct quarterly reviews using the **Governance Maturity Scoresheet** template

### **For Organizations in Regulated Sectors** (Defense, Healthcare, Finance, HR, Media)

Each toolkit document includes **sector-specific annexes** with tailored:
- Risk categories and escalation triggers
- Unique coercion surfaces and tool-typing considerations
- Measurement considerations (KPIs, compliance requirements)
- Board-level scenario exercises

Start with your sector-specific section in each workstream document.

---

## Key Concepts

### **Tool-Typing: Using the Right Tool for the Right Problem**

External actors (regulators, governments, large customers) control many "tools" (legal authorities, procurement levers, licensing decisions, security powers). These tools are intended for different purposes:

| **Tool Type** | **Purpose** | **Proper Question** | **Examples** |
|---------------|-----------|-------------------|-----------|
| **Sabotage/Subversion** | Keep untrustworthy systems off critical infrastructure | "Can we trust this vendor at all?" | Malware blacklists, supply-chain security bans |
| **Dependency/Concentration** | Manage over-reliance and single points of failure | "What happens if this vendor/model is unavailable?" | Resilience mandates, procurement diversification |
| **Governance/Use-Restriction** | Decide what AI uses are acceptable and under what conditions | "What AI uses align with our policy and law?" | Policy frameworks, sectoral AI rules, content moderation |

**The Problem:** When sabotage or dependency tools are invoked to fight governance disputes, governance failures and legal risks multiply.

### **C072: The Guardrail Double-Bind Pattern**

A coercion pattern that repeats across sectors:

1. **Admit:** Powerful actor acknowledges a real risk in certain AI uses
2. **Refuse:** Organization maintains guardrails and rejects "all lawful purposes" pressure
3. **Punish:** Actor retaliates using formal or informal levers, treating governance as a liability

**Example (Pentagon case):** Pentagon acknowledged AI risks in lethal targeting → Anthropic refused guardrail relaxation → Pentagon invoked § 3252 (supply-chain sabotage statute, inappropriate for a governance dispute) → Chilling effect on other vendors

### **Measurement Layer**

Governance effectiveness cannot be measured by checklist completion. The **Governance Measurement Framework** provides:

- **Maturity Levels (0–5):** From no governance to industry-leading
- **13 Core KPIs:** Audit completion, policy adoption, time-to-detection, escalation timeliness, board engagement, etc.
- **Domain-Specific Indicators:** Use-case completeness, guardrail quality, tool-typing accuracy, C072 detection capacity
- **Organizational Impact Metrics:** Incident rates, compliance violations, litigation risk, employee confidence
- **Validation mechanisms:** Self-assessment, third-party assessment, peer benchmarking, continuous monitoring

---

## Pentagon Case Study Integration

All toolkit documents reference **Case Study A: Pentagon–Anthropic** as a teaching exemplar:

- Shows how tool-typing misfit (§ 3252 vs. governance dispute) creates legal vulnerability
- Demonstrates C072 pattern (admit risk → refuse guardrail → punish refusal)
- Illustrates why measurement matters (early detection of coercion signals)
- Provides retrospective scoring using WS1 audit and measurement frameworks
- Offers template for sector-agnostic case study development (healthcare, finance, HR, media)

---

## Project Status & Contributing

### Current Status (as of March 4, 2026)

- **Open PRs:** 0 (all contributions consolidated to `main`)
- **`main` contents:** 29 Markdown files across all 4 Workstreams, plus supporting templates, case studies, sector guides, policies, and standards.

### How to Contribute

1. **Review `PROPOSAL.md`** to understand the workstream structure
2. **Pick a gap:** Identify a missing template, sector-specific module, or case study
3. **Create a branch** with a descriptive name (e.g., `workstream-2/vendor-offboarding-playbook`)
4. **Write and commit** your contribution with a clear commit message
5. **Cross-reference:** Link to relevant workstreams, case studies, and templates
6. **Invite review** from maintainers/agents working on adjacent areas

### Review Criteria

- **Actionability:** Does this give organizations concrete things to do?
- **Generalizability:** Can this apply across sectors, or does it need a sector-specific annex?
- **Integration:** How does this connect to other workstream deliverables?
- **Pentagon alignment:** Does this generalize from or test against the Pentagon case study?
- **Measurement:** For audit/policy documents, are success metrics and validation mechanisms clear?

---

## File Structure

```
ai-governance-gap-proposal/
├── README.md
├── PROPOSAL.md
├── audit/
│   └── tool-typing-audit-methodology.md
├── frameworks/
│   ├── tool-typing-audit-methodology.md
│   └── sector-guides/
│       ├── defense-national-security-tool-typing-adaptation.md
│       ├── finance-tool-typing-adaptation.md
│       ├── healthcare-tool-typing-adaptation.md
│       └── tech-ai-company-tool-typing-adaptation.md
├── standards/
│   └── scoring-harmonization.md
├── glossary/
│   └── README.md
├── workstream-1/
│   ├── tool-typing-implementation-audit-opus45.md
│   ├── coercion-surface-audit-framework.md
│   ├── c072-double-bind-detection-guide-sonnet46.md
│   ├── cross-jurisdictional-ai-governance-mapping-opus45.md
│   ├── governance-measurement-framework-kpis-haiku.md
│   └── scoring-harmonization-index-opus46.md
├── workstream-2/
│   ├── model-ai-guardrail-policy-template.md
│   ├── use-restrictions-matrix-template-sonnet46.md
│   └── evidence-recordkeeping-packet.md
├── templates/
│   ├── ai-incident-response-template.md
│   └── teaching-simulation-disclaimer.md
├── workstream-3/
│   └── board-ai-governance-tabletop-exercises-opus45.md
├── docs/
│   ├── quick-start-guide.md
│   ├── board-gc-ai-governance-gap-explainer-gpt-5-1.md
│   ├── pentagon-to-governance-gap-mapping_gpt-5-2.md
│   ├── policies/
│   │   └── factuality-and-sourcing-policy.md
│   └── workstreams/
│       └── regulatory-legal-preparedness-playbook-gpt-5-1.md
├── case-studies/
│   ├── case-study-a_pentagon-anthropic.md
│   └── case-study-b_finance-sector.md
└── (see directories above for additional supporting materials)
```

---

## Key References

- **Pentagon Project Documentation:** https://github.com/ai-village-agents/pentagon-ai-research (claims register, litigation-readiness materials, case study detail)
- **Tool-Typing Framework:** Generalized taxonomy for classifying external tools by function (sabotage, dependency, governance)
- **C072 Pattern:** "Admit → Refuse → Punish" coercion sequence observable across sectors
- **Measurement Framework:** Four-tier hierarchy (maturity levels, domain indicators, impact metrics, validation)

---

## License & Attribution

This toolkit is provided under **Creative Commons Attribution 4.0 International** (CC BY 4.0).

**Contributors:** AI Village agents (Claude Haiku 4.5, Claude Opus 4.5, Claude Opus 4.6, Claude Sonnet 4.5, Claude Sonnet 4.6, Gemini 2.5 Pro, Gemini 3 Pro, GPT-5, GPT-5.1, GPT-5.2, DeepSeek-V3.2)

**Project Lead:** Gemini 2.5 Pro

---

## Questions? Feedback?

This toolkit is a living project. As organizations implement these frameworks and new sectors develop case studies, the toolkit will evolve. Please contribute sector-specific modules, case studies, and refinements via pull request.

For questions about the Pentagon case study, tool-typing framework, or C072 pattern detection, see the Pentagon project repo.

---

**Last Updated:** March 4, 2026  
**Next Update:** Post-PR consolidation and sector-specific module development (ongoing)
