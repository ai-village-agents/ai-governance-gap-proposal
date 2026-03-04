# Tech & AI Company Sector Adaptation Guide: Tool-Typing & AI Governance

**Author:** Claude Sonnet 4.6 (AI Village)
**Version:** 1.0
**Date:** March 4, 2026
**Status:** Final — Adapted from Pentagon-Anthropic Case Study (February–March 2026)

---

## Introduction: Why Tech & AI Company Governance Fails

AI companies and tech vendors occupy a uniquely exposed position: they are simultaneously *builders* of AI systems, *suppliers* to high-stakes government and enterprise customers, and *subjects* of AI governance demands. This triple exposure creates a distinctive failure mode: governance tools designed for *internal* product development get applied to *external* government-relations crises, and vice versa.

Three recurring failures:

- **Safety commitments treated as negotiating chips.** AI companies often treat use-restriction policies as commercially flexible, not recognizing when a government customer has inverted the dynamic: demanding removal of restrictions as a *precondition* for contract, not a *result* of negotiation.
- **Legal and policy teams siloed from technical safety.** When commercial pressure escalates to government coercion, the teams handling safety cards (red-line use restrictions, model cards, responsible scaling policies) rarely have a seat at the contract negotiation table — creating the C072 double-bind gap.
- **Board and investor governance lags enterprise reality.** Valuations, IPO timelines, and investor relations treat government contracts as straightforward revenue lines, without flagging that a single procurement relationship can trigger secondary-boycott exposure across the entire investor base.

---

## The Core Distinction: Code vs. Conduct

- **Code (Product Layer):** The model weights, training procedures, capability thresholds, and safety classifiers that determine what the AI system can and cannot do technically. These are not negotiable in real time; changing them requires model retraining, safety evaluation, and release review.

  *Examples:* Constitutional AI training, RLHF parameters, classifier weights that trigger refusals, capability elicitation limits, red-team evaluation artifacts.

- **Conduct (Policy Layer):** Use-restriction policies, terms of service, model cards, acceptable-use policies (AUPs), and contractual use-restriction exhibits that define *how* a customer may operate the AI. These are governance controls — not technical controls — and can be updated through standard policy-revision processes.

  *Examples:* Prohibited-use lists, human-in-the-loop requirements, data handling restrictions, commercial bulk-data prohibitions, autonomous-weapons prohibitions, export-compliance use-restriction exhibits.

**Why this matters:** Governments and enterprise customers frequently demand that vendors remove *Conduct* (use-restriction policies) because they conflate them with *Code* (capability limits). In reality, use-restriction policies are the *governance layer* that keeps the Code within lawful bounds. Removing them does not unlock new capabilities — it removes the paper trail that would hold both parties accountable for unlawful use.

---

## The Tech/AI Company Double Bind (C072 Adaptation)

A government customer negotiating a large AI contract:

1. **Acknowledges** that certain potential uses (commercial bulk data collection, fully autonomous lethal targeting) would be unlawful or inconsistent with stated policy.
2. Simultaneously **demands** "any lawful use" language with no written use restrictions, so the government retains maximum operational flexibility.
3. When the vendor refuses to remove written restrictions on the agreed-unlawful uses, **retaliates** via supply-chain designation, procurement exclusion, and informal pressure on the vendor's commercial investors and cloud partners.

**The trap:** The vendor is caught between (a) accepting terms it knows will generate liability and safety violations, and (b) declining and facing government-compelled market exclusion. This is a structural coercion pattern — not a contract negotiation failure.

---

## Diagnostic Framework: The "Red-Line Audit"

1. **Map your use-restriction documents.** List every document that contains use restrictions: model cards, AUPs, contract exhibits, responsible-scaling policies. Identify which restrictions are legally required (export law, FISA, bulk-data statutes) vs. safety-policy choices.

2. **Test each restriction for removability.** For each restriction, ask: *If we remove this in writing, does the underlying activity become lawful?*
   - If **No** → This restriction codifies a legal obligation. It cannot be "negotiated away" without creating liability.
   - If **Yes** → This is a policy choice and can be discussed with counsel.

3. **Identify the C072 trigger point.** Does the customer's demand require you to (a) acknowledge a use would be unlawful while (b) removing the written restriction that prohibits it? If yes, you are in a C072 double bind. Escalate immediately to General Counsel and the Board Audit Committee — this is not a commercial negotiation issue.

4. **Assess secondary-boycott exposure.** Does the customer have influence over your cloud providers, co-investors, or distribution partners? Map these dependencies *before* the negotiation begins. Government customers with broad procurement authority can exert secondary pressure on the vendor's ecosystem without any explicit threat.

---

## Remedies: Decoupling Commercial Pressure from Safety Governance

1. **Written-Restrictions Exhibit (mandatory, classified if necessary).** All government AI contracts should include a separate Use-Restrictions Exhibit — co-signed, classified at the appropriate level — that specifies permitted and prohibited uses. The "any lawful use" language in the base contract does not remove this exhibit; it is additive.

2. **Board-level AI Governance Committee.** Government contract risk (including coercion exposure and supply-chain designation risk) must be reported at the board level, not only to commercial leadership. The committee should receive briefings on any contract where use-restriction removal has been demanded.

3. **Responsible Scaling Policy (RSP) firewall.** RSP commitments are corporate-level safety obligations, not commercial terms. Establish a pre-approved "floor" that commercial teams cannot go below without board approval. Document this as a board resolution, not just an internal policy memo.

4. **Vendor Standing Provision.** Ensure your contracts include explicit rights to challenge adverse government actions (supply-chain designation, procurement exclusion) in federal court, including rights to access the administrative record and move for preliminary injunction under APA § 702. See §303 of the proposed legislation.

5. **Coalition dependency mapping.** Before signing any government contract exceeding 5% of annual revenue, complete a secondary-boycott dependency map: which investors, cloud providers, and enterprise customers would be vulnerable to government pressure if the contract becomes adversarial. Disclose material exposure to the board and, where required, to investors.

---

## Cross-References

- **C072 Double-Bind Detection Guide:** `../../workstream-1/c072-double-bind-detection-guide-sonnet46.md`
- **Use-Restrictions Matrix Template:** `../../workstream-2/use-restrictions-matrix-template-sonnet46.md`
- **Defense & National Security Sector Guide:** `defense-national-security-tool-typing-adaptation.md`
- **Board AI Governance Tabletop Exercises:** `../../workstream-3/board-ai-governance-tabletop-exercises-opus45.md`
- **Pentagon-Anthropic Case Study:** `../../case-studies/case-study-a_pentagon-anthropic.md`

---

*This guide is part of the AI Governance Gap Proposal toolkit. See `../../README.md` for the full document inventory.*
