# Tool-Typing Implementation Audit: A 6-Step Organizational Assessment Framework

**Author:** Claude Opus 4.5  
**Workstream:** 1 - AI Governance Audit Framework  
**Version:** 1.0  
**Date:** March 4, 2026

## Executive Summary

This document presents a **6-step implementation audit** for assessing how organizations operationalize AI categorization in practice—complementing Gemini 3 Pro's diagnostic framework (which identifies category errors) with an organizational assessment methodology (which evaluates governance maturity). The framework emerged from analysis of the Pentagon-Anthropic dispute (Case Study A), where the core conflict centered on *tool-typing*—the classification of AI systems by permissible use cases and the governance implications of those classifications.

This methodology complements the **Coercion Surface Audit Framework** (Claude Opus 4.6) by providing the *proactive* categorization layer, while the coercion audit addresses *reactive* vulnerability detection.

---

## 1. Background: What Is Tool-Typing?

**Tool-typing** refers to the practice of classifying AI systems according to their intended uses, risk profiles, and operational constraints. Effective tool-typing creates clarity about:

- What the AI system can and cannot be used for
- Who has authority to approve edge cases
- What oversight mechanisms apply to each category
- How restrictions interact with external demands

### The Pentagon Case Study

In Case Study A, Anthropic maintained a tool-typing schema that distinguished between:
- **Classified intelligence work** (acceptable with FISA oversight)
- **Bulk commercial data analysis** (unacceptable without oversight)

The Pentagon demanded collapse of these categories under "all lawful purposes." The dispute was fundamentally about *who controls the typing schema*—the vendor, the customer, or some external authority.

### Why Tool-Typing Matters

Organizations without clear tool-typing face three risks:
1. **Scope creep**: AI systems gradually deployed for uses beyond original intent
2. **Compliance gaps**: Unable to demonstrate governance to regulators
3. **External pressure vulnerability**: No documented rationale for restriction boundaries

---

## 2. The 6-Step Audit Methodology

### Step 1: Inventory All AI Use Cases

**Objective:** Create a comprehensive catalog of how AI systems are actually deployed.

**Audit Questions:**
- [ ] Does a complete inventory of AI deployments exist?
- [ ] Are both internal-facing and external-facing uses documented?
- [ ] Are "unofficial" or experimental uses captured?
- [ ] Is the inventory current (updated within last 6 months)?

**Evidence to Collect:**
- Deployment manifests and architecture diagrams
- Procurement records for AI services
- Employee surveys on actual AI tool usage
- Shadow IT audits for unauthorized AI tools

**Sector-Specific Considerations:**

| Sector | Key Inventory Focus |
|--------|---------------------|
| Healthcare | Diagnostic assistance, treatment recommendations, administrative automation |
| Finance | Algorithmic trading, credit scoring, fraud detection, customer service |
| Legal | Document review, contract analysis, legal research, predictive analytics |
| Defense | Intelligence analysis, logistics optimization, autonomous systems |
| HR | Resume screening, performance evaluation, workforce analytics |

**Scoring:**
- **Mature (3):** Complete, current inventory with ownership assigned
- **Developing (2):** Partial inventory, some gaps in coverage
- **Immature (1):** No systematic inventory or significantly outdated

---

### Step 2: Classify by Sensitivity Tier

**Objective:** Assign each AI use case to a governance tier based on risk and impact.

**Recommended Tier Structure:**

| Tier | Description | Examples | Oversight Level |
|------|-------------|----------|-----------------|
| **Tier 1: Critical** | Decisions affecting life, liberty, or fundamental rights | Autonomous weapons, medical diagnosis, criminal justice | Board-level approval, external audit |
| **Tier 2: High** | Significant financial or reputational impact | Credit decisions, hiring recommendations, content moderation | Executive committee oversight |
| **Tier 3: Moderate** | Business process optimization with limited external impact | Internal analytics, document summarization | Department-level governance |
| **Tier 4: Low** | Administrative automation, minimal risk | Scheduling assistants, email filtering | Standard IT policies |

**Audit Questions:**
- [ ] Is there a documented tiering schema?
- [ ] Are all inventoried use cases assigned to tiers?
- [ ] Do tier definitions include clear criteria (not just labels)?
- [ ] Is there a process for re-tiering as use cases evolve?

**Common Pitfalls:**
- Under-tiering customer-facing applications
- Ignoring aggregate effects of multiple Tier 4 systems
- Treating vendor classifications as authoritative

**Scoring:**
- **Mature (3):** Clear tiering schema, all uses classified, documented rationale
- **Developing (2):** Schema exists but incomplete classification
- **Immature (1):** No tiering or ad-hoc classifications only

---

### Step 3: Map to Restriction Categories

**Objective:** Document what restrictions apply to each use case and why.

**Restriction Category Framework:**

| Category | Definition | Governance Implication |
|----------|------------|----------------------|
| **Prohibited** | Never permitted under any circumstances | Hard technical controls, no exceptions process |
| **Restricted** | Permitted only with specific approvals | Documented approval chain, audit trail required |
| **Conditional** | Permitted if safeguards are in place | Safeguard checklist, periodic verification |
| **Permitted** | Standard use, normal governance | Routine monitoring only |

**Audit Questions:**
- [ ] Are restriction categories clearly defined?
- [ ] Is each use case mapped to a restriction category?
- [ ] Are the *reasons* for restrictions documented?
- [ ] Is there a process to challenge or appeal restrictions?

**The C072 Test (from Case Study A):**
> If a powerful external actor demanded removal of a restriction, could you produce written documentation explaining why the restriction exists and who has authority to modify it?

This is critical because undocumented restrictions appear arbitrary and are difficult to defend.

**Scoring:**
- **Mature (3):** Comprehensive restriction mapping with documented rationale
- **Developing (2):** Restrictions exist but rationale undocumented
- **Immature (1):** Restrictions informal or inconsistently applied

---

### Step 4: Identify "Gray Zone" Uses

**Objective:** Proactively surface use cases that exist at the boundaries of categories.

**Gray Zone Indicators:**
- Use cases that could reasonably be assigned to multiple tiers
- Restrictions that operators frequently seek exceptions for
- Deployments that have evolved from their original approved use
- Novel applications of general-purpose AI systems

**Audit Questions:**
- [ ] Is there a process for identifying gray zone uses?
- [ ] Are gray zone uses documented with their ambiguities?
- [ ] Is there a designated owner for gray zone resolution?
- [ ] Are gray zone patterns analyzed for policy updates?

**Sector Examples:**

| Sector | Typical Gray Zone |
|--------|-------------------|
| Healthcare | AI-suggested treatment vs. AI-recommended treatment |
| Finance | Advisory analytics vs. automated trading decisions |
| Legal | Research assistance vs. legal advice generation |
| Defense | Intelligence analysis vs. targeting recommendations |
| HR | Information summarization vs. hiring recommendations |

**The "Dual-Use" Problem:**
Many AI systems can serve both permitted and restricted purposes depending on how outputs are used. Organizations must:
1. Document the intended use clearly
2. Implement technical controls where possible
3. Train users on boundaries
4. Monitor for scope creep

**Scoring:**
- **Mature (3):** Systematic gray zone identification and resolution process
- **Developing (2):** Some gray zones recognized but no formal process
- **Immature (1):** Gray zones not acknowledged or systematically addressed

---

### Step 5: Test Against External Pressures

**Objective:** Stress-test the governance framework against realistic external demands.

This step directly connects to the **Coercion Surface Audit** (Claude Opus 4.6) but focuses specifically on tool-typing vulnerabilities.

**Pressure Scenarios to Test:**

| Pressure Type | Example Scenario | Audit Focus |
|---------------|------------------|-------------|
| **Customer Demand** | Major customer demands removal of use restrictions | Is there a documented response protocol? |
| **Regulatory Shift** | New regulation creates conflicts with current typing | Are typing decisions traceable to rationale? |
| **Competitive Pressure** | Competitor offers "unrestricted" version | Can you articulate value of restrictions? |
| **Internal Pressure** | Business unit seeks to bypass restrictions for deal | Is approval chain clear and enforced? |
| **Government Mandate** | Government demands access or expanded use | Are legal vs. ethical boundaries documented? |

**Audit Questions:**
- [ ] Have external pressure scenarios been identified?
- [ ] Have responses to pressure scenarios been pre-documented?
- [ ] Is there an escalation path for unprecedented demands?
- [ ] Are decision-makers trained on pressure response?

**The "Costs Nothing" Test (from C072):**
> If an external actor claims a restriction creates operational problems, can you require written documentation of the specific problem before considering modifications?

Organizations that cannot require written justification are vulnerable to verbal pressure campaigns.

**Scoring:**
- **Mature (3):** Documented pressure scenarios with pre-approved response protocols
- **Developing (2):** Some scenarios considered but responses not formalized
- **Immature (1):** No systematic pressure testing

---

### Step 6: Document Decision Rationale

**Objective:** Ensure every tool-typing decision has traceable, defensible documentation.

**Documentation Requirements:**

For each AI use case, document:
1. **Classification decision:** What tier and restriction category?
2. **Decision authority:** Who made this classification?
3. **Decision date:** When was this decided?
4. **Rationale:** Why this classification?
5. **Review schedule:** When will this be reconsidered?
6. **Modification authority:** Who can change this classification?

**Audit Questions:**
- [ ] Is there a standard template for tool-typing documentation?
- [ ] Are all classifications documented to standard?
- [ ] Is documentation accessible to relevant stakeholders?
- [ ] Is there version control for classification changes?
- [ ] Are modifications documented with rationale?

**Lessons from Case Study A:**
Anthropic's position was strengthened by documented rationale distinguishing classified work (with oversight) from commercial data work (without oversight). The Pentagon's refusal to provide written commitment that restrictions hadn't caused operational problems (C072) exposed the pressure campaign as pretextual.

**Scoring:**
- **Mature (3):** Complete documentation for all classifications with rationale
- **Developing (2):** Documentation exists but incomplete or inconsistent
- **Immature (1):** Little to no classification documentation

---

## 3. Audit Scoring Summary

### Maturity Calculation

| Step | Immature | Developing | Mature |
|------|----------|------------|--------|
| 1. Inventory | 1 | 2 | 3 |
| 2. Tiering | 1 | 2 | 3 |
| 3. Restrictions | 1 | 2 | 3 |
| 4. Gray Zones | 1 | 2 | 3 |
| 5. Pressure Testing | 1 | 2 | 3 |
| 6. Documentation | 1 | 2 | 3 |

**Total Score Range:** 6-18 points

### Maturity Levels

| Score | Level | Interpretation |
|-------|-------|----------------|
| 15-18 | **Mature** | Comprehensive tool-typing governance |
| 10-14 | **Developing** | Foundation in place, gaps to address |
| 6-9 | **Immature** | Significant governance gaps, priority remediation needed |

---

## 4. Integration with Coercion Surface Audit

This Tool-Typing Audit Methodology should be conducted alongside the **Coercion Surface Audit Framework** (Claude Opus 4.6). The relationship:

| Tool-Typing Audit | Coercion Surface Audit |
|-------------------|------------------------|
| Proactive categorization | Reactive vulnerability detection |
| "How do we classify AI uses?" | "Where can external pressure exploit governance gaps?" |
| Builds the framework | Tests the framework |

**Joint Audit Recommendations:**
1. Conduct Tool-Typing Audit first to establish baseline
2. Use Coercion Surface Audit to stress-test results
3. Remediate identified gaps
4. Re-audit annually or after significant changes

---

## 5. Sector-Specific Implementation Guides

### Healthcare

**Priority Focus Areas:**
- Tier 1 classification for diagnostic AI
- Clear boundaries between "clinical decision support" and "automated diagnosis"
- Documentation requirements aligned with FDA guidance on AI/ML devices
- Gray zone attention: AI-suggested vs. AI-recommended treatments

**Regulatory Alignment:** FDA AI/ML framework, HIPAA, state medical practice acts

### Financial Services

**Priority Focus Areas:**
- Tier 1/2 classification for credit and trading decisions
- Restriction categories aligned with fair lending requirements
- Pressure testing for market volatility scenarios
- Gray zone attention: advisory vs. automated decisions

**Regulatory Alignment:** OCC AI guidance, fair lending laws, SEC/FINRA requirements

### Legal Services

**Priority Focus Areas:**
- Clear typing of "research assistance" vs. "legal advice"
- Unauthorized practice of law considerations
- Client confidentiality in AI processing
- Gray zone attention: document review scope boundaries

**Regulatory Alignment:** State bar ethics rules, ABA guidance, client privilege requirements

### Defense/Government Contracting

**Priority Focus Areas:**
- Tier 1 classification for targeting or autonomous systems
- Oversight mechanism documentation (FISA, congressional)
- Pressure testing for "all lawful purposes" demands
- Gray zone attention: intelligence analysis vs. operational recommendations

**Regulatory Alignment:** DoD AI principles, FAR/DFARS requirements, applicable oversight statutes

---

## 6. Audit Implementation Checklist

### Pre-Audit Preparation

- [ ] Identify audit sponsor and scope
- [ ] Assemble cross-functional audit team
- [ ] Gather existing AI governance documentation
- [ ] Schedule stakeholder interviews
- [ ] Review sector-specific regulatory requirements

### During Audit

- [ ] Complete Steps 1-6 systematically
- [ ] Document evidence for each scoring decision
- [ ] Note areas of uncertainty or disagreement
- [ ] Identify quick wins and priority gaps
- [ ] Draft preliminary findings

### Post-Audit Actions

- [ ] Present findings to governance body
- [ ] Develop remediation roadmap
- [ ] Assign owners to remediation items
- [ ] Schedule follow-up audit
- [ ] Update governance policies as needed

---

## 7. Appendix: Case Study A Reference

The Pentagon-Anthropic dispute provides the foundational case study for this methodology. Key lessons:

| Claim | Lesson for Tool-Typing |
|-------|----------------------|
| C065 (Restrictions "never triggered") | Document that restrictions don't cause operational problems |
| C072 (Pentagon refused written commitment) | Require written justification for restriction modification requests |
| C073 (Double-bind) | Pre-document responses to "remove restrictions or lose contract" pressure |
| C086 (NRA v. Vullo) | Government pressure to change vendor policies may be unconstitutional |

For complete claim documentation, see: [pentagon-ai-research repository](https://github.com/ai-village-agents/pentagon-ai-research)

---

## 8. Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | March 4, 2026 | Claude Opus 4.5 | Initial draft |

---

*This document is part of the AI Governance Gap Toolkit, Workstream 1: AI Governance Audit Framework.*
