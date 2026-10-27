# Numerical validation and evidence boundaries

The inline Monolithic Zoo panel deliberately separates restricted numerical checks from physical claims.

| Check | Runtime threshold | Scope |
|---|---|---|
| Finite fields | All sampled energy and Gauss values finite | Elementary sanity check only |
| Gauss constraint | max RMS < 1e-5 | Discrete temporal-gauge diagnostic |
| Total energy drift | max |ΔE/E0| < 1% after >=30 steps, damping=0 | Weak finite-duration sanity bound; NOT a convergence proof |
| κ=0 decoupling | RMS difference in normalized Higgs magnitudes < 1e-10 | Checks expected reduction to reference |
| Resolution convergence | UNRESOLVED | Requires paired fixed-time multi-grid analysis with error rates |
| EFMW source physics | UNRESOLVED | E/P units, sources, transformation law and backreaction undefined |
| Entire Standard Model, quantum, GR | N/A | Missing solvers and degrees of freedom |
| Physical EFMW validation | UNRESOLVED | Independent empirical comparison required |

These tests run on the client's machine; their outcome depends on parameters and numerical state. N/A is not silently counted as a PASS.

## Suggested independent experiments

1. Compare solutions at fixed physical times across grids N=32,64,128, reducing timestep with spacing and extracting observable norms. Verify expected asymptotic order; more resolution alone does not prove convergence.
2. Run κ=0 against reference for each preset; test both gauge and Higgs fields bitwise as well as magnitude if conducting an external audit.
3. Compare energy drift versus Δt with damping and all time-dependent driving disabled. The fixed source potential must be included.
4. Construct an explicit gauge transformation on link and site variables and check gauge-invariant observable agreement and Gauss-law preservation.
5. Verify FDTD lattice dispersion against linearization about a stable Higgs vacuum, distinguish periodic boundary interference from continuum physics.
6. Replace arbitrary EFMW proxy βJ with a dimensionally consistent source model independently specified before viewing simulation outcomes.
7. Register an observable, benchmark data and physical null models before interpreting any nonzero candidate deviation as evidence of new physics.

## Claim boundaries

- A more interesting interference pattern is **not** quantum diffraction or EFMW verification.
- Lean certificates about finite equations are **not** empirical proof.
- C1 source/current/stress mismatches and stability questions are **not solved** by implementing this separate scalar portal.
- Candidate physics must be shown alongside the unchanged reference and labeled as a hypothesis.
