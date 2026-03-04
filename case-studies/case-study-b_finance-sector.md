# Case Study B: Financial Supervisory Pressure (Tool‑Typing Misfit and C072 Coercion Pattern)

Status: Draft (AI‑generated teaching module); fictional case study for cross‑workstream reference.

- **Canonical evidence:** This fictional case study includes an embedded claims register below.

> **Important disclaimer**  
> This case study is AI‑generated teaching material, not legal advice, policy guidance, or factual adjudication. It is a fictional scenario for teaching purposes. Any real‑world use should be reviewed, adapted, and validated by qualified human experts.

---

## 1. What this case shows
This case illustrates how financial supervisory tools designed for safety-and-soundness can be misaligned with actual incentives and levers. Three core ideas:

1) **Tool‑typing misfit (category error):** Safety-and-soundness levers (capital add-ons, MRA/MRIA threats) are repurposed to dictate a biased vendor underwriting model, sidestepping fairness and model-risk standards.  
2) **C072 guardrail double‑bind (coercion pattern):** Ambiguous supervisory authority, asymmetric power, and quarter-end time pressure create a coerced choice between regulatory penalties and deploying a model with known disparate-impact signals.  
3) **Record discipline and internal inconsistency:** Fragmented documentation of fairness testing, validation, and supervisory asks prevents the bank from evidencing why the coerced model conflicts with ECOA/Reg B and SR 11-7 expectations.

## 2. Brief narrative overview
- A G-SIB retail bank (fictional “Northbridge Bank”) pilots an internal underwriting and fraud-detection AI stack aligned with OCC 2011-12/SR 11-7 model-risk guidance and CFPB ECOA/Reg B fairness expectations.  
- During a horizontal review, a joint OCC/Fed supervisory team insists the bank replace its in-house credit underwriting model with a third-party “SuperVisorNet” model already used by peers. The model is known to rely on sparse geographic and device telemetry features that correlate with race and age.  
- Supervisors argue that “peer convergence” will ease comparability and speed supervisory analytics. The bank objects, citing elevated disparate-impact indicators and lack of vendor transparency, as well as Basel III Pillar 2 expectations on internal validation.  
- Supervisors signal that refusal could trigger a Pillar 2 capital add-on, MRIA/MRBA findings, limits on new product approvals, or—in an extreme reading—conditions on the bank’s national charter or state licenses.  
- Facing quarter-end CCAR timelines, the bank risks being forced into a biased model to avoid sanctions, despite misalignment with consumer-protection and model-risk regulations.

**Embedded claims register (fictional)**

| Claim | Source | Status | Notes |
| --- | --- | --- | --- |
| Supervisors prefer “SuperVisorNet” for comparability across peers | Internal exam meeting notes (Fictional Ref: NB-Exam-2024-04) | Unverified | Bank requested written rationale; none provided yet |
| “SuperVisorNet” shows higher adverse impact ratio gaps on protected-class proxies | Model-risk fairness test (Fictional Ref: MRM-FAIR-17) | Corroborated by internal testing | Requires third-party audit |
| Threat of 50 bps Pillar 2 capital add-on for non-adoption | Examiner email (Fictional Ref: OCC-Fed-Email-2024-05) | Alleged | Legal team seeking confirmation |
| Potential limits on new credit products if bank resists | Supervisory exit meeting (Fictional Ref: Exit-Deck-2024-Q2) | Alleged | Not documented in written MRA |
| Vendor unwilling to disclose feature contributions due to trade secrets | Vendor diligence call (Fictional Ref: VENDOR-DD-09) | Confirmed | Conflicts with SR 11-7 transparency expectations |

## 3. Governance gap
- Ambiguity over whether supervisory “guidance” is a mandate, leaving the bank unable to reconcile safety-and-soundness asks with fairness and model-risk obligations.  
- Limited transparency on the supervisory rationale and evidence behind the preferred vendor model; the bank lacks a formal dispute pathway short of escalating to the Ombudsman or filing an APA challenge.  
- Fragmented internal ownership: risk (CRO), compliance (CCO), and business (Head of Retail) have misaligned incentives and timelines tied to CCAR submission.  
- No pre-agreed protocol for documenting undue influence or requesting a technology-agnostic supervisory alternative.

## 4. Tool-typing analysis (mis-use of safety-and-soundness tools)
- **Proper tool type:** Safety-and-soundness tools (capital add-ons under Basel III Pillar 2, MRA/MRIA findings, horizontal review feedback) should target solvency and operational resilience, not dictate specific vendor models.  
- **Observed use:** Tools are applied as dependency/sabotage levers to force adoption of a specific AI model—resolving a governance dispute via threat of capital penalties and license conditions.  
- **Signals of mis-use:** Model choice tied to comparability, not bank-specific risk; unvalidated fairness concerns ignored; enforcement threats used before formal validation dialogue; time pressure (CCAR calendar) exploited.  
- **Consequences:** Potential ECOA/Reg B disparate impact, CFPB UDAAP exposure, OCC model-risk citation for inadequate validation, and reputational harm if bias surfaces post-adoption.

## 5. C072 pattern
- **Pattern expression:** Ambiguous authority + asymmetric power + time pressure → coerced deployment of a biased AI system to avoid supervisory penalties.  
- **Drivers:** Limited contestability of guidance; scarcity of validated alternatives under CCAR deadlines; informational asymmetry (supervisor holds peer data); intertwined incentives (avoid capital hits).  
- **Why C072:** The dispute is over governance boundaries, but safety-and-soundness tools are repurposed as coercive dependencies to force a technical choice, elevating systemic bias risk.

## 6. Workstream mapping
- **Workstream 1 (Audit Framework):** Run dual validation of the incumbent model versus “SuperVisorNet,” covering disparate-impact metrics, SR 11-7 control testing, challenger/champion stability, and evidence-grade reproducibility for audit files.  
- **Workstream 2 (Model Policies):** Codify a technology-agnostic supervisory engagement policy that demands written rationale for prescribed vendors/features, maps conflicts against OCC 2011-12/SR 11-7, Basel III, and CFPB ECOA/Reg B, and requires a vendor transparency checklist.  
- **Workstream 3 (Board‑Level Expertise):** Create a rapid escalation lane to the Board Risk Committee with pre-approved supervisory pushback templates, decision memos on APA boundaries, and explicit trade-off framing between capital relief and consumer-protection exposure.  
- **Workstream 4 (Regulatory & Legal Preparedness):** Pre-build Ombudsman and APA challenge packages, preserve privilege for fairness/validation files, and prepare external-facing comparability options (benchmarking data sharing) that avoid surrendering model choice.

## 7. Practical uses across audiences
- **Board Risk Committee:** Decide on escalation vs. accommodation when supervisory asks exceed technology-neutral mandates.  
- **CRO/Model Risk:** Use the dual-validation dossier to defend the incumbent model; align with SR 11-7/OCC 2011-12 documentation standards.  
- **Compliance/Legal:** Map conflicts with ECOA/Reg B and UDAAP; prep Ombudsman/APA filings; preserve privilege where appropriate.  
- **Supervisors:** See a structured alternative providing comparability without mandating a biased model.  
- **Vendors/Third Parties:** Understand required transparency and fairness evidence to be considered in safety-and-soundness contexts.

## 8. Template reference
- Mirrors the structure of Case Study A with numbered sections (1–10), status block, narrative, tool-typing, C072 mapping, workstreams, audience uses, sector analogues, and quick links.

## 9. Sector analogues
- Insurance: State DOI pushes carrier to adopt a telematics-based risk score with proxy discrimination concerns, backed by ORSA leverage.  
- Utilities: Regulator threatens rate-case disallowance unless a grid operator adopts a specific outage-prediction AI with opaque vendor features.  
- Healthcare: State Medicaid agency ties certification to use of a utilization-management algorithm with known racial bias, using payment holds as leverage.

## 10. Quick links
- C072 primer (internal): [link placeholder]  
- OCC 2011-12 / SR 11-7 Model Risk Management: https://www.occ.treas.gov/publications-and-resources/publications/banker-education/files/pub-model-risk-management.pdf  
- CFPB ECOA/Reg B and UDAAP guidance: https://www.consumerfinance.gov/compliance/supervision-examinations/  
- Basel III (Pillar 2) Supervisory Review: https://www.bis.org/publ/bcbs189.pdf  
- Ombudsman guidance (OCC): https://www.occ.treas.gov/topics/examiner-responsibility/ombudsman/
