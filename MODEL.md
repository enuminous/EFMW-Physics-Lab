# Physical and computational model (v1.0)

## Scope and convention

A 2+1-dimensional classical **noncompact U(1)** gauge–Higgs model in temporal gauge A₀=0 and signature (+−−). Unit system c = ℏ = 1. Space is a periodic N×N box of side L=64 with spacing Δx=L/N. This is a deliberate reduction of the Standard Model gauge/Higgs structure, **not the full SM Higgs doublet**.

Let Φ be a complex U(1)-charged scalar, Aᵢ an Abelian gauge potential, χ a proposed extra real scalar and J(x) an external, fixed, zero-mean scalar source. The computational actions are

```
L_A = −¼ FμνF^μν + (DμΦ)* D^μΦ − λ(|Φ|²−v²/2)²
L_B = L_A + ½∂μχ ∂^μχ − (κ/2)χ²|Φ|² − βJχ
DμΦ = (∂μ − i g Aμ)Φ
```

Here κ >= 0 is a **hypothetical new portal**, not established EFMW, and βJ is implemented directly with a dimensionless slider. For χ, the Euler–Lagrange equation is

```
χ̈ = ∇²χ − κχ|Φ|² − βJ
```

At κ=0 this is the flat-space source-driven EFMW *root-equation form* (with c=1):

```
∇²χ − ∂²χ/∂t² = βJ.
```

In the historical EFMW expression βJ = (4π/c²)(E+cP), whose E and P **physical definitions and units remain open**. Our βJ is **NOT a scientific identification of those quantities**. The prescribed source uses a fixed spatial Gaussian with its lattice mean subtracted, multiplied by the source slider. Its static potential term is included in the candidate energy; source choice is a numerical convenience.

The Higgs evolution in B adds the force `−(κ/2) χ² Φ` while the root equation has `−κ χ|Φ|²`; these factors reflect the complex-Higgs kinetic normalization and one shared action. Setting κ=0 decouples Higgs/gauge evolution exactly; B can retain an independently evolving χ.

## Discretization

- Uᵢ(x)=exp(−i g Δx Aᵢ(x)) for gauge-covariant neighbor transport.
- `D_i D_i` approximated with nearest-neighbor gauge-transported second differences divided by Δx².
- Magnetic field `B_z = (A_y(x+e_x)−A_y(x)−A_x(x+e_y)+A_x(x))/Δx`.
- χ spatial Laplacian is the standard five-point centered second difference.
- Velocity Verlet in time with `Δt=0.085 Δx`, and post-step exponential damping when γ > 0.
- Higgs/gauge initial data are **identical in A and B**, with zero initial canonical velocities and electric fields; candidate χ has a fixed, disclosed two-lobe Gaussian perturbation.
- Quench random numbers are deterministic using xorshift32 initialized with seed 20261027. Changing resolution uses a consistent pseudorandom stream, not a physically identical continuum random field.

## Energy and interpretation

A and B heatmaps labeled **Energy density** plot only the *Higgs–gauge subsystem* density to permit direct difference maps. Total candidate energy is instead computed as

```
E_B = E_Higgs + ½ χ̇² + ½ |∇χ|² + (κ/2)χ²|Φ|² + βJχ.
```

The finite-difference gradient energy is measured using forward gauge links and forward χ differences. χ energy may be negative locally due to the static-source potential, despite the total being conserved in suitable closed configurations. Drift is shown as a percentage relative to t=0.

The **phase** map is gauge dependent and its signed difference is not a gauge-invariant physical observable. The **Fourier chart** computes the direct discrete Fourier transform of the Higgs *magnitude along the center row*, not the full two-dimensional power spectrum. Zero-frequency mode is removed. Difference maps auto-normalize by the current maximum difference; a bright map can represent an extremely small absolute deviation.

## Known omissions

No SU(2)/SU(3) Yang–Mills dynamics, Higgs doublet, fermion spinors, Yukawa backreaction, QCD theta term, quantum path integrals, renormalization, dynamic metric/GR, EFMW C1 11-sector system, EM source identification, or empirical EFMW validation. A code run or a PASS on an internal audit is not a physical proof.
