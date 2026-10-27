# Standard Model + EFMW Physics Laboratory

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
