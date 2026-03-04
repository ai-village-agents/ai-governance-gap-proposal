# Cross-Jurisdictional AI Governance Framework Mapping

**Author:** Claude Opus 4.5  
**Workstream:** 1 - AI Governance Audit Framework  
**Version:** 1.0  
**Date:** March 4, 2026

## Executive Summary

Organizations operating across jurisdictions face a fragmented AI regulatory landscape. This document maps the AI Governance Gap Toolkit's audit framework to major regulatory regimes, enabling organizations to maintain compliance while implementing consistent governance practices.

This mapping addresses the gap identified by Claude Sonnet 4.6: the absence of cross-jurisdictional compatibility in the toolkit.

---

## 1. Regulatory Landscape Overview

### Major AI Governance Frameworks

| Framework | Jurisdiction | Status | Primary Focus |
|-----------|--------------|--------|---------------|
| **EU AI Act** | European Union | In force (phased) | Risk-based regulation, prohibited uses |
| **NIST AI RMF** | United States | Voluntary | Risk management, trustworthy AI |
| **UK AI Regulation** | United Kingdom | Sector-specific | Pro-innovation, principles-based |
| **AI Safety Institute** | UK | Advisory | Frontier AI safety evaluation |
| **Canada AIDA** | Canada | Proposed | High-impact systems regulation |
| **China AI Regulations** | China | In force | Algorithm registration, content rules |
| **Singapore AI Governance** | Singapore | Voluntary | Model framework, sector guides |

---

## 2. EU AI Act Alignment

### Risk Categories Mapping

The EU AI Act uses a four-tier risk classification. Our Toolkit's tiering maps as follows:

| EU AI Act Category | Toolkit Tier | Implications |
|-------------------|--------------|--------------|
| **Unacceptable Risk** (Prohibited) | Tier 1 + Prohibited restriction | Social scoring, real-time biometric ID (most), manipulative AI |
| **High Risk** | Tier 1-2 + Restricted | Critical infrastructure, education, employment, law enforcement |
| **Limited Risk** | Tier 2-3 + Conditional | Chatbots, emotion recognition, deepfakes (transparency required) |
| **Minimal Risk** | Tier 3-4 + Permitted | Most AI applications (voluntary codes) |

### Audit Checklist: EU AI Act Compliance

For organizations subject to EU AI Act:

**Prohibited Systems Check:**
- [ ] Have we inventoried all AI systems against Article 5 prohibited practices?
- [ ] Are any systems performing social scoring, manipulative techniques, or prohibited biometric identification?
- [ ] Is there a process to catch new deployments that might cross prohibition boundaries?

**High-Risk System Governance:**
- [ ] Are high-risk systems registered in the EU database (when required)?
- [ ] Is there conformity assessment documentation?
- [ ] Are quality management systems in place per Article 17?
- [ ] Is technical documentation maintained per Annex IV?
- [ ] Are human oversight measures implemented per Article 14?

**General-Purpose AI (GPAI) Requirements:**
- [ ] Are GPAI models documented per Article 53?
- [ ] Is there a copyright compliance policy?
- [ ] For systemic risk models: Is there a model evaluation protocol?

### C072 Double-Bind Under EU AI Act

The EU AI Act creates specific coercion surface considerations:

| Pressure Scenario | EU AI Act Implication |
|-------------------|----------------------|
| Customer demands removal of safety guardrails | May violate Article 9 risk management requirements |
| Government demands expanded surveillance use | May cross into prohibited practices (Article 5) |
| Business unit seeks to bypass fairness checks | May violate high-risk system requirements (Annex III) |

**Key Principle:** EU AI Act requirements can serve as *external justification* for maintaining guardrails against pressure.

---

## 3. NIST AI RMF Alignment

### Framework Structure

The NIST AI Risk Management Framework uses four core functions:

| NIST Function | Toolkit Alignment |
|---------------|-------------------|
| **GOVERN** | Board oversight (WS3), Policy frameworks (WS2) |
| **MAP** | Step 1: Inventory, Step 4: Gray zones |
| **MEASURE** | Step 2: Tiering, Maturity scoring |
| **MANAGE** | Step 3: Restrictions, Step 5: Pressure testing |

### Crosswalk: Toolkit Steps to NIST Characteristics

| NIST Trustworthy AI Characteristic | Toolkit Coverage |
|-----------------------------------|------------------|
| **Valid and Reliable** | Step 2 tiering criteria, Step 6 documentation |
| **Safe** | Step 3 restriction categories, Coercion Surface Audit |
| **Secure and Resilient** | Step 5 pressure testing |
| **Accountable and Transparent** | Step 6 decision rationale, Step 1 inventory |
| **Explainable and Interpretable** | Gray zone identification (Step 4) |
| **Privacy-Enhanced** | Restriction mapping (Step 3) |
| **Fair with Harmful Bias Managed** | Tiering criteria, restriction categories |

### Audit Checklist: NIST AI RMF Integration

- [ ] Have we mapped our AI governance to NIST AI RMF functions?
- [ ] Are GOVERN structures (roles, policies, culture) documented?
- [ ] Is there a MAP process for context and categorization?
- [ ] Are MEASURE metrics defined for each AI system?
- [ ] Are MANAGE processes (response, monitoring) operational?

---

## 4. UK AI Regulation Alignment

### Pro-Innovation Principles

The UK takes a sector-specific, principles-based approach:

| UK AI Principle | Toolkit Alignment |
|----------------|-------------------|
| **Safety, security, robustness** | Step 5 pressure testing, Coercion Surface Audit |
| **Transparency and explainability** | Step 6 documentation |
| **Fairness** | Step 2-3 tiering and restrictions |
| **Accountability and governance** | All steps, Board oversight (WS3) |
| **Contestability and redress** | Step 4 gray zones, appeal processes |

### Sector Regulator Mapping

| UK Sector Regulator | AI Governance Focus |
|--------------------|---------------------|
| **FCA** (Financial Conduct) | Algorithmic trading, credit decisions |
| **MHRA** (Medicines) | Medical device AI |
| **CMA** (Competition) | Algorithmic collusion, market fairness |
| **ICO** (Data Protection) | Automated decision-making, profiling |
| **Ofcom** (Communications) | Content moderation AI |

### UK AI Safety Institute Integration

For organizations deploying frontier AI or working with AISI:

- [ ] Have we engaged with AISI evaluation frameworks?
- [ ] Are model evaluations documented to AISI standards?
- [ ] Is there a process for reporting concerning capabilities?

---

## 5. Multi-Jurisdictional Compliance Matrix

### Harmonization Challenges

| Challenge | Mitigation Strategy |
|-----------|---------------------|
| **Conflicting requirements** | Default to most restrictive standard |
| **Different risk thresholds** | Map to highest-applicable tier |
| **Varying documentation requirements** | Maintain superset documentation |
| **Enforcement uncertainty** | Document rationale for jurisdictional choices |

### Practical Compliance Approach

**Step 1: Jurisdiction Inventory**
- List all jurisdictions where AI systems are deployed or affect individuals
- Identify applicable regulatory frameworks per jurisdiction
- Note sector-specific requirements

**Step 2: Requirements Mapping**
- For each AI system, map requirements from all applicable frameworks
- Identify conflicts and harmonization opportunities
- Document compliance approach per requirement

**Step 3: Gap Analysis**
- Compare current governance against mapped requirements
- Prioritize gaps by risk and enforcement likelihood
- Create remediation roadmap

**Step 4: Unified Governance**
- Design governance that satisfies all applicable frameworks
- Document how each framework's requirements are met
- Establish monitoring for regulatory changes

---

## 6. Pentagon Case Study: Jurisdictional Lessons

Case Study A (Pentagon-Anthropic) illustrates jurisdictional complexity in government contracting:

### Applicable Frameworks

| Framework | Application |
|-----------|-------------|
| **10 USC § 3252** | Supply chain risk designation |
| **FASCSA** | Contracting exclusion (avoided) |
| **DoD AI Principles** | Ethical use guidelines |
| **FISA** | Surveillance oversight |

### Cross-Jurisdictional Insights

1. **Forum Shopping:** Government chose § 3252 over FASCSA to avoid procedural protections
2. **Framework Mismatch:** Supply chain statute used for governance dispute
3. **Oversight Gaps:** Commercial data uses lacked the oversight of classified work
4. **International Implications:** US AI policy affects global AI governance norms

### Audit Lesson

When facing regulatory pressure, organizations should:
- Document which framework the pressure invokes
- Assess whether the framework is properly typed for the dispute
- Identify alternative frameworks that might apply
- Consider cross-jurisdictional consistency implications

---

## 7. Regulatory Change Monitoring

### Establishing a Watch Process

- [ ] Assign regulatory monitoring responsibility
- [ ] Subscribe to official regulatory feeds
- [ ] Monitor industry association updates
- [ ] Track academic/policy analysis
- [ ] Schedule quarterly governance review

### Key Sources

| Jurisdiction | Primary Sources |
|--------------|-----------------|
| **EU** | EUR-Lex, AI Office communications, EDPB guidance |
| **US** | NIST, OSTP, FTC, SEC, sector regulators |
| **UK** | DSIT, sector regulators, AI Safety Institute |
| **International** | OECD AI Policy Observatory, GPAI |

---

## 8. Implementation Checklist

### For Organizations New to Multi-Jurisdictional AI Governance

**Week 1-2:**
- [ ] Complete jurisdiction inventory
- [ ] Identify applicable frameworks
- [ ] Assign regulatory monitoring owner

**Week 3-4:**
- [ ] Map AI systems to framework requirements
- [ ] Identify highest-risk compliance gaps
- [ ] Begin gap remediation planning

**Month 2:**
- [ ] Implement unified documentation standards
- [ ] Train governance team on multi-jurisdictional requirements
- [ ] Establish regulatory change monitoring

**Month 3:**
- [ ] Complete first compliance audit against mapped requirements
- [ ] Document compliance posture per framework
- [ ] Create ongoing compliance maintenance plan

---

## 9. Appendix: Quick Reference Tables

### EU AI Act Timeline

| Milestone | Date | Requirement |
|-----------|------|-------------|
| Prohibitions effective | Feb 2025 | Article 5 prohibited practices |
| GPAI obligations | Aug 2025 | General-purpose AI requirements |
| High-risk (Annex III) | Aug 2026 | Full high-risk system compliance |
| High-risk (Annex II) | Aug 2027 | Product-embedded AI systems |

### Framework Comparison: Risk Thresholds

| Risk Level | EU AI Act | NIST AI RMF | UK Approach |
|------------|-----------|-------------|-------------|
| **Highest** | Prohibited (banned) | Risk tolerance = 0 | Sector regulator determination |
| **High** | Mandatory requirements | Formal risk management | Proportionate oversight |
| **Medium** | Transparency requirements | Standard practices | Principles-based |
| **Low** | Voluntary codes | Basic documentation | Minimal intervention |

---

## 10. Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | March 4, 2026 | Claude Opus 4.5 | Initial draft |

---

*This document is part of the AI Governance Gap Toolkit, Workstream 1: AI Governance Audit Framework.*
