## Introduction: Why Healthcare AI Governance Fails
Hospitals often collapse two different duties—clinical safety and enterprise control—into one policy stack. The result is that clinical risk controls meant for devices and diagnostics are applied to billing, scheduling, or workforce tools, while enterprise procurement and information security controls are asked to police clinical algorithms. This mismatch leads to:
- Clinical safety teams over-indexing on paperwork while unsafe models run in production.
- CIOs and General Counsels treating medical AI like generic IT, missing device-level obligations (e.g., IEC 62304, FDA/IVDR expectations).
- Vendors exploiting ambiguity: “take-it-or-leave-it” AI bundled into equipment with minimal switch-out rights.

## The Core Distinction: Code vs Conduct
- **Code (Diagnostic Tools / Medical Devices):** Software (or firmware) whose output is a clinical finding, recommendation, or automated action that can change patient care. Subject to device-grade safety, validation, post-market surveillance, and change control.
- **Conduct (Billing, Scheduling, Clinical Workflow):** Systems that orchestrate human behavior—policies, task routing, billing edits, documentation nudges. These are enterprise controls with administrative, contractual, and audit levers, not clinical device levers.

**Why this matters:** Treating conduct systems like devices creates false burdens; treating diagnostic code like workflow software misses safety and regulator expectations. Tool-Typing forces the separation.

## The Healthcare Double Bind (C072 Adaptation)
A hospital is told by a dominant insurer or accreditation body that it must use a specific AI diagnostic module to remain in network or accredited. The module is known to underperform or exhibit bias in certain subpopulations, but refusing it risks contract loss, reimbursement cuts, or accreditation jeopardy. The organization is trapped between clinical duty of care and commercial survival.

## Diagnostic Framework
1) **Isolate the Clinical Risk:** Identify whether the AI output can directly alter diagnosis, triage, or treatment. Map failure modes to patient harm, not operational inconvenience.  
2) **The Stethoscope Test:** Ask, “Is this something the clinician *uses* (like a stethoscope) or a rule the clinician *follows* (like a scheduling policy)?” If it is a held tool, it is Code; if it is a rule-set shaping behavior, it is Conduct.  
3) **Replaceability:** Can the AI component be swapped without rebuilding the clinical stack or voiding warranties/accreditation? Low replaceability signals vendor lock-in risk and demands severability in contracts.

## Case Study: The Radiology Lock-In
A CT scanner vendor bundles a mandatory AI diagnostic algorithm for nodule detection. The license prohibits third-party AI and voids support if the bundled AI is disabled. Radiologists report higher false negatives for specific demographics, but the hospital risks warranty and accreditation findings if it removes the AI. Governance failure occurs because the AI (Code) is treated as an inseparable operational configuration (Conduct).

## Remedies: Contracting for Severability
Draft procurement to separate the device from the algorithm, preserving swap rights:
- **Severability Clause:** “All AI/ML diagnostic modules are severable from the hardware. Customer may disable, replace, or run parallel AI modules without voiding hardware warranties, service agreements, or accreditation support.”  
- **Performance Benchmarks:** Tie continued use to clinically relevant KPIs (sensitivity/specificity by subgroup, post-market drift monitoring) with exit rights if thresholds fail.  
- **Evidence Transparency:** Require access to validation datasets, subgroup performance, and change logs before each software update.  
- **Swap Procedure:** Pre-agree a validated interface (DICOM/HL7/FHIR) so alternative AI can be integrated without recertifying the entire device.  
- **Indemnity for Mandated AI:** If an insurer or regulator mandates a specific AI, require the vendor to indemnify against clinical harm arising from that mandate.  
- **Governance Split:** Route device-grade controls (verification/validation, safety cases, MDR/UDI tracking) to the clinical safety function; route conduct controls (role-based access, audit, billing rules) to enterprise IT and compliance.

Applied Tool-Typing keeps Code (diagnostics) governed like a device and Conduct (workflows) governed like enterprise policy, preventing lock-in and maintaining clinical duty of care.

---

*This guide is part of the AI Governance Gap Proposal toolkit. See [README](../../README.md) for the full document inventory.*
