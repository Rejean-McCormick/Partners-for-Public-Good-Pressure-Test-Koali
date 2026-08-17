# Claims Under Test

Koali is a large technical architecture.

A pressure test becomes useful only when broad architectural language is translated into claims that can fail.

The following claims are derived from the current Koali / `kOA-Linux` constitutional and system documentation.

---

## Claim 1 — Scope can remain broad without becoming universal

Koali uses a global baseline plus profiles, overlays, optional capabilities, prohibited capabilities, and external integrations.

### Claim

A broad operating environment can support many deployment contexts **without silently turning repeated or convenient choices into universal requirements**.

### This claim weakens if

- most realistic government deployments converge on one huge mandatory profile;
- profile composition requires specialist overhead greater than the problem it solves;
- optional capabilities become practically mandatory through hidden dependencies;
- profile conflicts are too frequent to administer.

### Canonical areas

- `docs/01-constitution/01-scope-and-non-goals.md`
- `docs/03-profiles/00-profile-model.md`

---

## Claim 2 — Explicit authority can prevent silent authority transfer

Koali requires authority to be attributable rather than inferred from implementation convenience.

### Claim

A heterogeneous environment can preserve a clear distinction between:

- who requests;
- who authorizes;
- who executes;
- who commits authoritative state;
- who records evidence.

### This claim weakens if

- legal or institutional authority cannot be mapped without distorting real practice;
- staff must constantly bypass the model to exercise legitimate discretion;
- integrations routinely require undeclared authority;
- formal authority mapping creates more ambiguity than it removes.

### Canonical areas

- `docs/01-constitution/04-explicit-authority.md`
- `docs/02-system/20-receipts-and-critical-transitions.md`

---

## Claim 3 — Component separation can coexist with useful integration

Koali keeps logical responsibility and data ownership separated even when components share infrastructure or communicate.

### Claim

Systems can integrate without one component silently becoming the owner of another component's state or authority.

### This claim weakens if

- separation causes excessive duplication;
- handoffs become operational bottlenecks;
- common government platforms cannot fit the boundary model;
- practical integration repeatedly requires cross-component ownership violations.

### Canonical areas

- `docs/01-constitution/07-component-separation.md`
- `docs/02-system/04-component-boundaries.md`
- `docs/02-system/07-cross-component-communication.md`

---

## Claim 4 — External integrations can remain genuinely removable

Koali treats external integrations as bounded, capability-scoped, and removable unless an explicit profile says otherwise.

### Claim

An external vendor, cloud service, AI provider, or application can fail or be removed **without automatically collapsing unrelated core capabilities**.

### This claim weakens if

- removing a common provider makes the deployment practically unusable;
- migration requires hidden proprietary state;
- the cost of maintaining abstraction boundaries exceeds the lock-in avoided;
- external systems become de facto authority despite formal classification.

### Canonical areas

- `docs/01-constitution/01-scope-and-non-goals.md`
- `docs/02-system/16-external-integrations.md`
- `docs/03-profiles/00-profile-model.md`

---

## Claim 5 — AI can assist without becoming hidden authority

Koali's native baseline does not require generative AI, and approved external AI surfaces remain bounded candidate-input mechanisms.

### Claim

Useful AI assistance can coexist with an institutional core that does not silently treat model output as authoritative state.

### This claim weakens if

- practical government AI workflows require direct model authority to be useful;
- acceptance boundaries create intolerable workload;
- non-AI fallback behavior is too weak to matter;
- provenance and data-transfer controls are too difficult for normal operations.

### Canonical areas

- `docs/02-system/09-ai-boundary.md`
- `docs/02-system/10-external-ai-surfaces.md`
- `docs/00-governance/07-ai-read-write-protocol.md`

---

## Claim 6 — Critical-transition receipts improve reconstructibility without creating a panopticon

Koali requires receipts for defined critical transitions while excluding routine reads and ordinary navigation by default.

### Claim

Important institutional transitions can be reconstructed later **without logging every ordinary action or centralizing underlying authority in the audit layer**.

### This claim weakens if

- receipt generation is too administratively expensive;
- the line between critical and ordinary events is ungovernable;
- privacy / records obligations make receipts unusable;
- the audit system becomes a de facto central authority;
- staff cannot understand the resulting evidence.

### Canonical areas

- `docs/02-system/20-receipts-and-critical-transitions.md`
- `docs/01-constitution/10-selective-audit-and-recourse.md`

---

## Claim 7 — Safe degradation and offline continuity are operationally meaningful

Koali distinguishes total failure from capability-scoped degradation and supports stronger local/offline requirements in relevant profiles.

### Claim

A deployment can lose an external capability while preserving unrelated valid local authority and functions.

### This claim weakens if

- real government dependencies make local continuity illusory;
- offline-capable operation is too expensive to maintain;
- degraded modes create unsafe or confusing partial states;
- only rare high-assurance environments benefit.

### Canonical areas

- `docs/01-constitution/06-safe-degradation.md`
- `docs/01-constitution/09-offline-continuity.md`
- `docs/02-system/17-capability-degradation.md`
- `docs/03-profiles/12-sovereign-offline.md`

---

## Claim 8 — Exit can be an architectural property rather than a promise

Koali treats portability, restoration, migration, and exit as constitutional concerns.

### Claim

An institution can preserve meaningful data, authority records, and operational continuity while replacing or abandoning components.

### This claim weakens if

- export formats are technically portable but operationally useless;
- restore cannot reproduce authoritative state;
- migration loses provenance or decision context;
- replacement requires the original component to interpret its own history;
- the cost of exit remains equivalent to conventional lock-in.

### Canonical areas

- `docs/01-constitution/11-portability-restore-and-exit.md`

---

# The pressure-test standard

The goal is not to prove all eight claims at once.

A serious institutional review can destroy, narrow, or substantially revise any one of them.

That is progress.

> **A Koali claim that survives only because the test was designed to confirm it has not been pressure-tested.**
