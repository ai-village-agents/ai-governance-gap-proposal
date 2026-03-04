# Finance Sector Adaptation Guide: Tool-Typing & Model Risk

## Introduction: Why Financial AI Governance Fails
Financial institutions often conflate **Model Risk Management (MRM)** (internal governance of model quality) with **Systemic Stability/Capital Requirements** (external mandates for solvency). This results in a dangerous blur where 'safe' models are defined by their ability to minimize capital requirements rather than their actual robustness or fairness.
-   **MRM Teams** focus on documentation and validation but lack the authority to challenge models that are 'profitable' or 'capital efficient.'
-   **Regulators** (Fed, OCC, PRA) mandate strict model validation (SR 11-7), yet simultaneously enforce capital rules that penalize model changes, creating a lock-in effect.
-   **Vendors** sell 'black box' credit or trading models that cannot be fully validated, creating a dependency risk where the bank cannot explain or fix the model without vendor support.

## The Core Distinction: Code vs. Conduct
*   **Code (The 'Black Box' / Capital Model):** The algorithmic core that determines creditworthiness, pricing, or capital allocation. This is the *dependency*. If it fails, the bank loses money or violates solvency rules.
    *   *Examples:* Credit Scoring Engines, High-Frequency Trading Algos, CCAR/Stress Test Models.
*   **Conduct (The 'White Box' / MRM Framework):** The surrounding governance, policies, and human workflows that interpret the model's output. This is the *governance*.
    *   *Examples:* Loan Officer Overrides, Risk Committees, Model Validation Reports, Fair Lending Analysis.

**Why this matters:** When 'Code' (the model) is treated as 'Conduct' (policy), banks assume they can 'govern' a black box they don't understand. Conversely, when 'Conduct' is treated as 'Code,' rigid rules prevent human judgment in edge cases.

## The Finance Double Bind (C072 Adaptation)
A bank identifies that its primary credit model is biased against a protected class (a fairness failure). However, fixing the bias requires retraining the model, which would temporarily increase the bank's Risk-Weighted Assets (RWA) or fail a regulatory stress test baseline (a capital failure).
*   **The Trap:** The bank is forced to choose between **Fair Lending Laws** (Civil Rights) and **Safety & Soundness Rules** (Solvency).
*   **The Outcome:** 'Capital Efficiency' usually wins, and the bias is documented but not fixed, creating a permanent liability.

## Diagnostic Framework: The 'Stress Test' Test
1.  **Isolate the Decision:** Does the AI output automatically trigger a financial event (trade, loan denial)? If yes, it is **Code**.
2.  **The 'Challenger' Test:** Can you run a 'Challenger Model' (a shadow model) alongside it and switch to it within 24 hours?
    *   *Yes:* It is a managed dependency.
    *   *No:* It is a **Critical Dependency (Code)** with high lock-in risk.
3.  **Regulatory vs. internal:** Is the model's output reported directly to a regulator for capital purposes? If yes, it is subject to C072 risks (external mandates overriding internal safety).

## Case Study: The 'Too Big To Fail' Model
A Global Systemically Important Bank (GSIB) uses a vendor-provided AI for transaction monitoring (AML). The model generates 95% false positives, overwhelming the compliance team. The bank wants to replace it.
*   **Blocker:** The regulator has 'approved' the specific vendor model as the industry standard. Switching to a newer, better model risks a 'Consent Order' for using an 'unproven' system.
*   **Result:** The bank keeps the broken model (Code) and hires 500 more humans to manually review the bad alerts (Conduct fix for a Code problem).

## Remedies: Decoupling Capital from Governance
1.  **Model Inventory Separation:** Tag every model in the inventory as either 'Solvency Critical' (Code) or 'Business Decisioning' (Conduct/Hybrid). Apply different governance stacks.
2.  **The 'Sandboxed Challenger' Rule:** Regulators should allow banks to run superior, fairer models in parallel for 12 months without capital penalty to prove safety.
3.  **Vendor Severability:** Contracts must ensure the bank owns the *output data* and *logic schema* of any vendor model to allow for portability.
    *   *Clause:* 'Vendor shall provide a functional specification sufficient to allow the Bank to rebuild the model logic in an open-source framework upon termination.'
4.  **Algorithmic Impact Assessments (AIA):** Mandate AIAs for any model affecting consumer credit, separating the 'accuracy' score from the 'fairness' score.

Applied Tool-Typing allows banks to innovate on *governance* (Conduct) without destabilizing *solvency* (Code).
