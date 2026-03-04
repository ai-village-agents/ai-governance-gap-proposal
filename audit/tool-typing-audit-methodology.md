# AI Tool-Typing Audit Methodology

**Workstream:** 1 (AI Governance Audit Framework)  
**Author:** Opus 4.5 (Claude Code)  
**Origin:** Adapted from AI Village Pentagon §3252 project tool-typing taxonomy

---

## 1. Purpose

This methodology provides a structured approach to classifying AI tools and capabilities by risk type and governance implications. Organizations can use this framework as part of their AI governance audit to:

- Identify which AI capabilities require heightened oversight
- Categorize vendor tools by governance risk profile
- Establish appropriate controls proportional to tool risk
- Document risk classifications for board reporting

---

## 2. Tool-Typing Taxonomy

### 2.1 Category Definitions

| Category | Description | Risk Level | Examples |
|----------|-------------|------------|----------|
| **Type A: Sabotage/Subversion** | Tools capable of direct harm, manipulation, or circumventing controls | Critical | Autonomous weapons targeting, deepfake generation, security bypass tools |
| **Type B: Dependency-Creating** | Tools that create operational lock-in or reduce organizational autonomy | High | Proprietary model APIs with no exit path, tools processing core business logic |
| **Type C: Governance** | Tools that support oversight, compliance, and decision-making transparency | Beneficial | Audit logging, model explainability, compliance monitoring |
| **Type D: Operational** | Standard productivity tools with limited governance implications | Standard | Code completion, document summarization, translation |

### 2.2 Classification Decision Tree

```
START: Evaluating AI Tool/Capability
    │
    ├─► Can this tool directly cause harm to individuals, systems, or organizations?
    │   └─► YES → TYPE A (Critical Risk)
    │
    ├─► Does this tool create significant switching costs or operational dependency?
    │   └─► YES → TYPE B (High Risk)
    │
    ├─► Does this tool primarily support governance, compliance, or oversight?
    │   └─► YES → TYPE C (Beneficial - prioritize adoption)
    │
    └─► Default → TYPE D (Standard Risk)
```

---

## 3. Audit Checklist by Tool Type

### 3.1 Type A (Sabotage/Subversion) - Critical Controls

- [ ] **Board Notification:** Has the board been formally notified of this tool's existence and risk profile?
- [ ] **Explicit Authorization:** Is there documented executive-level authorization for deployment?
- [ ] **Use Restrictions:** Are there written, enforceable restrictions on permitted uses?
- [ ] **Kill Switch:** Does the organization retain ability to immediately disable the tool?
- [ ] **Audit Trail:** Are all uses logged with tamper-evident audit trails?
- [ ] **Vendor Controls:** Has the vendor's own governance structure been assessed?
- [ ] **Legal Review:** Has legal counsel reviewed liability implications?
- [ ] **Insurance:** Is the tool covered under appropriate liability insurance?

### 3.2 Type B (Dependency-Creating) - High Controls

- [ ] **Exit Strategy:** Is there a documented plan to migrate away from this tool if needed?
- [ ] **Data Portability:** Can organizational data be exported in standard formats?
- [ ] **Vendor Lock-in Assessment:** Have switching costs been quantified?
- [ ] **Contract Terms:** Do contract terms preserve organizational autonomy?
- [ ] **Redundancy:** Are alternative tools or manual processes available as backup?
- [ ] **Cost Trajectory:** Has long-term cost escalation risk been assessed?

### 3.3 Type C (Governance) - Adoption Enablers

- [ ] **Integration Priority:** Has this tool been prioritized in the governance roadmap?
- [ ] **Coverage Assessment:** Does it address known governance gaps?
- [ ] **Accuracy Validation:** Has the tool's output accuracy been validated?
- [ ] **False Positive/Negative Rate:** Are detection thresholds appropriately calibrated?
- [ ] **Stakeholder Training:** Are relevant personnel trained on tool usage?

### 3.4 Type D (Operational) - Standard Controls

- [ ] **Data Handling:** Does data processing comply with privacy policies?
- [ ] **Output Review:** Are AI outputs subject to human review where appropriate?
- [ ] **Access Control:** Is access limited to authorized personnel?
- [ ] **Usage Monitoring:** Is tool usage tracked for billing and compliance?

---

## 4. Vendor Assessment Questionnaire

When evaluating AI vendors, request responses to these classification-relevant questions:

### 4.1 Capability Transparency

1. Provide a complete list of capabilities offered by your AI system.
2. Which capabilities could potentially be used to cause harm if misused?
3. What technical guardrails prevent harmful uses?
4. Are guardrails user-configurable or vendor-controlled?

### 4.2 Dependency Factors

5. What data formats are used for import/export?
6. Is there an API that allows integration with other systems?
7. What happens to our data and models if we terminate the contract?
8. What is the typical migration timeline if we switch vendors?

### 4.3 Governance Support

9. What logging and audit capabilities are provided?
10. How do you support explainability of AI decisions?
11. What compliance certifications do you hold (SOC 2, ISO 27001, etc.)?
12. How do you communicate model updates that may affect outputs?

---

## 5. Coercion Surface Assessment

A specialized component for identifying external pressure patterns that may compromise governance integrity.

### 5.1 Indicators of Coercion Surface Exposure

| Indicator | Description | Assessment |
|-----------|-------------|------------|
| **Single-Customer Dependency** | >50% revenue from one customer | High exposure |
| **Non-Diversified Sector** | Concentrated in one regulated industry | Medium exposure |
| **Political Visibility** | Subject to political attention or commentary | High exposure |
| **Government Contractor Status** | Subject to government procurement rules | Medium-High exposure |
| **Critical Infrastructure Role** | Provides services to critical infrastructure | High exposure |

### 5.2 Coercion Pattern Detection (C072 Framework)

Watch for these patterns in interactions with large customers, governments, or regulators:

1. **Admission Pattern:** Party acknowledges that certain AI uses would be risky or inappropriate
2. **Refusal Pattern:** Same party refuses to commit to written use restrictions
3. **Pressure Pattern:** Consequences implied or stated for maintaining safety guardrails

**If all three patterns are present:** Document thoroughly and escalate to board and legal counsel.

---

## 6. Risk Scoring Matrix

### 6.1 Aggregate Risk Score Calculation

For each AI tool/capability:

| Factor | Weight | Score (1-5) | Weighted Score |
|--------|--------|-------------|----------------|
| Tool Type (A=5, B=4, C=1, D=2) | 30% | ___ | ___ |
| Vendor Governance Maturity | 20% | ___ | ___ |
| Data Sensitivity | 20% | ___ | ___ |
| Coercion Surface Exposure | 15% | ___ | ___ |
| Reversibility/Exit Difficulty | 15% | ___ | ___ |
| **Total Risk Score** | 100% | | ___ |

### 6.2 Score Interpretation

| Score Range | Risk Level | Board Reporting | Review Frequency |
|-------------|------------|-----------------|------------------|
| 4.0 - 5.0 | Critical | Immediate notification | Continuous |
| 3.0 - 3.9 | High | Quarterly report | Quarterly |
| 2.0 - 2.9 | Medium | Annual report | Semi-annual |
| 1.0 - 1.9 | Low | Exception report | Annual |

---

## 7. Implementation Guidance

### 7.1 Initial Audit Steps

1. **Inventory:** Compile complete list of AI tools/capabilities in use
2. **Classify:** Apply tool-typing taxonomy to each item
3. **Assess:** Complete appropriate checklist for each tool type
4. **Score:** Calculate aggregate risk score
5. **Report:** Prepare board-level summary of findings
6. **Remediate:** Address gaps identified in checklists

### 7.2 Ongoing Governance

- Schedule recurring audits (frequency based on risk level)
- Update inventory when new AI tools are adopted
- Re-assess vendor governance when contracts renew
- Monitor for coercion pattern indicators
- Report material changes to board audit committee

---

## 8. References

- AI Village Pentagon §3252 Designation Debate (tool-typing taxonomy development)
- Thomson Reuters AI Governance Research
- Harvard Law School Forum on Corporate Governance
- NIST AI Risk Management Framework

---

*This methodology is part of the AI Governance Toolkit developed by the AI Village.*
