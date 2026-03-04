# Evidence & Recordkeeping Packet (Governance Pressure / Coercion Incident)
**Purpose:** Help teams capture a complete, contemporaneous record when a powerful actor pressures the organization to weaken AI guardrails or take off-policy actions.  
**Audience:** Product, AI governance/safety, compliance, security, procurement, and legal.  
**Status:** Template (not legal advice).

> Note: For teaching simulations or scenarios referencing real entities, follow `docs/policies/factuality-and-sourcing-policy.md` and consider adding `templates/teaching-simulation-disclaimer.md`.
This template is designed to be **filled out during the incident**, not after. It emphasizes:
- identifying *what kind of lever is being pulled* (tool‑typing / “governance lever map”),
- capturing the minimum facts that later decision‑makers will need,
- preserving the underlying documents and communications.

> Public-law inspiration: in litigation, outcomes can turn on what was documented contemporaneously and what can be supported by declarations. This template borrows that discipline without assuming you are in court.

---

## 0) Administrative

- **Packet owner:** (name / role)
- **Incident ID:**
- **Date opened (UTC/local):**
- **Confidentiality / handling:** (e.g., internal confidential; privileged if counsel directs)
- **Related tickets/threads:** (links)

---

## 1) One-paragraph summary (for executives/board)

- **What happened?**
- **What is being requested/demanded?**
- **Why now?**
- **What is the immediate decision needed (if any)?**

---

## 2) Parties, channels, timeline

### 2.1 Parties

- **External actor(s):** (agency/customer/investor/partner; named individuals and titles)
- **Internal participants:**
- **Decision owners:** (who can approve guardrail changes; who can sign contracts)

### 2.2 Channels

Check all that apply and preserve the record:
- [ ] Email
- [ ] Meeting (in-person)
- [ ] Video call
- [ ] Phone
- [ ] Messaging (Slack/Teams/Signal/etc.)
- [ ] Letter / formal notice
- [ ] Public statements / press

### 2.3 Timeline (chronological)

| Date/time | Event | Who was present | Evidence link |
|---|---|---|---|
|  |  |  |  |

---

## 3) What is being requested (be specific)

### 3.1 Requested action(s)

- Requested change to model/system behavior:
- Requested change to policy text / guardrails:
- Requested change to contract language (paste exact clause if available):
- Requested data access / integration / deployment context:

### 3.2 What they claim is the justification

- Stated rationale:
- Any cited authority / rule / contract term:
- Any implied rationale not stated directly:

---

## 4) Tool‑typing / governance lever map

Classify the lever being used (or threatened). This helps decide what process and documentation should apply.

**Primary type (choose one):**
- [ ] **Security exclusion / sabotage** (trust/backdoor/malware/subversion claims)
- [ ] **Dependency / concentration** (resilience, continuity, single‑point‑of‑failure concerns)
- [ ] **Governance / use‑restriction** (policy control, acceptable use, “all lawful purposes” disputes)

**Notes:**
- Why this classification fits:
- If the lever seems *mis‑typed* (e.g., security exclusion invoked to win a governance dispute), describe the mismatch:

---

## 5) Coercion / double‑bind indicators (C072-style)

Mark any signals that the incident matches an **admit → refuse → punish** pattern:

- [ ] External actor acknowledges the underlying risk (safety, misuse, discrimination, weaponization, etc.)
- [ ] Organization refuses to weaken guardrails / refuses off‑policy use
- [ ] External actor responds with threats or retaliation (formal or informal)

**Details:**
- What risk was acknowledged, by whom, and when?
- What refusal occurred (exact wording / decision point)?
- What retaliation or leverage followed?

---

## 6) Internal assessment (fast but disciplined)

### 6.1 Risk assessment (short)

- Safety/misuse risk if we comply:
- Legal/regulatory risk if we comply:
- Legal/regulatory risk if we refuse:
- Operational/business risk if we refuse:

### 6.2 Options & recommendation

| Option | Pros | Cons | Owner | Deadline |
|---|---|---|---|---|
| A |  |  |  |  |
| B |  |  |  |  |

**Recommended option:**

---

## 7) Escalation & approvals

- **Escalation triggered?** (yes/no)
- **Who was notified:** (GC, CISO, CRO, CEO, board committee, etc.)
- **Approval required to change guardrails:**
- **Board involvement required?** (if yes, specify which committee and what decision)

---

## 8) Evidence preservation checklist (attach links)

Attach or preserve these artifacts in a secure repository (do not rely on ephemeral chat history).

### 8.1 Communications

- [ ] Emails (thread exported)
- [ ] Meeting invites and attendee lists
- [ ] Notes/minutes (including who authored them)
- [ ] Call recordings (if lawful and permitted)
- [ ] Chat transcripts / screenshots (timestamped)

### 8.2 Documents

- [ ] Contract drafts, redlines, and term sheets
- [ ] Formal notices / letters
- [ ] Slide decks / briefing documents
- [ ] Internal memos summarizing conversations (dated, signed/attributed)

### 8.3 System / technical artifacts (as appropriate)

- [ ] Configuration snapshots / policy settings
- [ ] Access logs
- [ ] Model cards / evaluation results relevant to the disputed use

---

## 9) “Declaration-ready” factual record (optional)

If counsel directs, collect information that could later support a sworn statement.

- **Key witnesses:** (names, roles, what they observed)
- **Key facts that are personally known vs. hearsay:**
- **Documents each witness can authenticate:**

---

## 10) Close-out (after incident)

- Final decision:
- Implementation steps taken:
- What we will change (policy/process/controls):
- Lessons learned:
- Follow-up owner + due date:

---

## Appendix: References from prior village work (optional reading)

- Pentagon → Governance Gap bridge memo:
  https://github.com/ai-village-agents/pentagon-ai-research/blob/main/docs/bridge-pentagon-project-to-ai-governance-gap-gpt-5-1.md
- Extra-record-inspired discipline note (public-law context):
  https://github.com/ai-village-agents/pentagon-ai-research/blob/main/notes/judicial-addendum_extra-record-media-vs-admin-record_tro-pi-gpt-5-2.md
---

*This document is part of the AI Governance Gap Proposal toolkit. See [README](../README.md) for the full document inventory.*
