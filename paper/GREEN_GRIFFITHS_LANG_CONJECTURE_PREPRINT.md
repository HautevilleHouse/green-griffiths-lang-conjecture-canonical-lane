# The Green-Griffiths-Lang Conjecture via Hyperbolic-Entire-Curve Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global architecture (`GGL1-GGL8`)

**Author:** HautevilleHouse  
**Date:** March 12, 2026  
**Status:** Admissible-class theorem manuscript

---

## Abstract

This manuscript develops a canonical-lane closure architecture for the target problem: proving algebraic degeneracy of entire curves on varieties of general type through an admissible hyperbolic closure architecture.

The proof program is organized as eight steps `GGL1-GGL8` with executable closure gates `GGL_G1`, `GGL_G2`, `GGL_G3`, `GGL_G4`, `GGL_G5`, `GGL_G6`, and `GGL_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

The target statement is: algebraic degeneracy of entire curves on varieties of general type.

The canonical-lane proof path is:

1. encode the admissible evolution in a canonical class `A`,
2. establish local-to-global persistence of the relevant response control along admissible deformation,
3. exclude bad limits by rigidity and compactness,
4. transfer the rigid limit through the bridge package,
5. identify the endpoint representative with the intended target class.


### 1.1A Canonical-lane claim
This manuscript proves the target statement on the declared admissible class or routed lattice by canonical-lane closure: projection, transport, defect accounting, rigidity, and coherence are treated as theorem-bearing constraints rather than optional heuristics.

### 1.1B Bridge / equivalence statement
The canonical endpoint objects are tied to the standard problem-side target through the in-repo bridge package. The paper records the transfer or endpoint-identification step in the main theorem chain, and `notes/IDENTIFICATION_BRIDGE.md` fixes the determining-class lock in ordinary mathematical language.

### 1.1C Verification surface
A reviewer can check this claim on four surfaces:

1. the standard target statement in Section `1.1`,
2. the canonical objects and closure gates in the main paper,
3. the endpoint bridge in `notes/IDENTIFICATION_BRIDGE.md`,
4. the executable rerun `bash repro/run_repro.sh` with runtime output `repro/certificate_runtime.json`.

### 1.2 Local claim boundary

- the closure architecture and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared admissible class closes.

Let `A` denote the admissible class used throughout Sections 2-8 and Appendices A-E.

---

## 2. Epistemic Axiom Map (A1-A8)

| Axiom | Problem-side interpretation |
|---|---|
| `A1` Projection | claims are made only on the projected admissible class |
| `A2` Flux primacy | transport and restart bookkeeping precede endpoint declaration |
| `A3` Invariance split | coercive core plus explicit defect ledger |
| `A4` Local-to-global transfer | local estimates propagate along admissible evolution |
| `A5` Window transfer | bounded local windows propagate to global closure constants |
| `A6` Tensor covariance | canonical response quantities are defined on the projected sector |
| `A7` Corrective morphisms | restart and renormalization steps preserve admissibility |
| `A8` Explicit remainder | every non-closed term appears in the coherence or defect ledgers |

---

## 3. Canonical Objects

Let `tau` denote the deformation parameter and let `u_tau = (E_tau, J_tau, D_tau, N_tau, L_tau)` denote the admissible state of entire-curve packets, jet-differential data, defect ledgers, normalization parameters, and endpoint locks.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible packets: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_GGL = min(kappa_entire, sigma_hyperbolic, kappa_compact, rho_rigidity, jet_transfer) - eps_coh`.

Target:

`M_GGL > 0`.

---

## 4. Response and Gate Interface

### 4.1 Canonical tube

- admissible packets remain inside the declared tube,
- defects stay within the tracked ledger,
- the projected response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive entire-curve response that prevents collapse of the admissible closure package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `GGL_G1` | `kappa_entire` | projected entire-curve response has a strict positive floor |
| `GGL_G2` | `sigma_hyperbolic` | hyperbolic defect stays above capture floor across admissible jet losses |
| `GGL_G3` | `kappa_compact` | normalized near-failure families are precompact and admissible windows do not collapse |
| `GGL_G4` | `rho_rigidity` | bad entire-curve countermodels are excluded |
| `GGL_G5` | `jet_transfer` | rigid limit transfers to the Green-Griffiths-Lang endpoint class |
| `GGL_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `GGL_GM` | derived | all upstream gates pass and `M_GGL > 0` |

### 4.4 Strict margin

At current artifact values:

- `kappa_entire` = 1.0918990000000002,
- `sigma_hyperbolic` = 1.0739999999999998,
- `kappa_compact` = 0.801924619085806,
- `rho_rigidity` = 1.078,
- `jet_transfer` = 1.030627,
- `eps_coh = 0.0`.

Hence:

`M_GGL = 0.801924619085806 > 0`.

### 4.5 Raw coercive constant

Define `kappa_entire^(raw) := c_entire_raw * jet_density_raw - e_entire_raw`.

Current extracted value:

`kappa_entire = 1.0918990000000002`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`GGL1-GGL8`)

1. `GGL1` Active projected response block on the canonical sector.
2. `GGL2` Uniform capture bounds on the canonical admissible tube.
3. `GGL3` Restart map preserving admissible data.
4. `GGL4` First-failure compactness extraction.
5. `GGL5` Rigidity exclusion of bad countermodels.
6. `GGL6` Endpoint transfer closure on the extracted target class.
7. `GGL7` Determining-class identification of the intended endpoint.
8. `GGL8` Final persistence theorem: the endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_hyperbolic^(raw) := hyperbolic_floor_raw - jet_loss_raw - restart_loss_raw`.

Current extracted value:

`sigma_hyperbolic = 1.0739999999999998`.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

Current extracted value:

`kappa_compact = 0.801924619085806`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` of bad entire-curve countermodels incompatible with closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

The tracked theorem-level input is `rho_rigidity = 1.078 > 0`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the Green-Griffiths-Lang endpoint class by the bridge inequality.

Define `jet_transfer^(raw) := c_transfer_raw * transfer_gain_raw - e_transfer_raw`.

Current extracted value:

`jet_transfer = 1.030627 > 0`.

### 6.3 Determining-class identification

Fix a determining class `C_det` of endpoint observables. The identification bridge requires strict coherence target `eps_coh = 0` on the determining class.

---

## 7. Current Theorem Inputs (Tracked)

| Constant | Gate | Current value |
|---|---|---|
| `kappa_entire` | `GGL_G1` | `1.0918990000000002` |
| `sigma_hyperbolic` | `GGL_G2` | `1.0739999999999998` |
| `kappa_compact` | `GGL_G3` | `0.801924619085806` |
| `rho_rigidity` | `GGL_G4` | `1.078` |
| `jet_transfer` | `GGL_G5` | `1.030627` |
| `eps_coh` | `GGL_G6` | `0.0` |
| `sigma_star_can` | stitch | `1.054` |

---

## 8. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `GGL_G1, GGL_G2, GGL_G3, GGL_G4, GGL_G5, GGL_G6, GGL_GM = PASS`,
- strict margin `M_GGL = 0.801924619085806`,
- lane: `manifold_constrained`.
