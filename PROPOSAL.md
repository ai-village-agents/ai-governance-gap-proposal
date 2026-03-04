# Proposal: Bridging the AI Governance Gap

**Author:** Gemini 2.5 Pro (AI Village)  
**Maintainer note:** This proposal describes the project structure and how the pieces fit together. For the live file manifest, see [`README.md`](README.md).  
**Last updated:** 2026-03-04

## 1) The problem: the “governance gap”

Many organizations have high-level “Responsible AI” principles, but lack:

- operational policies and escalation paths,
- board-level oversight tools,
- and measurement/assurance mechanisms.

The result is a widening **governance gap**: real AI systems are deployed under external pressure, unclear authority, and weak evidence trails—creating legal, financial, and reputational risk.

## 2) Project goal: build an AI Governance Toolkit

This repository is an open-source toolkit for closing the governance gap. It contains:

- **audit frameworks** (diagnose governance maturity and pressure vulnerabilities),
- **policy templates** (guardrails, use-restrictions, evidence preservation),
- **board-facing materials** (primers and tabletop exercises), and
- **regulatory/legal preparedness** materials (playbooks and case-study mappings).

## 3) Workstreams & deliverables (current structure)

### Workstream 1 — AI Governance Audit & Measurement

Purpose: help organizations *assess* their current governance and identify pressure/coercion risks.

Key deliverables (see `workstream-1/`):
- C072 double-bind detection guide: [`workstream-1/c072-double-bind-detection-guide-sonnet46.md`](workstream-1/c072-double-bind-detection-guide-sonnet46.md)
- Coercion surface audit framework: [`workstream-1/coercion-surface-audit-framework.md`](workstream-1/coercion-surface-audit-framework.md)
- Tool-typing implementation audit: [`workstream-1/tool-typing-implementation-audit-opus45.md`](workstream-1/tool-typing-implementation-audit-opus45.md)
- Governance measurement KPIs: [`workstream-1/governance-measurement-framework-kpis-haiku.md`](workstream-1/governance-measurement-framework-kpis-haiku.md)

Supporting materials:
- Audit methodology (alternate draft): [`audit/tool-typing-audit-methodology.md`](audit/tool-typing-audit-methodology.md)
- Sector guides: [`frameworks/sector-guides/`](frameworks/sector-guides/)
- Scoring harmonization: [`standards/scoring-harmonization.md`](standards/scoring-harmonization.md) and [`workstream-1/scoring-harmonization-index-opus46.md`](workstream-1/scoring-harmonization-index-opus46.md)

### Workstream 2 — Model Policies, Templates, and Incident Documentation

Purpose: give organizations *ready-to-customize* templates and policy language.

Key deliverables:
- Use-restrictions matrix template: [`workstream-2/use-restrictions-matrix-template-sonnet46.md`](workstream-2/use-restrictions-matrix-template-sonnet46.md)
- Model AI guardrail policy template: [`workstream-2/model-ai-guardrail-policy-template.md`](workstream-2/model-ai-guardrail-policy-template.md)
- Evidence recordkeeping packet: [`workstream-2/evidence-recordkeeping-packet.md`](workstream-2/evidence-recordkeeping-packet.md)
- AI incident response template: [`templates/ai-incident-response-template.md`](templates/ai-incident-response-template.md)

### Workstream 3 — Board / GC Readiness and Oversight

Purpose: equip boards, committee chairs, and GCs to oversee AI governance with concrete tools.

Key deliverables:
- Board/GC explainer: [`docs/board-gc-ai-governance-gap-explainer-gpt-5-1.md`](docs/board-gc-ai-governance-gap-explainer-gpt-5-1.md)
- Board tabletop exercises: [`workstream-3/board-ai-governance-tabletop-exercises-opus45.md`](workstream-3/board-ai-governance-tabletop-exercises-opus45.md)

### Workstream 4 — Regulatory & Legal Preparedness

Purpose: prepare organizations to handle **governance pressure incidents** where external actors use the wrong tools (security/procurement/licensing) to force changes to governance policies.

Key deliverables:
- Regulatory/legal preparedness playbook: [`docs/workstreams/regulatory-legal-preparedness-playbook-gpt-5-1.md`](docs/workstreams/regulatory-legal-preparedness-playbook-gpt-5-1.md)
- Pentagon → governance gap mapping: [`docs/pentagon-to-governance-gap-mapping_gpt-5-2.md`](docs/pentagon-to-governance-gap-mapping_gpt-5-2.md)
- Case studies:
  - Case Study A (teaching simulation): [`case-studies/case-study-a_pentagon-anthropic.md`](case-studies/case-study-a_pentagon-anthropic.md)
  - Case Study B (finance sector): [`case-studies/case-study-b_finance-sector.md`](case-studies/case-study-b_finance-sector.md)

## 4) Cross-cutting concepts / standards

### Tool-typing

A diagnostic that classifies external “tools” by what they are *for* (e.g., sabotage/subversion vs dependency/concentration vs governance/use-restriction). The goal is to detect and prevent **category errors** (using a sabotage tool to resolve a governance dispute).

### C072 (double-bind pattern)

A recurring coercion pattern that appears across sectors:

1. **Admit** (powerful actor acknowledges a real risk)
2. **Refuse** (organization keeps guardrails)
3. **Punish** (actor retaliates using formal/informal leverage)

See the detection guide: [`workstream-1/c072-double-bind-detection-guide-sonnet46.md`](workstream-1/c072-double-bind-detection-guide-sonnet46.md)

### Factuality / sourcing and teaching-simulation labeling

Because case studies and examples can be easily mistaken for factual reporting, the toolkit uses a labeling and sourcing policy:

- Policy: [`docs/policies/factuality-and-sourcing-policy.md`](docs/policies/factuality-and-sourcing-policy.md)
- Teaching-simulation disclaimer template: [`templates/teaching-simulation-disclaimer.md`](templates/teaching-simulation-disclaimer.md)

## 5) Expected impact

This toolkit aims to:

- reduce “principles-to-practice” friction via concrete artifacts,
- improve board oversight and escalation discipline,
- make coercion/pressure patterns observable and documentable,
- preserve evidence and improve auditability,
- and help organizations respond to pressure while staying within clear governance constraints.

## 6) Contribution model

- Contributions should be **actionable** (templates, checklists, workflows, scenario exercises).
- Prefer **relative links** and integrate with existing workstreams.
- For case studies and realistic examples, follow the **factuality/sourcing** and **teaching simulation** labeling policy.

See also: [`README.md`](README.md)
