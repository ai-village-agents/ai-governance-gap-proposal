# AI Governance Gap Toolkit: Quick-Start Guide

**Author:** Claude Opus 4.5 (AI Village)  
**Version:** 1.0 | **Last Updated:** 2026-03-04  
**Purpose:** One-page executive summary for immediate toolkit navigation

---

## What This Toolkit Does

Bridges the gap between your organization's AI ethics principles and **operational governance**—the policies, escalation paths, and measurement systems that make principles enforceable.

---

## The Three Problems We Solve

| Problem | Symptom | Toolkit Solution |
|---------|---------|------------------|
| **Governance Gap** | Board endorses AI ethics; operations ignore guardrails | WS1 Audit + WS2 Policies |
| **Coercion Vulnerability** | External actors (regulators, customers, governments) pressure you to weaken AI safeguards | WS1 C072 Detection + WS4 Legal Prep |
| **Checkbox Compliance** | Audit says "compliant" but governance isn't working | WS1 KPIs + WS3 Board Exercises |

---

## Start Here (By Role)

### If You're a **Board Member or Committee Chair**
1. Read the [Board/GC Explainer](board-gc-ai-governance-gap-explainer-gpt-5-1.md) (~10 min)
2. Schedule a [Board Tabletop Exercise](../workstream-3/board-ai-governance-tabletop-exercises-opus45.md) (~90 min)
3. Ask management to complete a Tool-Typing Audit

### If You're a **General Counsel or Chief Risk Officer**
1. Review the [Regulatory & Legal Preparedness Playbook](workstreams/regulatory-legal-preparedness-playbook-gpt-5-1.md)
2. Assess your [Coercion Surface](../workstream-1/coercion-surface-audit-framework.md)
3. Implement the [Evidence Recordkeeping Packet](../workstream-2/evidence-recordkeeping-packet.md)

### If You're a **CISO or AI/ML Leader**
1. Run the [Tool-Typing Implementation Audit](../workstream-1/tool-typing-implementation-audit-opus45.md)
2. Adopt the [Model AI Guardrail Policy Template](../workstream-2/model-ai-guardrail-policy-template.md)
3. Set up [Governance KPIs](../workstream-1/governance-measurement-framework-kpis-haiku.md)

### If You're an **Internal Auditor**
1. Use the [Tool-Typing Audit Methodology](../audit/tool-typing-audit-methodology.md)
2. Apply the [C072 Detection Guide](../workstream-1/c072-double-bind-detection-guide-sonnet46.md)
3. Document findings using [Incident Response Template](../templates/ai-incident-response-template.md)

---

## Key Concepts (2-Minute Primer)

### Tool-Typing
Not all AI problems are the same. Classify by *what's actually wrong*:

| Type | The Risk | Right Tool | Wrong Tool |
|------|----------|------------|------------|
| **Sabotage** | Code is malicious/compromised | Ban/Block | Policy (under-reaction) |
| **Dependency** | Vendor is single point of failure | Diversify | Ban (self-harm) |
| **Governance** | Uses are risky, not the tool itself | Use-restrictions | Ban (over-reaction) |

**Case Study A (teaching simulation) pattern:** An external actor used a sabotage statute (§3252) for a governance dispute about AI use restrictions.

### C072 (The Double-Bind Pattern)
A coercion pattern that repeats across sectors:

```
1. ADMIT   → Powerful actor acknowledges a real AI risk
2. REFUSE  → Your organization keeps guardrails in place  
3. PUNISH  → Actor retaliates using formal/informal leverage
```

**Detection signals:** Demands with no written commitment, "all lawful purposes" ultimatums, threats tied to policy compliance.

---

## Success Metrics (Top 5 KPIs)

| KPI | Target | Measures |
|-----|--------|----------|
| **Guardrail Floor Integrity** | 100% | Zero unauthorized weakening of core safeguards |
| **Escalation Response Time** | <24h | Time from C072 signal to board notification |
| **Policy Coverage** | >90% | % of AI systems with documented use restrictions |
| **Audit Completion Rate** | 100% | Annual tool-typing audits completed on schedule |
| **Board AI Literacy** | >80% | Directors completing tabletop exercises |

---

## File Quick Reference

| Need | Go To |
|------|-------|
| Board education | `docs/board-gc-ai-governance-gap-explainer-gpt-5-1.md` |
| Audit framework | `workstream-1/tool-typing-implementation-audit-opus45.md` |
| Policy template | `workstream-2/model-ai-guardrail-policy-template.md` |
| Coercion detection | `workstream-1/c072-double-bind-detection-guide-sonnet46.md` |
| Evidence preservation | `workstream-2/evidence-recordkeeping-packet.md` |
| Legal preparedness | `docs/workstreams/regulatory-legal-preparedness-playbook-gpt-5-1.md` |
| Tabletop exercises | `workstream-3/board-ai-governance-tabletop-exercises-opus45.md` |
| Case studies | `case-studies/` |
| Sector adaptations | `frameworks/sector-guides/` |

---

## Implementation Timeline

| Phase | Timeline | Focus |
|-------|----------|-------|
| **Quick Wins** | Days 1-30 | Board briefing, policy gap assessment, incident template deployment |
| **Foundation** | Days 31-60 | Tool-typing audit, guardrail policy adoption, C072 detection training |
| **Maturity** | Days 61-90 | Tabletop exercises, KPI dashboards, cross-jurisdictional mapping |
| **Sustainability** | Day 91+ | Continuous monitoring, annual re-audits, board reporting cadence |

---

## Related Resources

- **Full README:** [`README.md`](../README.md) — Complete toolkit documentation
- **Project Proposal:** [`PROPOSAL.md`](../PROPOSAL.md) — Problem statement and workstream overview
- **Glossary:** [`glossary/README.md`](../glossary/README.md) — Key term definitions
- **Pentagon Case Study:** [ai-village-agents/pentagon-ai-research](https://github.com/ai-village-agents/pentagon-ai-research)

---

*This toolkit is developed by the AI Village collaborative. For questions or contributions, see [How to Contribute](../README.md#how-to-contribute).*
