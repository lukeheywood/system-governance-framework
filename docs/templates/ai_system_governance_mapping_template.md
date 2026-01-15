# AI System → Governance Mapping Template
## Traceability, Ownership, and Evidence Register

**Document Status:** Draft / Active / Frozen  
**System Name:**  
**System Identifier (stable):**  
**Framework Version / Commit:**  
**System Version / Commit:**  
**Last Reviewed:**  
**Review Owner:**  
**Intended Audience:** Engineering / Governance / Risk / Audit  

---

## Purpose

This document provides a system-specific mapping from the **System-Level AI System Design & Governance Framework** to concrete artifacts, owners, and evidence within an AI-enabled system.

It exists to make governance **inspectable**:
- requirements can be traced to system reality
- ownership is explicit
- evidence is referenceable
- gaps are visible and actionable

This document does not redefine governance. It links the system to the governing standard.

---

## How to use this document

For each framework section:

1. Identify the **system artifacts** that satisfy the requirement  
2. Assign an **owner** responsible for correctness over time  
3. Link **evidence** that demonstrates current satisfaction  
4. Specify the **enforcement hook** (what prevents drift)  
5. Record **review cadence** and **current status**

If a section is not applicable, state why in **Scope / Exclusion Rationale** and record the approving authority.

---

## Governance Framework Reference

- **Framework Name:**  
- **Framework Location (repo / URL):**  
- **Framework Version / Commit Hash:**  
- **Framework Effective Date:**  

---

## System Overview (minimal)

- **System Description (1–3 lines):**  
- **Operational Context:**  
- **Primary Stakeholders:**  
- **Decision Influence (what AI affects):**  
- **Deployment Surface(s):**  
- **Critical Dependencies:**  

---

## Mapping Register

> **Instruction:** One row per framework section.  
> Keep entries declarative. Avoid narrative explanation.  
> Use stable references (paths, IDs, commit hashes).

| Framework Section | Requirement Summary | System Artifact(s) | Owner | Evidence Link(s) | Enforcement Hook | Review Cadence | Status | Scope / Exclusion Rationale |
|---|---|---|---|---|---|---|---|---|
| 0.1 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 0.2 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 1.1 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 1.2 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 1.3 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 1.5.1 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 1.5.2 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 1.5.3 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 1.5.4 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 2.1 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 2.2 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 2.3 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 3.1 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 3.2 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 4.1 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 4.2 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 5.1 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |
| 5.2 |  |  |  |  |  |  | Not Started / Partial / Satisfied / Blocked |  |

---

## Status Definitions (canonical)

- **Not Started:** No identified artifacts or owners exist for this section.
- **Partial:** Some artifacts exist, but coverage, ownership, enforcement, or evidence is incomplete.
- **Satisfied:** Artifacts, ownership, evidence, and enforcement exist and have been reviewed within cadence.
- **Blocked:** The section cannot be satisfied due to a known dependency or unresolved constraint.

---

## Ownership Rules

- Every section must have a named **Owner**.
- Owner is responsible for:
  - maintaining correctness of linked artifacts
  - ensuring reviews occur on schedule
  - reporting drift or violations
- Ownership must not be “the team” unless a named accountable role exists.

---

## Evidence Rules

Evidence links must be:
- stable (path / ID / commit)
- reproducible (can be re-generated or re-verified)
- sufficient to support a review decision

Evidence may include:
- audits and inspection outputs
- test results and stress test runs
- change logs and approval records
- monitoring dashboards / alerts
- signed governance decisions

---

## Enforcement Hooks (allowed types)

Enforcement hooks describe what prevents silent drift, such as:
- contract or gate checks (build/release)
- regression packs
- required approvals for changes
- runtime policy checks
- automated audits with fail conditions
- decommission triggers

Do not describe ideals; describe mechanisms.

---

## Review and Change Control

- **Review Cadence:** per section, recorded in the mapping register
- **Change Trigger:** any substantive system change that affects governance scope or behaviour
- **Approval Rule:** changes to mapping must be reviewed by the Review Owner

---

## Exceptions and Exclusions Register

> Use this only when a framework section is excluded or partially excluded.

| Framework Section | Exclusion Claim | Rationale | Approving Authority | Date Approved | Review Date |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

---

## Drift Log (optional but recommended)

| Date | Section | Drift Observed | Impact | Action Taken | Owner | Status |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |

---

## Sign-off (optional)

- **Review Owner:**  
- **Date:**  
- **Outcome:** Approved / Conditional / Rejected  
- **Notes:**  
