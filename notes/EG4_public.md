# EG4 Public Note (Rigidity and Endpoint Transfer)

Canonical wording: `bad-limit exclusion / endpoint transfer`.

In-paper anchor: `paper/GREEN_GRIFFITHS_LANG_CONJECTURE_PREPRINT.md` (`GGL_G4`, `GGL_G5`).

## Goal
Separate the rigidity job from the endpoint-transfer job for `proving algebraic degeneracy of entire curves on varieties of general type through an admissible hyperbolic closure architecture`.
The older wording `rigidity and endpoint-transfer` corresponds to bad-limit exclusion plus the bridge into the intended endpoint object.

## Objects

- bad-limit class: candidates extracted by the compactness gate but incompatible with closure.
- rigidity floor: `rho_rigidity`.
- endpoint-transfer lock: `jet_transfer`.
- coherence interface: `eps_coh` remains available to the bridge and final margin.

## Closure Criterion

`GGL_G4` closes when `rho_rigidity` excludes bad endpoint alternatives: bad entire-curve countermodels are excluded.
`GGL_G5` closes when `jet_transfer` transfers the surviving endpoint to the intended target class: rigid limit transfers to the Green-Griffiths-Lang endpoint class.
Together they feed the strict margin `M_GGL`.

## Lemma Chain and Proof Payload

### Lemma EG4.1 (bad-limit exclusion)
Every extracted bad limit contradicts a declared rigidity constraint or leaves the admissible class.

Payload: check `rho_rigidity` in the registry and certificate surfaces.

### Lemma EG4.2 (endpoint transfer)
The surviving rigid representative is locked to the standard problem-side endpoint by `jet_transfer`.

Payload: read this note together with `notes/IDENTIFICATION_BRIDGE.md`.

### Theorem EG4.3 (rigidity/transfer gate closure)
If bad limits are excluded and the endpoint lock is active, then `GGL_G4` and `GGL_G5` deliver the boundary object needed by the final margin.

## Current Instantiation

- rigidity gate: `GGL_G4`
- rigidity artifact key: `rho_rigidity`
- transfer gate: `GGL_G5`
- transfer artifact key: `jet_transfer`
- canonical equivalent: `bad-limit exclusion / endpoint identification`
- audit surface: `notes/IDENTIFICATION_BRIDGE.md` and `repro/certificate_runtime.json`
