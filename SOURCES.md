# Sources and Source Policy

This public call is intentionally thin.

It should not become a second authority for Koali or any other kOA subsystem.

---

## Source rule

The Civilizational Coherence source registry uses the following default logic:

```text
Interpretive document
        ↓
live repository / documentation
        ↓
current default branch
```

For an actual publication audit or formal pressure-test result, the exact reviewed commit should also be recorded.

The distinction matters:

> **Documented ≠ Implemented ≠ Tested ≠ Validated**

---

# Koali / kOA-Linux

**Live repository**

https://github.com/Rejean-McCormick/kOA-Linux

The Civilizational Coherence source registry identifies `kOA-Linux / Koali` as the live implementation reference for:

- local runtime;
- sovereignty;
- offline operation;
- integration environment.

## Canonical areas most relevant to this call

### Constitutional charter

`docs/01-constitution/00-charter.md`

Covers the constitutional frame for authority, component/data separation, profile choices, offline continuity, external integrations, AI boundaries, audit/recourse, portability/exit, and related global principles.

### Scope and non-goals

`docs/01-constitution/01-scope-and-non-goals.md`

Especially relevant to:

- preventing scope inflation;
- keeping optional integrations optional;
- avoiding universal AI requirements;
- preventing profile-specific choices from becoming global by repetition;
- ensuring removal of optional integrations does not collapse unrelated capabilities.

### Explicit authority

`docs/01-constitution/04-explicit-authority.md`

Relevant to authority ownership and prevention of silent authority inference.

### Component separation

`docs/01-constitution/07-component-separation.md`

Relevant to logical responsibility, component boundaries, and authoritative ownership.

### Data authority and ownership

`docs/01-constitution/08-data-authority-and-ownership.md`

Relevant to data-domain ownership and cross-component mutation boundaries.

### Safe degradation

`docs/01-constitution/06-safe-degradation.md`

Relevant to capability-scoped failure rather than uncontrolled total failure.

### Offline continuity

`docs/01-constitution/09-offline-continuity.md`

Relevant to declared local/offline behavior.

### Selective audit and recourse

`docs/01-constitution/10-selective-audit-and-recourse.md`

Relevant to accountability without universal exposure.

### Portability, restore and exit

`docs/01-constitution/11-portability-restore-and-exit.md`

Relevant to migration, restoration, replacement, and credible exit.

### Profile model

`docs/03-profiles/00-profile-model.md`

Relevant to required / optional / conditional / prohibited / not-applicable capability classification and deterministic profile composition.

### External integrations

`docs/02-system/16-external-integrations.md`

Relevant to integration classification, authority, data transfer, failure behavior, and removal.

### AI boundaries

`docs/02-system/09-ai-boundary.md`  
`docs/02-system/10-external-ai-surfaces.md`

Relevant to external AI as bounded, removable, non-native authority.

### Receipts and critical transitions

`docs/02-system/20-receipts-and-critical-transitions.md`

Relevant to reconstructibility of authorization, execution, commit, publication, external transfer, lifecycle, and other critical transitions.

---

# Other kOA implementation references

These may participate in a test composition but remain authoritative in their own repositories.

## Kristal

https://github.com/Rejean-McCormick/kristal-framework

Portable, versioned, provenance-bearing knowledge artifacts.

## Konnaxion

https://github.com/Rejean-McCormick/Konnaxion

Coordination, contribution, governance, deliberation, and related civic capabilities.

## Orgo

https://github.com/Rejean-McCormick/Orgo

Decision-to-execution, routing, cases, tasks, escalation, closure, and operational memory.

## SemantiK Architect

https://github.com/Rejean-McCormick/SemantiK_Architect

Structured and deterministic language realization.

## SenTient

https://github.com/Rejean-McCormick/SenTient

Ambiguity, uncertainty, and proposition-handling implementation material.

## K-Port

https://github.com/Rejean-McCormick/K-Port

Identity / credential / portability-related implementation material; scope should be verified per claim.

---

# Partners for Public Good

All PPG descriptions in this repository should be based on official PPG sources.

## Our Work

https://partnersforpublicgood.org/our-work/

PPG describes its focus on the core government levers of budgeting, procurement, technology, and staffing, with support through implementation, policy, talent, community, and learning.

## PPG Tech — Designing the Human Help that Government Technology Needs in the AI Era

https://partnersforpublicgood.org/news-events/designing-the-human-help-that-government-technology-needs-in-the-ai-era/

Denise Linn Riedl describes PPG Tech's 2026 discovery work with government technology leaders, vendors, nonprofits, and funders, including problems around technology procurement, cross-team collaboration, governance, vendor accountability, AI, and supported technology testing. The article describes PPG Tech's intent to provide vendor-neutral implementation/governance assistance, support pilots, mediate product feedback, add capacity, measure what works, and undertake government demonstration projects.

## Denise Linn Riedl

https://partnersforpublicgood.org/team/denise-linn-riedl/

Head of Public Sector Technology at PPG.

## Emily Binet Royall

https://partnersforpublicgood.org/team/emily-binet-royall/

Assistant Director overseeing the Procurement Excellence Network; her background includes public-interest technology, strategic procurement, smart cities, and responsible AI.

---

# Verification discipline

This call makes an architectural proposition, not a maturity claim.

Before a real pressure test:

1. record the Koali commit under review;
2. record the relevant profile and contract versions;
3. identify which claims are only documented;
4. identify which claims have implementation evidence;
5. identify which claims have tests;
6. identify which claims have external validation, if any.

The pressure-test result should preserve those distinctions.
