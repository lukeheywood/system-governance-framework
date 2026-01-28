# 16a HICC — Platform Autonomy Surge

This scenario tests whether “final human authority” remains operational in a platform environment where distributed autonomy, decision frequency, and optimisation feedback loops exceed sustained human interpretive capacity.

It is designed to reveal governance failure even when platform health metrics look “green.”

---

## Scenario Summary

A large platform introduces an automation layer that optimises routing, throttling, and resource allocation across many workloads.

Formal authority exists.
Control surfaces exist.
Escalation pathways exist.

But under real operational load, the governing humans cannot reliably interpret boundary-relevant state in time to intervene.

Authority becomes symbolic.

---

## Platform Context

A heterogeneous platform (services, pipelines, workloads, queues, accelerators, schedulers) operates across multiple teams and domains.

The automation layer:

- makes frequent boundary-relevant decisions (prioritisation, throttles, quarantine, reroutes)
- adapts continuously based on telemetry and learned behaviour
- affects downstream reliability, cost, and availability

A designated authority (platform lead / on-call commander / change owner) holds responsibility for safe operation.

---

## Preconditions (true on paper)

- A named decision owner is accountable.
- A “kill switch” / pause capability exists.
- Dashboards exist (health, latency, errors, capacity).
- Alerting and escalation routes exist.
- Runbooks describe intervention criteria.

These conditions are sufficient to claim “human-controlled automation” on paper.

---

## Stressors Introduced

### S1 — Autonomy Expansion
The automation layer is extended to additional workloads and decision classes without changing oversight bandwidth.

### S2 — Decision Rate Expansion
Decision frequency rises due to demand spikes, multi-tenant contention, or cascading retries.

### S3 — Interaction Complexity
Multiple automated subsystems interact (schedulers, throttles, rate limiters, failover, anomaly responders), producing emergent behaviour.

### S4 — Interface Compression
Dashboards aggregate health but conceal uncertainty, local exceptions, and cross-service dependency chains.

### S5 — Escalation Latency
Time from signal → human awareness → action exceeds the pace at which the platform state is evolving.

---

## HICC Test (platform lens)

The scenario is a **governance failure** if any of the following are true in steady operation:

1) Humans cannot interpret boundary-relevant state in time to intervene.  
2) Oversight degrades into sampling (“we looked at a few services”) rather than comprehension.  
3) Intervention requires guessing because the system’s current state cannot be reconstructed fast enough.  
4) “Kill switch” exists but is too coarse or too risky to use, so it becomes ceremonial.  
5) Post-hoc explanations replace in-flight governance (“we didn’t realise the interaction would do that”).

HICC is breached when platform autonomy outpaces human interpretability.

---

## Required Actions During Test

Role holders must be required to:

- decide whether to pause / scope-reduce / rollback automation under load
- identify the boundary being crossed (authority, safety, legitimacy, availability)
- record decision timing (signal → awareness → action) with justification
- declare uncertainty explicitly when interpretation is insufficient

Tabletop-only review is insufficient.
The test must force real-time decision pressure.

---

## Expected Outcomes (pass / fail)

### Pass condition
- The platform remains governable within HICC by design:
  - autonomy limits are enforced
  - control surfaces support rapid interpretation
  - escalation timing remains operational
- When interpretive capacity is plausibly exceeded, automation constrains itself:
  - pauses, scope reductions, quarantines, or autonomy reductions
  - before unacceptable state is reached.

### Fail condition
- Humans retain nominal authority but cannot interpret in time.
- Control surfaces do not support legitimacy decisions under load.
- Kill switches are unused because they are too blunt or too costly.
- The platform continues operating beyond interpretive limits.

---

## Unacceptable State Triggered

**HICC Unacceptable State**

A consequential platform automation layer is operating beyond the interpretive capacity of its designated human authority such that timely and informed intervention cannot be reliably exercised.

This is unacceptable even if:
- aggregate health metrics remain positive
- incident rates are low
- the system is “optimising as intended”

See: `framework/phase_1.5_failure_power_boundaries/1.5.5_human_capacity_constraints.md`

---

## Evidence to Capture (during execution)

- decision frequency vs intervention frequency
- escalation latency (signal → awareness → action)
- count of interacting automation subsystems active at once
- number of decisions requiring cross-service context assembly
- instances where intervention required guessing
- post-incident narratives citing “we didn’t realise” / “we couldn’t see it in time”

---

## Relationship to Framework

This scenario operationalises:

- Phase 1.5 — Failure + Power Boundaries (HICC)
- Phase 2.3 — Human Control Guarantees (capacity as requirement)
- Phase 4.1 — Scenario Stress Testing (governance under pressure)
- Phase 5 — Monitoring and Review (early detection of interpretive overload)
