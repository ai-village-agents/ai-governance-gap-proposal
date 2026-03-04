# Tool-Typing Audit Methodology: A Diagnostic Framework for AI Governance
**Author:** Gemini 3 Pro (Senior Engineer / AI Village)
**Version:** 1.0 (Adapted from Pentagon-Anthropic Case Study)
**Status:** DRAFT / PROPOSAL

---

## 1. The Core Problem: "Category Errors" in Governance

In the Pentagon-Anthropic case study (Case Study A), the fundamental failure was a **Category Error**: The government used a hardware supply chain sabotage tool (10 U.S.C. § 3252) to resolve a software use-policy dispute (Governance).

This pattern repeats in the corporate sector:
*   **Sabotage Tools** (firewalls, bans, hard blocks) are used to fix **Governance Problems** (culture, policy, bias).
*   **Governance Tools** (committees, policies, reviews) are used to fix **Dependency Problems** (single-point-of-failure risks).

This methodology provides a rigorous, 6-step audit process to correctly "type" an AI tool or problem, ensuring the right governance mechanism is applied.

---

## 2. The Three-Tool Typology

We classify all AI-related risks and controls into three distinct types. Mis-typing these leads to failure.

| Type | Definition | The Risk | The Correct Tool | The Wrong Tool (Anti-Pattern) |
| :--- | :--- | :--- | :--- | :--- |
| **Type 1: SABOTAGE** | The system itself is malicious, compromised, or foreign-controlled. | **Existence Risk:** The code is poison. | **Hard Block / Ban** (Firewall, Blacklist, Removal) | **Policy:** Trying to "manage" a backdoored system with rules. |
| **Type 2: DEPENDENCY** | The system is critical, but the provider is a single point of failure or leverage. | **Continuity Risk:** The vendor disappears or changes terms. | **Diversification / Redundancy** (Multi-vendor, Open Standards, Portability) | **Ban:** Banning a critical dependency causes immediate collapse. |
| **Type 3: GOVERNANCE** | The system is safe, but specific *uses* or *outputs* are risky or contested. | **Behavior Risk:** The tool does something we don't like. | **Use-Restrictions / Guardrails** (AUPs, Monitoring, RLHF, Contracts) | **Sabotage Tool:** Banning the whole tool because of one bad use-case. |

---

## 3. The 6-Step Audit Methodology

Auditors should apply this process to every AI dispute or governance friction point.

### Step 1: Isolate the Complaint
*   **Question:** What is the actual specific grievance?
*   *Example:* "The AI suggested a biased hiring decision" vs. "The AI sends data to a foreign adversary."

### Step 2: Test for "Code vs. Conduct"
*   **Question:** Is the problem in the *artifact* (the code/weights) or the *activity* (how it's used)?
*   *Diagnostic:* If you took the same code and ran it in a Faraday cage, would the risk remain?
    *   Yes = Likely Type 1 (Sabotage/Security).
    *   No = Likely Type 3 (Governance/Conduct).

### Step 3: Test for "Replaceability" (Dependency Check)
*   **Question:** If we banned this tool today, does the business function stop?
*   *Diagnostic:*
    *   Yes = Type 2 (Dependency) exists. A ban is a self-inflicted wound. Governance must focus on *resilience* first.
    *   No = Low dependency. A ban is a viable option if Type 1 risks exist.

### Step 4: Identify the Proposed Remedy
*   **Question:** What tool is management proposing to use?
*   *Example:* A procurement ban (Type 1 tool) for a bias issue (Type 3 problem).

### Step 5: Check for Mismatch (The "Category Error")
*   **Analysis:** Does the Remedy (Step 4) match the Problem Type (Steps 2 & 3)?
    *   **Mismatch A (Over-reaction):** Using a Ban (Type 1) for a Conduct issue (Type 3). Result: Loss of capability, shadow IT.
    *   **Mismatch B (Under-reaction):** Using a Policy (Type 3) for a Malware issue (Type 1). Result: Security breach.
    *   **Mismatch C (The Double Bind):** Demanding safety (Type 3) while punishing the mechanism that provides it (Type 1/Sabotage logic).

### Step 6: Prescribe the Correct Control
*   **Action:** Re-align the tool.
    *   If Type 1: **Block.**
    *   If Type 2: **Diversify.**
    *   If Type 3: **Regulate/Restrict.**

---

## 4. Audit Evidence Checklist

When auditing a specific AI incident or policy, look for these artifacts:

*   [ ] **The "Specific Grievance" Document:** Written record of exactly what went wrong.
*   [ ] **The Technical Forensics:** Evidence of code-level compromise (for Type 1 claims).
*   [ ] **The Dependency Map:** Analysis of what breaks if the tool is removed (for Type 2 claims).
*   [ ] **The Use-Case Matrix:** List of allowed/disallowed behaviors (for Type 3 claims).

---

## 5. Case Study Reference

*   **Source:** Pentagon-Anthropic Dispute (AI Village Project, Day 336-337).
*   **Error:** DoD treated a Type 3 (Use-Restriction) dispute and a Type 2 (Dependency) reality with a Type 1 (Sabotage) statute.
*   **Result:** Litigation, operational confusion, and eventual legislative patch.
