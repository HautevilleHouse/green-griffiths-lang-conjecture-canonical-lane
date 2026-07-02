# Reviewer Map

## Claim Scope

- Canonical-lane claim: inside the `manifold_constrained` lane, if the theorem chain in this repository holds and the guard certificate passes, the repository-level closure claim is satisfied.
- Standard target claim: carried by the in-repo bridge theorems tying the lane to the target statement.

## Theorem Dependency Chain

1. `EG1`: coercive response and active control floor.
2. `EG2`: capture and admissible continuation.
3. `EG3`: compactness and no-collapse spacing.
4. `EG4`: rigidity and transfer.
5. Identification bridge: strict coherence on the determining class.
6. Scalar closure: `GGL_G1`, `GGL_G2`, `GGL_G3`, `GGL_G4`, `GGL_G5`, `GGL_G6`, `GGL_GM` all `PASS`.

Primary files:

- `paper/GREEN_GRIFFITHS_LANG_CONJECTURE_PREPRINT.md`
- `notes/EG1_public.md`
- `notes/EG2_public.md`
- `notes/EG3_public.md`
- `notes/EG4_public.md`
- `notes/IDENTIFICATION_BRIDGE.md`

## Closure Gates

| Gate | Constant | Description |
|------|----------|-------------|
| `GGL_G1` | `kappa_entire` | projected entire-curve response has a strict positive floor |
| `GGL_G2` | `sigma_hyperbolic` | hyperbolic defect stays above capture floor across admissible jet losses |
| `GGL_G3` | `kappa_compact` | normalized near-failure families are precompact and admissible windows do not collapse |
| `GGL_G4` | `rho_rigidity` | bad entire-curve countermodels are excluded |
| `GGL_G5` | `jet_transfer` | rigid limit transfers to the Green-Griffiths-Lang endpoint class |
| `GGL_G6` | `eps_coh` | strict coherence / identification closure |
| `GGL_GM` | derived | final strict margin |

## Falsification Conditions

- `repro/certificate_runtime.json` has any non-`PASS` gate.
- `lane.active_lane != "manifold_constrained"`.
- `all_pass != true`.
- Any manifest hash mismatch under `repro/repro_manifest.json`.
- A certified counterexample to any EG theorem statement used in the paper.
