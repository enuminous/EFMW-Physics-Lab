# Executed browser smoke tests (2026-10-27)

Headless Chromium/Playwright loaded the dependency-free HTML via an in-memory page and exercised the numeric inspection API. These are **local code execution smoke tests**, not independent verification of the physical model.

| Case | Steps | Grid | Candidate Gauss RMS | Candidate energy drift | RMS Higgs difference | Notes |
|---|---:|---:|---:|---:|---:|---|
| κ=0, pulse | 600 | 64² | 0 | −0.2592% | 0 | exact Higgs decoupling |
| κ=.30, pulse | 600 | 64² | 0 | −0.2015% | 0.04989 | nonzero candidate response |
| κ=0, stronger proxy source | 800 | 64² | 0 | −0.2121% | 0 | candidate χ dynamic, reference remains unchanged |
| κ=.30, quench | 450 | 64² | 8.9×10⁻¹⁶ | −0.0634% | 0.11988 | quench + gauge evolution |
| κ=.30, vortex pair | 450 | 64² | 4.9×10⁻¹⁶ | −0.1683% | 0.03078 | vortex pair + gauge evolution |
| κ=.30, pulse | 500 | 32² | 2.6×10⁻¹⁶ | −0.2518% | 0.03533 | coarse grid (L fixed) |
| κ=.30, pulse | 500 | 128² | 1.0×10⁻¹⁵ | −0.1435% | 0.05803 | fine grid (L fixed) |

**Caution:** Grid examples have different simulated final times because `Δt=0.085·Δx`. They do **not** establish convergence. Absolute energy drift does not prove symplectic accuracy or correct continuum physics.

Browser UI tests also exercised all three export actions (JSON, CSV, PNG), the root scalar tab, and mobile viewport overflow check (390px width, no horizontal overflow). No JavaScript console exceptions were observed during the tests.

Reproduce manually using `SMEFMWLab.pause()`, `SMEFMWLab.configure({kappa:0})`, `SMEFMWLab.advance(600)` and `SMEFMWLab.getState()` in your browser console. No runtime dependency is required.
