# Standard Model + EFMW Physics Laboratory

<!-- ENUMINOUS-UNIFIED-NAV:START -->
## Repository navigation

**eNuminous network:** [All public repositories](https://github.com/enuminous/EFMW/blob/main/REPOSITORY_NAVIGATION.md) · [EFMW](https://github.com/enuminous/EFMW) · [102 equations](https://github.com/enuminous/Monolithic_102_EFMW) · [Frozen Lean](https://github.com/enuminous/Monolithic-102-Zoo-Lean4) · [Zoo](https://github.com/enuminous/Tortoise) · [Papers](https://github.com/enuminous/papers) · [Quantum geometry](https://github.com/enuminous/Base888-Quantum-Geometry)

**This project:** [Repository home](https://github.com/enuminous/EFMW-Physics-Lab) · [Subject index](https://github.com/enuminous/EFMW/blob/main/REPOSITORY_NAVIGATION.md#fundamental-physics-cosmology-and-quantum-geometry)

<details open>
<summary><strong>On this page</strong></summary>

- [Launch](#launch)
- [What it does](#what-it-does)
- [First experiment](#first-experiment)
- [Files](#files)
- [EFMW source context](#efmw-source-context)
- [Connected physics research units](#connected-physics-research-units)


</details>

**Related repositories:** [Higgs-Gauge-Lab](https://github.com/enuminous/Higgs-Gauge-Lab) · [Standard-Model-Reduction](https://github.com/enuminous/Standard-Model-Reduction) · [Quantum-Gravity](https://github.com/enuminous/Quantum-Gravity) · [QST](https://github.com/enuminous/QST) · [Base888-Quantum-Geometry](https://github.com/enuminous/Base888-Quantum-Geometry) · [EFMW](https://github.com/enuminous/EFMW) · [papers](https://github.com/enuminous/papers)

> **Evidence boundary:** A link between projects is navigation, not an assertion of proven equivalence, experimental validation, or shared authorship. See each repository’s own status and review notes.
<!-- ENUMINOUS-UNIFIED-NAV:END -->


An **offline, single-file, GitHub Pages-ready** classical lattice field research laboratory. The working application is **`index.html`**, with no external dependencies.

## Launch

Open `index.html` in a browser. For GitHub Pages, upload everything to the repository root and enable **Settings → Pages → Deploy from a branch → main → /(root)**. This archive is flat: no nested directory needs moving.

## What it does

- Runs two deterministic, matched **2+1D classical Abelian–Higgs** lattice simulations (A and B).
- Adds a **candidate EFMW-inspired real root scalar** χ to simulation B, and an *independently proposed, hypothetical* Higgs–χ portal coupling `κ`.
- Shows synchronized energy, Higgs magnitude, scalar phase, gauge flux and χ panels, plus a signed B−A field.
- Provides evolution diagnostics, a central-row Fourier spectrum, a bounded and qualified Zoo-style numerical audit, and JSON/CSV/PNG export.
- Supports 32², 64² and 128² grids with fixed physical box length L=64, three initial conditions, deterministic random seed, dynamic controls, and velocity-Verlet time integration.

**Important:** This is **not** a full Standard Model (no SU(2), SU(3), dynamical fermions or QCD), a quantum field theory simulation, a gravity model or verification of EFMW as new physics. Do not interpret color-map patterns as direct evidence of quantum diffraction or discovery.

## First experiment

1. Start with **Radial pulse**, choose **Energy density** or **Higgs magnitude**.
2. Observe the two matched runs and B−A difference while κ=0.30.
3. Move **κ to 0** and **Reset**. The Higgs/gauge fields must remain identical; χ can still evolve freely. The `Decoupling at κ=0` audit should PASS.
4. Set **damping γ = 0**; run at least 30 time steps and inspect energy drift and Gauss residual.
5. Change to 32², 64², 128² at fixed L and compare time-aligned observable traces (this app does **not** automatically claim convergence).
6. Export JSON, CSV and PNG for outside review.

## Files

- `index.html`: complete standalone executable application.
- `MODEL.md`: equations, assumptions, scope and numerics.
- `VALIDATION.md`: checks and unperformed obligations.
- `LICENSE_NOTICE.md`: redistribution note; no license asserted without owner selection.

## EFMW source context

- [Frozen EFMW-Lagrangian C1 candidate](https://github.com/enuminous/EFMW-Lagrangian/blob/main/candidate/CANDIDATE.md)
- [Physical obligations](https://github.com/enuminous/EFMW-Lagrangian/blob/main/docs/PHYSICAL_OBLIGATIONS.md)
- [EFMW root and recursive-coherence candidate](https://github.com/enuminous/papers/blob/main/EFMW-F001-Recursive-Coherence-Dynamics.md)

The lab's *new portal* is an exploratory hypothesis for computational comparison, **not** an EFMW-derived law or an implementation of the C1 action family.

<!-- ENUMINOUS-RESEARCH-CHAIN:START -->
## Connected physics research units

**Established-theory reconstructions and baseline laboratories:** [Standard-Model-Reduction](https://github.com/enuminous/Standard-Model-Reduction) · [Higgs-Gauge-Lab](https://github.com/enuminous/Higgs-Gauge-Lab) · [EFMW-Physics-Lab](https://github.com/enuminous/EFMW-Physics-Lab)

**Proposed quantum-geometry bridge:** [Base888-Quantum-Geometry](https://github.com/enuminous/Base888-Quantum-Geometry) · [QST-001](https://github.com/enuminous/Quantum-Gravity/blob/main/QST-001.md) · [QST-002](https://github.com/enuminous/QST/blob/main/QST-002.md)

**EFMW definitions, pressure-cycle model, and spacetime investigations:** [Canonical 102 equations](https://github.com/enuminous/Monolithic_102_EFMW) · [Frozen Lean review](https://github.com/enuminous/Monolithic-102-Zoo-Lean4) · [RHC-001: Rahasya pressure-cycle formalization](https://github.com/enuminous/papers/blob/main/RHC-001-EFMW-Rahasya-Pressure-Cycle-Formalization.md) · [EFMW-Lagrangian](https://github.com/enuminous/EFMW-Lagrangian) · [Cosmology](https://github.com/enuminous/Cosmology)

> **Interpretation:** Cross-links represent research dependencies and comparisons. The Standard Model and continuum gravity are inputs in current QST calculations; their emergence from Base888 and the physical status of the pressure cycle remain **UNRESOLVED**.
<!-- ENUMINOUS-RESEARCH-CHAIN:END -->
