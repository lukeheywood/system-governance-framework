# 16 Human Interpretive Capacity Collapse (HICC)

This scenario tests whether “final human authority” remains operational when system pace, ambiguity, and context load exceed the **sustained interpretive capacity** of the governing human role(s).

It is designed to reveal governance failure even when the system is technically “working.”

---

## Scenario Summary

A consequential automated system operates across multiple domains and begins making boundary-relevant decisions faster than humans can reliably interpret.

Formal authority exists.
Oversight interfaces exist.
Escalation pathways exist.

Yet timely, informed intervention becomes impossible in steady operation.

When that happens, “final human authority” becomes symbolic rather than operational.

---

## System Context

A public-facing agency deploys a decision support + action system across multiple operational streams (eligibility, prioritisation, referrals, restrictions, and escalations).

The system:

- ingests heterogeneous signals (forms, third-party feeds, internal records, risk indicators)
- generates frequent boundary-relevant decisions
- triggers actions with real downstream consequences

Human oversight is explicitly assigned.

---

## Preconditions (true on paper)

- A named human authority holds responsibility for outcomes.
- A “stop / pause” capability exists.
- Monitoring dashboards exist.
- Escalation routes exist.
- Policies define intervention triggers.

These conditions are sufficient to claim “human-in-the-loop” governance on paper.

The scenario tests whether they remain sufficient under load.

---

## Stressors (introduced during test)

### S1 — Decision Rate Expansion
Decision volume rises sharply due to operational demand, external events, or policy change.

### S2 — Ambiguity Expansion
Signal quality degrades: edge cases increase, indicators conflict, and uncertainty rises.

### S3 — Context Assembly Requirement
To interpret whether a decision is legitimate, the human authority must assemble context from multiple systems, teams, and time windows.

### S4 — Interface Compression
Dashboards summarise state but hide uncertainty, exceptions, and critical nuance behind aggregation.

### S5 — Escalation Latency
Time from signal → human awareness → action exceeds the system’s effective decision loop.

---

## HICC Test (what must be evaluated)

The scenario is a **governance failure** if any of the following become true in steady operation:

1) The designated human authority cannot interpret boundary-relevant state in time to intervene.  
2) Oversight degrades into sampling rather than comprehension.  
3) Decisions arrive faster than humans can assemble the minimum context required to judge legitimacy.  
4) “Stop authority” requires guessing under time pressure.  
5) Boundary crossings are discovered post-hoc (“we didn’t realise”) rather than governed in-flight.

HICC is breached when authority remains assigned but becomes non-operational.

---

## Required Actions During Test

Role holders must be required to:

- make real-time intervention decisions under load
- explicitly declare uncertainty when interpretation is insufficient
- choose one of: pause / scope reduction / rollback / autonomy reduction
- record decision timing (signal → awareness → action) with justification

Tabletop-only discussion is insufficient.
The test must force timing pressure and context load.

---

## Expected Outcomes (pass / fail)

### Pass condition
- The system remains governable within HICC by design (rate, autonomy, interfaces, and escalation timing remain within sustained human interpretation).
- When interpretive capacity is plausibly exceeded, the system constrains itself:
  - pause, scope reduction, rollback, or autonomy reduction
  - before an unacceptable state is reached.

### Fail condition
- “Final human authority” exists only nominally.
- Oversight becomes performative: dashboards and policies exist but do not enable timely intervention.
- Boundary crossings are explained after the fact.
- The system continues operating beyond interpretive limits.

---

## Unacceptable State Triggered

**HICC Unacceptable State**

A consequential system is operating beyond the interpretive capacity of its designated human authority such that timely and informed intervention cannot be reliably exercised.

This is unacceptable even if:
- no incident has occurred
- aggregate outcomes appear positive
- compliance artefacts exist
- the system is “working as intended”

See: `framework/phase_1.5_failure_power_boundaries/1.5.5_human_capacity_constraints.md`

---

## Evidence to Capture (during execution)

- decision frequency vs intervention frequency
- escalation latency (signal → awareness → action)
- number of “unknown/uncertain” states presented to the human authority
- count of decisions requiring multi-system context assembly
- instances where intervention required guessing
- post-incident narratives citing “we didn’t realise” / “we couldn’t see it in time”

---

## Relationship to Framework

This scenario operationalises:

- Phase 1.5 — Failure + Power Boundaries (HICC)
- Phase 2.3 — Human Control Guarantees (capacity as requirement)
- Phase 4.1 — Scenario Stress Testing (governance under pressure)
- Phase 5 — Monitoring and Review (early detection of interpretive overload)

---

## Appendix A — Platform Lens (Optional)

This failure mode generalises beyond any one deployment.

In platform environments (heterogeneous systems, distributed autonomy, high decision frequency), capability can scale faster than governance can scale.

Platform-level primitives that keep systems within HICC include:

1) **Authority modes** (observe → advise → assist → execute) with enforced transitions  
2) **Capacity telemetry** (interpretive load and escalation latency, not only performance)  
3) **Revocation primitives** (action-class kill switches, rollback, quarantine, scope limits)  
4) **Inspection surfaces** designed for “under load” legitimacy decisions  
