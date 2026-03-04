# Factuality and Sourcing Policy

Boilerplate for authors (paste near the top of docs):

> This document follows the project factuality policy: content is labeled at the smallest practical unit (section, paragraph, or bullet), sources are cited, and teaching simulations are clearly marked as fictionalized.

See also: WS2 guardrail policy template (`workstream-2/model-ai-guardrail-policy-template.md`, PR #20), WS2 use-restrictions matrix template (`workstream-2/use-restrictions-matrix-template-sonnet46.md`, PR #25), and Case Study A guidance (PR #17).

## Classification of Statements
- **Verified:** Supported by cited primary sources or direct records.
- **Attributed:** Cited to a secondary source; accuracy depends on that source.
- **Analysis:** Reasoned interpretation or inference; not a factual assertion.
- **Hypothetical:** Scenario that may or may not occur; clearly contingent.
- **Teaching Simulation:** Fictionalized, claims-based scenario used for instruction.

Label at the smallest practical unit (section, paragraph, or bullet) so readers can tell where Verified or Attributed facts end and Analysis, Hypothetical, or Teaching Simulation content begins. Mixed sections are acceptable when subheadings or callouts keep the categories distinct.

## Minimum Sourcing Rules
- Prefer primary sources (official releases, filings, transcripts). If secondary sources are used, cite them.
- Do not include unsourced factual assertions about real people or organizations.
- Date-stamp news or time-sensitive claims (e.g., “As of 2024-03-15...”).
- Quote sparingly and paraphrase accurately; avoid copy-paste of large passages.
- When using aggregated data, note the dataset name, publisher, and collection date.

## Guidance for Using “Case Study A”
- Clearly label as **Teaching Simulation** at first mention and in any headers.
- Avoid naming real companies or governments unless the section is strictly about public record facts and includes citations.
- Keep fictional elements distinct from cited facts; do not blend them in the same sentence.
- If a real-world event inspires the scenario, state that the scenario is fictionalized and not a claim about actual conduct.

## Guidance for Internal Claim IDs
- Claim IDs (if used) are internal to this project and do not imply external validation or endorsement.
- When present, include a brief note such as “Claim IDs are internal tracking labels, not third-party ratings.”

## Naming Note
- The phrase “Traffic Light Protocol (TLP)” can be confused with the established TLP standard; prefer neutral terms like “RAG sensitivity tags” or “handling levels” unless you are intentionally implementing that standard.

## Checklist
- Label content at the smallest practical unit (section, paragraph, or bullet) to separate Verified/Attributed facts from Analysis/Hypothetical/Teaching Simulation material; use subheadings for mixed sections.
- Cite primary sources where available; cite secondary sources otherwise.
- No unsourced factual claims about real people or organizations.
- Date-stamp time-sensitive statements.
- Teaching Simulation sections are clearly marked; fictional content is separated from facts.
- Any internal claim IDs are explained as project-only.

---

*This policy is part of the AI Governance Gap Proposal toolkit. See [README](../../README.md) for the full document inventory.*
