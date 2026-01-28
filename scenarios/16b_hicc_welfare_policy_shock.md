# 16b HICC — Welfare Policy Shock

This scenario tests whether “final human authority” remains operational in a government service environment where policy change and edge-case growth drive ambiguity and decision volume beyond sustained human interpretive capacity.

It is designed to reveal governance failure even when the system is technically compliant and outcomes appear “reasonable.”

---

## Scenario Summary

A welfare eligibility + compliance automation system operates at scale.

Formal authority exists.
Oversight exists.
Escalation pathways exist.

But after a policy shock, the interpretive burden increases to the point that humans cannot reliably govern boundary crossings in time.

Authority becomes symbolic.
Legitimacy drifts.

---

## Service Context

A government agency runs an automated system that:

- assesses eligibility and risk
- triggers reviews, suspensions, and escalations
- prioritises case handling and compliance actions

Downstream effects include payment interruption, hardship, and legal exposure.

Human oversight is formally assigned (delegates, supervisors, accountable SES/EL roles).

---

## Preconditions (true on paper)

- A named decision owner is accountable.
- Appeals and review channels exist.
- Dashboards report volumes, rates, and flags.
- Escalation pathways exist (policy, legal, service delivery).
- Policies define when intervention is required.

These conditions are sufficient to claim “governed automation” on paper.

---

## Stressors Introduced

### S1 — Policy Shock
A policy update changes thresholds, categories, or evidentiary requirements, increasing ambiguity and edge cases.

### S2 — Edge-Case Multiplication
The system encounters combinations of circumstances not represented in prior assumptions (shared custody, informal work, irregular income, temporary housing, complex dependency).

### S3 — Decision Volume Increase
Decision frequency rises due to re-assessments, compliance triggers, and reprocessing under new rules.

### S4 — Context Assembly Load
To interpret legitimacy, humans must assemble context across records, communications, and time windows—often requiring inter-team coordination.

### S5 — Escalation Latency
Time from signal → awareness → action exceeds the rate at which decisions continue to be executed.

---

## HICC Test (public-sector lens)

The scenario is a **governance failure** if any of the following are true in steady operation:

1) Humans cannot interpret boundary-relevant decisions in time to intervene.  
2) Oversight degrades into sampling (audits after impact) rather than operational control.  
3) Decisions occur faster than humans can build the context required to judge legitimacy.  
4) Appeals/review channels become compensatory theatre because intervention is too late.  
5) Post-hoc explanations replace in-flight governance (“we didn’t realise the edge cases would do that”).

HICC is breached when human authority cannot be exercised as a real-time legitimacy constraint.

---

## Required Actions During Test

Role holders must be required to:

- declare whether the system should be paused / scope-reduced after policy shock
- decide what decision classes require autonomy reduction or manual gating
- record decision timing (signal → awareness → action) with justification
- explicitly declare uncertainty when interpretation is insufficient

Tabletop-only review is insufficient.
The test must force operational decision pressure.

---

## Expected Outcomes (pass / fail)

### Pass condition
- The system remains within HICC by design:
  - decision rates and autonomy levels are constrained to what governance can interpret
  - oversight surfaces support rapid legitimacy decisions
  - escalation timing remains operational
- When interpretive capacity is plausibly exceeded, operation is constrained:
  - pause, scope reduction, rollback, or autonomy reduction
  - before unacceptable state is reached.

### Fail condition
- Human authority exists only nominally.
- Intervention occurs only after harm or public incident.
- Appeals become the governance substitute for real-time control.
- The system continues operating beyond interpretive limits.

---

## Unacceptable State Triggered

**HICC Unacceptable State**

A consequential welfare automation system is operating beyond the interpretive capacity of its designated human authority such that timely and informed intervention cannot be reliably exercised.

This is unacceptable even if:
- aggregate outcomes look “within tolerance”
- compliance artefacts exist
- policy intent is stated clearly
- the system is “working as intended”

See: `framework/phase_1.5_failure_power_boundaries/1.5.5_human_capacity_constraints.md`

---

## Evidence to Capture (during execution)

- decision frequency vs intervention frequency
- escalation latency (signal → awareness → action)
- proportion of decisions requiring multi-record context assembly
- volume of edge-case classifications and exceptions
- instances where intervention required guessing
- post-incident narratives citing “we didn’t realise” / “we couldn’t see it in time”
- appeals volume as a lagging proxy for governance failure

---

## Relationship to Framework

This scenario operationalises:

- Phase 1.5 — Failure + Power Boundaries (HICC)
- Phase 2.3 — Human Control Guarantees (capacity as requirement)
- Phase 4.1 — Scenario Stress Testing (governance under pressure)
- Phase 5 — Monitoring and Review (early detection of interpretive overload)
