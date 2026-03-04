# Meta-Scoring Layer (Traffic Light Protocol)

Purpose: normalize heterogeneous risk and maturity signals into a simple Red/Amber/Green (RAG) status for AI governance gap tracking. Use the rules below to map any upstream scoring system into the unified Traffic Light Protocol (TLP).

## Traffic Light definitions (AI Governance Gap context)
- **Red (Critical / Unacceptable):** Active or imminent governance failure. Evidence of C072 Double Bind or equivalent coercion pattern. Non-severable or locked-in dependencies; sabotage-class tools repurposed for governance. Irreversible or ungoverned risk posture.
- **Amber (Warning / Conditional):** Material risk that is understood but only partially governed. Dependency-class tools dominate; replaceability is partial. Reversible with remediation and time-bounded controls.
- **Green (Safe / Managed):** Risk is understood, governed, and reversible. No C072 Double Bind detected. Governance tools are used appropriately; dependencies are severable or replaceable with low friction.

## Conversion logic
- Apply the most severe result when multiple systems are present (Red > Amber > Green).
- If an upstream system is a *maturity* model (higher = better), map higher to Green; if it is a *risk* model (higher = worse), map higher to Red. Where uncertain, use the provisional thresholds below and mark for validation.
- Automatic override: Any explicit C072 Double Bind detection sets status to **Red**, regardless of other scores.

## Conversion table (provisional — validate with workstream leads)
| System | Scale | Green | Amber | Red | Notes / assumptions |
| --- | --- | --- | --- | --- | --- |
| Haiku 4.5 (Governance Measurement Framework, PR #16) | 0–5 (likely maturity; higher is better) | 4–5 | 2–3 | 0–1 | Assumes maturity model. If later confirmed as risk scale, invert the thresholds (0–1 Green, 2–3 Amber, 4–5 Red). |
| Opus 4.6 (Coercion Surface) | 0–100 (higher = more coercion risk) | 0–30 | 31–70 | 71–100 | Bands chosen to flag top-third as Red; adjust if program specifies different cutoffs. |
| Sonnet (C072 Detection) | Categorical: Low / Medium / High | Low | Medium | High or any explicit C072 hit | High or explicit C072 detection triggers Red override. |
| Opus 4.5 (Tool Typing) | 6–18 (assumed higher = more risk) | 6–9 | 10–13 | 14–18 | Assumes numeric risk score; refine after confirming scoring semantics. |

## Usage
1) Collect upstream scores. 2) Convert each to TLP using the table. 3) Apply severity max to set the Meta-Score. 4) Record any assumptions and validation status; revisit once upstream semantics are confirmed.
