---
topic: minmax-ricci-flow-extinction
type: topic
section: "6"
---

# Minimal spheres realize the width

Everything in the last three sections was preparation for one conclusion: the width is not an abstract infimum but a number attained by actual surfaces. Tightening makes near-maximal slices almost harmonic; the neck estimate keeps their energy from leaking; compactness turns them into harmonic spheres; the varifold statement says the convergence is convergence of surfaces. Packaged as a general saddle-point theorem, that is:

![[thm-minmax-harmonic-maps]]

Specialized to sphere sweepouts, it becomes the proposition the extinction argument consumes:

![[prop-minmax-minimal-spheres]]

The third conclusion is the one the evolution argument spends, and it is the reason the compactness theorem had to be proved for *every* near-maximal slice rather than for one minimizing sequence: the whole top of the sweepout is close, as a [[def-varifold|varifold]], to a union of minimal spheres, so an estimate for minimal spheres controls all of it at once. Closeness in that sense turns into agreement of curvature integrals — the quantitative bridge from *looks like minimal spheres* to *decays like minimal spheres*:

![[lem-varifold-quadratic-form]]
