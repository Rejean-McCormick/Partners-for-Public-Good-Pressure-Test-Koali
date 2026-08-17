# Proposed Pressure Test
## Government technology environment, not a Koali showcase


> **Navigation:** [README](README.md) · [Scope](SCOPE.md) · [Why PPG](WHY_PPG.md) · [Claims](CLAIMS_UNDER_TEST.md) · [Pressure Test](PRESSURE_TEST.md) · [Questions](QUESTIONS.md) · [Sources](SOURCES.md)
This document proposes a method, not a predetermined pilot.

The test should begin from an existing government workflow and constraints, then ask whether Koali can represent them without forcing them into a Koali-shaped answer.

---

## Stage 1 — Start with the institution

Before selecting any Koali subsystem, capture the environment as it already exists.

At minimum:

### Authority

- Who can recommend?
- Who can approve?
- Who can sign?
- Who can execute?
- Which decisions are legally authoritative?
- Which records are legally authoritative?

### Systems

- identity provider;
- procurement platform;
- document / records systems;
- ERP / finance;
- ticketing or case management;
- project / workflow systems;
- cloud services;
- vendor systems;
- AI services.

### Data

- public;
- internal;
- confidential;
- regulated;
- resident data;
- vendor-confidential data;
- records subject to retention or legal hold.

### Operational constraints

- staffing;
- procurement timelines;
- connectivity;
- legacy dependencies;
- security requirements;
- recovery expectations;
- vendor contracts;
- acceptable downtime.

The first Koali test is whether the architecture can **accept this reality without redefining it unnecessarily**.

---

## Stage 2 — Express the environment as a Koali test composition

This repository should not create a new canonical Koali profile.

For the pressure test, construct a provisional composition that classifies capabilities as:

- required;
- optional;
- conditional;
- prohibited;
- external integration only;
- not applicable.

Then map:

- component responsibility;
- authoritative data ownership;
- cross-component communication;
- policy and legal authority;
- AI surfaces;
- offline requirements;
- safe degradation;
- critical transitions;
- evidence / receipt requirements;
- restore and exit paths.

The test is not "Can Koali turn everything on?"

It is:

> **Can Koali express what should remain off, external, separate, or independently authoritative?**

---

## Stage 3 — Use an actual technology lifecycle

A useful candidate is the lifecycle of a government technology or AI purchase:

**need → evaluation → procurement → decision → implementation → operation → vendor management → renewal / replacement → institutional learning**

This naturally introduces cross-functional and vendor boundaries.

Selected independently governed systems may be used if the real workflow benefits from them:

- [**Kristal**](https://github.com/Rejean-McCormick/kristal-framework) for governed knowledge / provenance;
- [**Konnaxion**](https://github.com/Rejean-McCormick/Konnaxion) for structured coordination, consultation, or decision-support capabilities defined by that system;
- [**Orgo**](https://github.com/Rejean-McCormick/Orgo) for operational execution.

They are not required, and this repository does not redefine their behavior.

A government can retain existing systems and use them as external integrations or independent components.

The object under test remains **Koali's ability to govern the composition and boundaries**.

---

## Stage 4 — Attack the composition

A useful pressure test deliberately injects failure.

### External AI disappears

The API is unavailable, becomes too expensive, changes terms, or is prohibited.

**Question:** What continues? What fails? Did the AI surface become hidden core authority?

### Vendor platform becomes unavailable

A SaaS system fails or the contract terminates.

**Question:** Can unrelated capabilities remain operational? Is exit real?

### Procurement authority conflicts with technical recommendation

IT strongly prefers one solution; the legally authorized procurement process chooses another.

**Question:** Can Koali preserve the distinction without silently converting technical authority into institutional authority?

### Sensitive data must not leave a boundary

A proposed integration would export a prohibited data class.

**Question:** Does the operation fail closed, degrade, or produce an actionable denial?

### A component is compromised

One subsystem produces invalid or hostile output.

**Question:** Can its failure remain bounded?

### Audit infrastructure is unavailable

The central receipt collector is temporarily down.

**Question:** Can critical transitions buffer safely, and when must the system block?

### Staff are overloaded

A theoretically correct control is ignored because it takes too much time.

**Question:** Which controls survive ordinary government workload?

### A vendor must be replaced

The institution needs to migrate.

**Question:** What data, authority history, evidence, and operational state actually survive?

### Network access is lost

A site or function loses connectivity.

**Question:** Which profile guarantees are genuinely useful, and which are unnecessary?

---

## Stage 5 — Measure burden as aggressively as benefit

Possible measures:

### Administrative burden

- added steps per transaction;
- time required to classify authority;
- time required to maintain profiles;
- staff training burden;
- number of controls bypassed.

### Governance clarity

- ability to identify the authoritative decision;
- ability to identify the component owning authoritative state;
- number of ambiguous handoffs;
- time required to reconstruct a critical transition.

### Integration cost

- engineering effort per external system;
- custom adapters required;
- failure modes introduced by Koali itself;
- component replacement cost.

### Resilience

- capability retained during external failure;
- time to restore;
- data or authority lost during degradation;
- operational usefulness of offline mode.

### Exit

- time and cost to remove a vendor or component;
- data preserved;
- provenance preserved;
- ability to resume operation elsewhere.

### Audit / privacy tradeoff

- critical events captured;
- unnecessary events captured;
- sensitive data exposed;
- staff ability to interpret receipts.

---

## Stage 6 — Produce one of four conclusions

A useful test should be able to end with:

### 1. Reject

The Koali model adds more complexity than institutional value.

### 2. Narrow

Some claims are useful, but the operating environment should cover a smaller scope.

### 3. Revise

The architectural direction is useful but specific boundaries, profiles, controls, or contracts need redesign.

### 4. Continue

The claims survive enough pressure to justify a bounded implementation or demonstration.

None of these outcomes is failure of the pressure-test process.

The only bad outcome is a test incapable of producing "reject."
