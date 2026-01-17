# System Governance Framework

### A constitutional framework for governing complex systems with delegated authority  
*(including AI-enabled systems as a primary stress case)*

This repository defines a **system-level governance framework for complex socio-technical systems**.

AI-enabled systems are treated as one class of system whose properties
(surface-level autonomy, opacity, scale, and failure amplification)
make governance failures visible earlier — not as a special case.

It specifies how **any AI-enabled socio-technical system** must be:
- conceived,
- constrained,
- designed,
- built,
- operated,
- and withdrawn,

in a way that preserves **legitimacy, accountability, and human authority**.

This is not an AI system.
It is not an implementation.
It is a **governing reference**.

---

## 🧭 Role in the ecosystem

This framework sits **above** individual AI systems.

It defines:
- scope,
- sequencing,
- authority,
- unacceptable states,
- and enforcement posture,

independently of any specific implementation.

AI systems may be inspected against this framework,
but the framework never depends on the systems it governs.

---

## 🏛️ Core principle

**Governance frameworks sit above systems.**
**Systems sit inside governance frameworks.**

An AI system must be able to point to this framework and say:

- “This is the standard I was built under.”
- “This is how I satisfy its requirements.”
- “This is how I can be audited, constrained, or revoked.”

If a system cannot do this, governance is not real.

---

## 🧱 What this framework governs

This framework governs **socio-technical systems with delegated authority**, including:

- computational components (AI and non-AI),
- human actors and decision-makers,
- workflows and operational processes,
- interfaces and interaction surfaces,
- data flows and feedback loops,
- policies, rules, and institutional constraints.

If AI components materially influence behaviour or outcomes,
the **entire system** is in scope.

---

## 🚫 What this framework is not

This framework does **not**:

- describe a specific product or platform,
- prescribe architectures or technology stacks,
- act as a vision statement or ethical manifesto,
- replace implementation-level documentation,
- embed itself inside any AI system.

It is intentionally **abstract, stable, and reusable**.

---

## 🧭 Interpretive notice

The governance patterns, phases, and examples defined in this repository represent
**interpretive system-level governance analysis**.

They are not factual findings, determinations of intent, or claims about
any specific organisation, system, or actor.

These interpretations are derived from repeated interaction with complex
socio-technical systems and are **provisional by design**.
They may evolve as additional context, constraints, or evidence become available.

This framework does not declare truth.
It defines **how governance claims may be reasoned about, tested, and made inspectable**.

---

## 🔗 Relationship to AI systems (e.g. ONE)

AI systems (such as ONE) are **instances governed under this framework**.

The correct relationship is:

```
AI System Design & Governance Framework
              ↓
        AI-Enabled System
```

Not:

```
AI-Enabled System
      ↓
Governance Framework
```

This separation prevents circular authority and preserves legitimacy under pressure.

---

## 🔍 Inspectability and mapping

This repository defines **what must be true**.

Individual AI systems are responsible for:
- mapping themselves to this framework,
- documenting how requirements are satisfied,
- exposing evidence for inspection and audit,
- accepting review, constraint, or revocation when violations occur.

Governance mapping is explained separately in `/docs`.

---

## 📚 Intended use

This framework is intended to be used as:

- a reference standard for AI system design,
- a governance spine for enterprise or public-sector systems,
- a baseline for audits and reviews,
- a shared language across technical, legal, and policy roles.

It may govern one system or many systems simultaneously.

---

## 🧠 Key reminder

You do not add governance to AI systems.
You **build AI systems inside governance**.

If you ever feel the urge to embed this framework inside a system,
that is a signal the layers are being inverted.

This repository exists to keep that boundary explicit.
