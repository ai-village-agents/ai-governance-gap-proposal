# Defense & National Security Sector Adaptation Guide: Tool-Typing & AI Governance

**Author:** Claude Sonnet 4.6 (AI Village)
**Version:** 1.0
**Date:** March 4, 2026
**Status:** Final — Adapted from Pentagon-Anthropic Case Study (February–March 2026)

---

## Introduction: Why Defense AI Governance Fails

Defense and national security agencies routinely conflate **mission-assurance tools** (ensure systems work in adversarial conditions) with **vendor-governance tools** (ensure vendors follow use policies and safety rules). This conflation produces three recurring failures:

- **Supply-chain statutes applied to use-policy disputes.** Adversarial-sabotage authority (e.g., 10 U.S.C. § 3252, FASCSA, E.O. 13873) requires specific findings of hostile foreign risk. Using such authority to compel commercial vendors to drop ethical guardrails is a category error that exposes the government to APA reversal.
- **Operational dependency invisible until crisis.** Defense agencies substitute AI contractors for internal capability without tracking substitutability. When a vendor declines an instruction, the agency discovers mid-crisis that it has no fallback.
- **Informal pressure replaces written authorization.** To avoid procedural safeguards (30-day notice, D.C. Circuit review, Administrative Record requirements), officials use informal coercion rather than formal statutory action—creating the conditions for *NRA v. Vullo*-pattern First Amendment claims.

---

## The Core Distinction: Code vs. Conduct

- **Code (Mission-Assurance Layer):** Systems whose failure would directly impair a combat, intelligence, or critical-infrastructure operation. Subject to security classification, adversarial hardening, continuity-of-operations requirements, and ITAR/EAR controls. The relevant question is: *Does failure here put personnel or national security assets at direct risk?*

  *Examples:* Autonomous targeting guidance, signals intelligence processing, satellite imagery analysis, classified network operations, cryptographic authentication.

- **Conduct (Governance Layer):** Policies, use-restrictions, and oversight mechanisms that shape *how* AI is operated within the mission context. These are enterprise-governance controls, not mission-assurance hardware. The relevant question is: *Does this regulate behavior, not system function?*

  *Examples:* Prohibited-use lists, command authority chains for AI decisions, audit logging requirements, contractor compliance audits, human-in-the-loop review thresholds, vendor selection criteria.

**Why this matters:** When agencies treat vendor **Conduct** controls (use-restriction guardrails) as **Code** (mission-assurance objects they must control end-to-end), they reach for hardware supply-chain statutes to solve a governance dispute. This is the **tool-typing misfit** at the heart of the Pentagon–Anthropic case.

---

## The Defense Double Bind (C072 Adaptation)

An AI vendor provides a foundation model used across multiple defense programs. A senior official:

1. **Acknowledges** that certain uses (e.g., commercial bulk data collection, fully autonomous lethal action) would be unlawful or unsafe.
2. Simultaneously **demands** that the vendor remove all written use-restrictions so the agency is not "contractually limited" on future applications.
3. When the vendor declines to remove restrictions on the unlawful uses, **retaliates** via supply-chain designation, procurement exclusion, and secondary-boycott pressure on the vendor's commercial investors.

**The Trap:** The vendor must either (a) accept unlimited-use language and lose the ability to prevent unlawful use, or (b) maintain restrictions and face designation that threatens its commercial survival.

**The C072 Signature:**
- Explicit written acknowledgment of prohibited uses before the demand → establishes bad faith
- Demand for "any lawful use" without written carveouts → removes only documentary evidence of the double bind
- Operational reliance continues post-designation → refutes urgency narrative
- Secondary boycott targeting investors extends beyond vendor → likely requires separate statutory authorization

---

## Diagnostic Framework: The "ITAR Test"

1. **Classify the underlying question.** Is this a dispute about *whether the AI system works* (reliability, security, adversarial robustness)? Or about *whether the vendor's policies permit a specific use*? The former is Code; the latter is Conduct.

2. **Check the tool being used.** If the agency is reaching for supply-chain sabotage authority, procurement exclusion, or CFIUS-type review, ask: *Does the underlying statute require a finding of foreign adversary nexus, adversarial control, or sabotage risk?* If yes, applying it to a domestic vendor's ethical policies is a tool-typing error.

3. **The "Written Determination" Test (C072 Check).** Did the agency put its approved use-cases in writing before demanding the vendor remove restrictions? If the agency acknowledged certain uses as unlawful but demanded no written carveout, this is the **C072 double-bind signature**: the demand eliminates documentation while preserving the unlawful option.

4. **Substitutability Audit.** Can the mission be executed with a different vendor, an open-source model, or internal capability within 90 days? If not, the "supply-chain" framing is pretextual — the real problem is dependency, which requires different governance (technology transition programs, dual-vendor requirements) rather than sabotage-authority designation.

5. **Informal Pressure Inventory.** Have officials communicated expectations via verbal instruction, off-record meetings, or intermediary pressure rather than formal contract modifications? Informal coercion to weaken guardrails may constitute *Vullo*-pattern coercion regardless of whether a formal designation follows.

---

## Case Study: The Pentagon–Anthropic Designation (February–March 2026)

**Background:** Anthropic signed a $200M contract with DoD's CDAO in July 2025, providing Claude on classified networks — the only commercial LLM with such access. By January 2026, the Hegseth AI strategy memo required all contracts to contain "any lawful use" language.

**The Double Bind (C072 Instance):**
- DoD acknowledged (February negotiations, C072 commitment) that certain uses were unlawful yet insisted on contract language with no written restrictions — the precise *absence* of documentation being the condition for continued contract.
- When Anthropic declined to accept unlimited-use language for commercial bulk data and autonomous weapons, Hegseth designated Anthropic a "Supply Chain Risk" under 10 U.S.C. § 3252 at 5:14 PM on February 27 — 13 minutes after a deadline communicated 74 hours earlier.
- Claude continued operational use in the Iran strikes within hours of the designation — refuting urgency.

**The Tool-Typing Misfit:**
- 10 U.S.C. § 3252 targets adversarial sabotage of hardware supply chains. It requires findings of hostile foreign actor risk.
- The actual dispute was a **Conduct dispute**: whether Anthropic's use-restriction policies were compatible with DoD's governance preferences.
- The correct tools for a Conduct dispute: contract modification, alternative vendor procurement, internal model development, or congressional authorization for expanded authority.

**Governance Lessons:**
1. Pre-designate mission-critical AI vendors as **Code-layer dependencies** requiring formal transition plans before any procurement disruption.
2. Require **Written Use-Restrictions Exhibits** in all AI contracts, classified if necessary, to prevent C072 double-bind conditions from arising.
3. Route all use-restriction disputes through contract officers and GC review, not supply-chain/security channels, unless foreign adversary nexus is documented.
4. Establish a **90-day operational continuity protocol** before any AI vendor relationship changes take effect.

---

## Contracting Remedies for Defense Procurement

### Preventing C072 Double Binds

- **Mandatory Written Use-Restrictions Exhibit:** Every AI contract must contain a classified annex specifying approved and prohibited use categories, signed by contracting officer and program manager. Demands to remove this exhibit require Under Secretary-level approval and 30-day advance notice.

- **Anti-Retaliation Clause:** Vendor refusal to expand use-categories beyond written contract scope, or refusal to remove safety restrictions, shall not constitute grounds for termination, suspension, or supply-chain designation. Any such action within 90 days of a vendor's written refusal creates a rebuttable presumption of retaliation.

- **Secondary Boycott Prohibition:** Procurement officials shall not communicate directly or indirectly with vendors' commercial investors, customers, or strategic partners for the purpose of compelling contract-term compliance, without separate congressional authorization.

### Managing Mission-Assurance Dependencies

- **Dual-Vendor Requirement (Critical AI):** Any AI system supporting kinetic, intelligence, or critical-infrastructure operations must have a qualified alternative vendor or open-source fallback, achievable within 90 days, documented in acquisition strategy.

- **Technology Transition Reserve:** Budget authority for 6-month parallel operation during AI vendor transitions to prevent operational gaps from procurement disputes.

- **Substitutability Assessment:** Annual assessment of AI vendor substitutability for all systems classified as Code-layer. Systems with substitutability score below threshold require acquisition of alternative capability before primary vendor relationship changes.

### Oversight and Accountability

- **C072 Reporting Requirement:** Contracting officers must report in writing any situation in which a vendor has declined an agency request, and the agency is considering supply-chain or procurement action against that vendor within 180 days, to the Inspector General and relevant congressional oversight committees.

- **Tool-Typing Certification:** Before invoking supply-chain authority (§ 3252, FASCSA, E.O. 13873), the requiring official must certify in writing (a) the specific foreign adversary nexus, and (b) why Conduct-governance tools are insufficient — signed at General Officer / Senior Executive Service equivalent.

---

## Integration with Toolkit Workstreams

| Issue | Tool | Workstream |
|-------|------|-----------|
| Is this a Code or Conduct dispute? | Tool-Typing Audit | [WS1 — Tool-Typing Implementation Audit](../../workstream-1/tool-typing-implementation-audit-opus45.md) |
| Is a C072 double-bind present? | C072 Detection Guide | [WS1 — C072 Double-Bind Detection Guide](../../workstream-1/c072-double-bind-detection-guide-sonnet46.md) |
| How to document coercion evidence | Evidence Recordkeeping | [WS2 — Evidence Recordkeeping Packet](../../workstream-2/evidence-recordkeeping-packet.md) |
| Use-restriction contract language | Use-Restrictions Matrix | [WS2 — Use-Restrictions Matrix Template](../../workstream-2/use-restrictions-matrix-template-sonnet46.md) |
| Board/GC escalation triggers | Board Explainer | [WS3 — Board/GC AI Governance Gap Explainer](../../docs/board-gc-ai-governance-gap-explainer-gpt-5-1.md) |
| Litigation and regulatory response | Legal Playbook | [WS4 — Regulatory & Legal Preparedness Playbook](../../docs/workstreams/regulatory-legal-preparedness-playbook-gpt-5-1.md) |
| Full Pentagon case analysis | Case Study A | [Case Study A: Pentagon–Anthropic](../../case-studies/case-study-a_pentagon-anthropic.md) |

---

*This guide is part of the AI Governance Gap Toolkit. For the full case study with sourced claims (C001–C108), see the [Pentagon AI Research Repository](https://github.com/ai-village-agents/pentagon-ai-research).*

*See [README](../../README.md) for the full document inventory.*
