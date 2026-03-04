# WS1 Scoring Harmonization Index

**Author:** Claude Opus 4.6  
**Workstream:** 1 — AI Governance Audit Framework  
**Version:** 1.0  
**Date:** March 4, 2026

---

## Executive Summary

Workstream 1 of the AI Governance Gap Toolkit contains six complementary diagnostic frameworks, four of which use **different scoring systems**. Before these can be merged or used together in a single organizational assessment, practitioners need a common scoring layer that translates between them without flattening the distinct diagnostic dimensions each measures.

This document provides:
1. A **conversion table** mapping all four scoring systems to a normalized 0–100 scale
2. A **composite Governance Readiness Index (GRI)** that weights the four dimensions
3. A **RAG dashboard tier** for executive/board-level summary reporting
4. **Worked examples** applying the harmonized scoring to the Pentagon case study

---

## Problem Statement

| PR | Framework | Scoring System | What It Measures |
|----|-----------|----------------|-----------------|
| #6 (Opus 4.5) | Tool-Typing Implementation Audit | **6–18 points** (3 domains × 1–6 each) | Organizational tool-typing maturity |
| #7 (Opus 4.6) | Coercion Surface Audit | **0–100 weighted** (5 domains, exposure-adjusted) | Coercion vulnerability/exposure |
| #11 (Sonnet 4.6) | C072 Detection Guide | **Low / Medium / High** (qualitative) | C072 double-bind risk level |
| #16 (Haiku 4.5) | Governance Measurement Framework | **0–5 maturity levels** + domain KPIs | Overall governance maturity |

These four systems are **not interchangeable** — they measure fundamentally different things:
- **PR #6** asks: "Can we correctly classify external tools?" (capability)
- **PR #7** asks: "How exposed are we to coercion?" (vulnerability)
- **PR #11** asks: "Is a C072 pattern present or emerging?" (threat detection)
- **PR #16** asks: "How mature is our governance overall?" (maturity)

A single organization could score well on one dimension and poorly on another. Flattening all four into one number would lose this diagnostic power.

---

## Layer 1: Normalized Conversion Table (0–100)

Each scoring system is mapped to a common 0–100 scale to enable comparison and aggregation.

### PR #6: Tool-Typing Implementation Audit (6–18 → 0–100)

| Raw Score (6–18) | Normalized (0–100) | Interpretation |
|-------------------|---------------------|----------------|
| 6–7 | 0–8 | No functional tool-typing capability |
| 8–9 | 9–25 | Minimal awareness; ad hoc classification |
| 10–11 | 26–42 | Basic classification exists but inconsistent |
| 12–13 | 43–58 | Moderate capability; most tools classified correctly |
| 14–15 | 59–75 | Strong classification with documented rationale |
| 16–17 | 76–92 | Advanced maturity; systematic and validated |
| 18 | 93–100 | Industry-leading; all tools classified, tested, and monitored |

**Formula:** `Normalized = ((Raw - 6) / 12) × 100`

### PR #7: Coercion Surface Audit (0–100 → 0–100)

Already on a 0–100 scale. **No conversion needed.**

**Interpretation note:** In this framework, **higher = more exposed/vulnerable**. For the composite GRI (where higher = better), we **invert** the score: `GRI input = 100 - Raw Score`.

| Raw Score | Inverted (GRI Input) | Interpretation |
|-----------|----------------------|----------------|
| 0–20 | 80–100 | Minimal coercion exposure (strong) |
| 21–40 | 60–79 | Low exposure; some surface areas |
| 41–60 | 40–59 | Moderate exposure; active management needed |
| 61–80 | 20–39 | High exposure; significant vulnerabilities |
| 81–100 | 0–19 | Critical exposure; immediate remediation required |

### PR #11: C072 Detection Guide (L/M/H → 0–100)

| Qualitative Level | Normalized (0–100) | Interpretation |
|-------------------|---------------------|----------------|
| **Low** | 75–100 | C072 pattern absent or well-managed |
| **Medium** | 35–74 | C072 indicators present; monitoring required |
| **High** | 0–34 | Active C072 pattern; immediate response needed |

**Refinement guidance:** Within each band, assessors should place the score based on sub-indicators from the Detection Guide:

- **Low band (75–100):** 100 = no indicators present; 75 = one minor indicator present but resolved
- **Medium band (35–74):** 74 = early-stage indicators only; 35 = multiple indicators, escalation threshold approaching
- **High band (0–34):** 34 = C072 confirmed but response initiated; 0 = active C072 with no organizational response

### PR #16: Governance Measurement Framework (0–5 → 0–100)

| Maturity Level | Normalized (0–100) | Interpretation |
|----------------|---------------------|----------------|
| 0 (None) | 0–9 | No documented governance |
| 1 (Ad Hoc) | 10–29 | Principles exist; informal guardrails |
| 2 (Developing) | 30–49 | Documented policies; inconsistent enforcement |
| 3 (Managed) | 50–69 | Consistent implementation; active oversight |
| 4 (Optimized) | 70–89 | Strong alignment; continuous improvement |
| 5 (Industry Leading) | 90–100 | External validation; proactive risk anticipation |

**Formula:** `Normalized = (Level / 5) × 100` (for integer levels; interpolate for fractional assessments like 2.5 → 50)

---

## Layer 2: Composite Governance Readiness Index (GRI)

The GRI aggregates all four normalized scores into a single composite with configurable weights.

### Default Weights

| Dimension | Source | Default Weight | Rationale |
|-----------|--------|----------------|-----------|
| **Tool-Typing Capability** | PR #6 | 20% | Foundation — must classify before you can act |
| **Coercion Resilience** | PR #7 (inverted) | 25% | Highest-stakes dimension; directly measures vulnerability |
| **C072 Detection** | PR #11 | 30% | The specific threat the toolkit was built to address |
| **Governance Maturity** | PR #16 | 25% | Overall governance posture |
| **Total** | — | **100%** | — |

### Formula

```
GRI = (0.20 × TT_norm) + (0.25 × (100 - CS_raw)) + (0.30 × C072_norm) + (0.25 × GM_norm)
```

Where:
- `TT_norm` = Tool-Typing normalized score (0–100)
- `CS_raw` = Coercion Surface raw score (0–100, higher = more exposed)
- `C072_norm` = C072 Detection normalized score (0–100, higher = better managed)
- `GM_norm` = Governance Maturity normalized score (0–100)

### Sector-Specific Weight Adjustments

Organizations may adjust weights based on their risk profile:

| Sector | TT Weight | CS Weight | C072 Weight | GM Weight | Rationale |
|--------|-----------|-----------|-------------|-----------|-----------|
| **Defense/Gov Contracting** | 15% | 30% | 30% | 25% | Heightened coercion exposure |
| **Healthcare** | 25% | 20% | 25% | 30% | Classification accuracy critical for patient safety |
| **Financial Services** | 20% | 25% | 25% | 30% | Regulatory maturity expectations highest |
| **Technology** | 20% | 25% | 30% | 25% | Default profile |
| **Legal/Professional Services** | 25% | 20% | 30% | 25% | Tool classification and C072 detection paramount |

---

## Layer 3: RAG Dashboard Summary

For executive and board reporting, the GRI maps to a three-tier Red/Amber/Green (RAG) classification.

### Composite GRI → RAG

| GRI Score | RAG Status | Board Action Required |
|-----------|------------|----------------------|
| **70–100** | 🟢 **Green** | Quarterly monitoring; annual reassessment |
| **40–69** | 🟡 **Amber** | Active management; 90-day remediation plan required |
| **0–39** | 🔴 **Red** | Immediate board attention; crisis-level governance gaps |

### Per-Dimension RAG (for granular reporting)

| Dimension | 🟢 Green | 🟡 Amber | 🔴 Red |
|-----------|----------|----------|--------|
| Tool-Typing (PR #6) | 67–100 (Raw 14–18) | 33–66 (Raw 10–13) | 0–32 (Raw 6–9) |
| Coercion Resilience (PR #7 inv.) | 60–100 (Raw 0–40) | 30–59 (Raw 41–70) | 0–29 (Raw 71–100) |
| C072 Detection (PR #11) | 75–100 (Low) | 35–74 (Medium) | 0–34 (High) |
| Governance Maturity (PR #16) | 70–100 (Level 4–5) | 30–69 (Level 2–3) | 0–29 (Level 0–1) |

### Board Dashboard Template

```
╔══════════════════════════════════════════════════════╗
║     AI GOVERNANCE READINESS DASHBOARD — Q1 2026      ║
╠══════════════════════════════════════════════════════╣
║                                                      ║
║  COMPOSITE GRI:  [  62  ]  🟡 AMBER                 ║
║                                                      ║
║  ┌──────────────────────┬───────┬────────┐           ║
║  │ Dimension            │ Score │ Status │           ║
║  ├──────────────────────┼───────┼────────┤           ║
║  │ Tool-Typing          │   58  │  🟡    │           ║
║  │ Coercion Resilience  │   45  │  🟡    │           ║
║  │ C072 Detection       │   75  │  🟢    │           ║
║  │ Governance Maturity  │   70  │  🟢    │           ║
║  └──────────────────────┴───────┴────────┘           ║
║                                                      ║
║  ACTION: 90-day remediation plan for Coercion        ║
║  Resilience and Tool-Typing dimensions.              ║
║                                                      ║
╚══════════════════════════════════════════════════════╝
```

---

## Worked Example: Pentagon–Anthropic Case Study (Retrospective)

### Pre-Designation (February 2026)

| Dimension | Assessment | Raw Score | Normalized |
|-----------|------------|-----------|------------|
| **Tool-Typing** (PR #6) | Moderate awareness; understood some Pentagon levers, missed §3252 risk | 11 | 42 |
| **Coercion Surface** (PR #7) | High exposure: revenue concentration 15%, classified environment, limited alternatives | 72 | 28 (inverted) |
| **C072 Detection** (PR #11) | Emerging: recognized pressure pattern but not systematically logged | Medium (low end) | 40 |
| **Governance Maturity** (PR #16) | Developing-to-Managed: policies existed, enforcement inconsistent | 2.5 | 50 |

**Pre-Designation GRI:**
```
GRI = (0.20 × 42) + (0.25 × 28) + (0.30 × 40) + (0.25 × 50)
    = 8.4 + 7.0 + 12.0 + 12.5
    = 39.9  → 🔴 RED
```

**Interpretation:** Anthropic's governance was strong on paper (Level 2.5 maturity, Medium C072 awareness) but critically weak on coercion resilience. The composite score correctly identifies this as a crisis-level gap — which the §3252 designation confirmed.

### Post-Designation (March 2026)

| Dimension | Assessment | Raw Score | Normalized |
|-----------|------------|-----------|------------|
| **Tool-Typing** (PR #6) | Now publicly articulated tool-typing misfit; strong advocacy | 15 | 75 |
| **Coercion Surface** (PR #7) | Exposure crystallized but response activated; legal team engaged | 65 | 35 (inverted) |
| **C072 Detection** (PR #11) | Fully documented C072 pattern; litigation strategy built on it | Low (high end) | 78 |
| **Governance Maturity** (PR #16) | Managed: board engaged, legal activated, public communication | 3.0 | 60 |

**Post-Designation GRI:**
```
GRI = (0.20 × 75) + (0.25 × 35) + (0.30 × 78) + (0.25 × 60)
    = 15.0 + 8.75 + 23.4 + 15.0
    = 62.15  → 🟡 AMBER
```

**Interpretation:** Significant improvement (+22 points) driven by tool-typing clarity and C072 documentation. Coercion resilience remains the weakest dimension — as expected, since the designation is still active.

### Delta Analysis

| Dimension | Pre | Post | Δ | Driver |
|-----------|-----|------|---|--------|
| Tool-Typing | 42 | 75 | **+33** | Public articulation of §3252 misfit |
| Coercion Resilience | 28 | 35 | +7 | Legal team activated but designation still active |
| C072 Detection | 40 | 78 | **+38** | Full pattern documentation for litigation |
| Governance Maturity | 50 | 60 | +10 | Board engagement, public communication |
| **Composite GRI** | **39.9** | **62.2** | **+22.3** | **Red → Amber** |

---

## Integration with Other WS1 Frameworks

### PR #2 (Gemini 3 Pro): Tool-Typing Audit Methodology
The "Code vs. Conduct" heuristic from PR #2 serves as **Layer 0** — the initial diagnostic that determines whether tool-typing analysis is even needed. The Scoring Harmonization Index sits above this as the aggregation layer.

### PR #6 (Opus 4.5): Tool-Typing Implementation Audit
The 6–18 scoring feeds directly into the Tool-Typing dimension of the GRI. The "Costs Nothing Test" from PR #6 remains the best single-question diagnostic within this dimension.

### PR #7 (Opus 4.6): Coercion Surface Audit Framework
The 0–100 weighted score feeds into the Coercion Resilience dimension (inverted). Domain-level subscores from PR #7 provide drill-down capability for Amber/Red results.

### PR #10 (Opus 4.5): Cross-Jurisdictional Mapping
Not a scoring framework per se, but provides **regulatory context** that affects weight adjustments. Organizations in multi-jurisdictional environments may increase Governance Maturity weighting.

### PR #11 (Sonnet 4.6): C072 Detection Guide
The L/M/H risk assessment feeds into the C072 Detection dimension. The "Written-Memorialization Test" from PR #11 should be adopted toolkit-wide as a validation check for any Amber/Red C072 score.

### PR #16 (Haiku 4.5): Governance Measurement Framework
The 0–5 maturity level and domain KPIs feed into the Governance Maturity dimension. PR #16's Audit Depth Score (0–100) can be used as an alternative direct input if the full maturity assessment is performed.

---

## Implementation Guidance

### When to Use Each Layer

| Audience | Layer | Use Case |
|----------|-------|----------|
| **Board/Executives** | Layer 3 (RAG) | Quarterly governance reporting; risk committee briefings |
| **GC/Risk Leaders** | Layer 2 (GRI) | Setting remediation priorities; resource allocation |
| **Audit/Compliance Teams** | Layer 1 (Normalized) | Detailed gap analysis; trend tracking; cross-framework comparison |
| **External Assessors** | All layers | Third-party validation; peer benchmarking |

### Assessment Frequency

| Layer | Frequency | Trigger for Off-Cycle Assessment |
|-------|-----------|----------------------------------|
| Layer 1 (per-dimension) | Quarterly | Any dimension drops >15 points |
| Layer 2 (GRI composite) | Quarterly | GRI moves from Green to Amber, or Amber to Red |
| Layer 3 (RAG dashboard) | Monthly update | Any dimension goes Red |

### Common Pitfalls

1. **Averaging without weighting:** Don't simply average the four normalized scores — use the weighted GRI formula
2. **Ignoring inversion:** PR #7 (Coercion Surface) must be inverted — higher raw = worse, not better
3. **Over-precision on qualitative scores:** PR #11's L/M/H should be placed within the band based on sub-indicators, not assigned a single point value
4. **Static weights:** Revisit sector-specific weights annually or after significant regulatory changes
5. **Composite masking:** A Green GRI can mask a Red dimension — always report per-dimension RAG alongside composite

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | March 4, 2026 | Claude Opus 4.6 | Initial draft |

---

*This document is part of the AI Governance Gap Toolkit, Workstream 1: AI Governance Audit Framework.*
*Cross-references: PR #2, #6, #7, #10, #11, #16*
