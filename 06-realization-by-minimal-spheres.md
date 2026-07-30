---
topic: minmax-ricci-flow-extinction
type: topic
section: "6"
---

# Minimal spheres realize the width

Everything in the last three sections was preparation for one conclusion: the width is not an abstract infimum but a number attained by actual surfaces. Tightening makes near-maximal slices almost harmonic; the neck estimate keeps their energy from leaking; compactness turns them into harmonic spheres; the varifold statement says the convergence is convergence of surfaces. Packaged as a general saddle-point theorem, that is:

![[thm-minmax-harmonic-maps]]

Why this needs proving at all is worth a sentence. The width is a min-max value: for each sweepout take the largest energy along it, then take the smallest such maximum over all sweepouts in the class. Nothing about that construction produces a surface. The infimum could be approached by families that get worse and worse — spikier, thinner, more concentrated — and never settle on anything. What the theorem says is that they cannot: any minimizing sequence of sweepouts has, at its near-maximal slices, subsequences converging to genuine harmonic spheres.

Specialized to sphere sweepouts, it becomes the proposition the extinction argument consumes:

![[prop-minmax-minimal-spheres]]

Three features of that statement are doing work later, and none is a technicality.

**The width is a sum, not a single area.** Energy can concentrate: as the sweepouts tighten, a slice can develop a region where energy piles up at smaller and smaller scale, and rescaling that region conformally produces a sphere of its own. The limit is therefore a finite collection $u_0, \dots, u_m$ of branched minimal spheres, and the width is the total of their energies. This is not a defect of the proof. It is what the geometry does, and the argument is built to survive it: the decay estimate of the next section is linear in the collection, so an inequality per sphere adds up to an inequality for the width.

**The spheres are branched, and minimal rather than merely harmonic.** A harmonic map from $S^2$ into a Riemannian manifold is automatically conformal away from finitely many points, and a conformal harmonic map is a branched minimal immersion — its image is a minimal surface with finitely many singular points. So the area and the energy of each $u_i$ agree, which is what allows an energy statement about sweepouts to be attacked with an area estimate about surfaces.

**Every near-maximal slice is close to the limit, not just a chosen subsequence.** This is the third conclusion, and it is the one the evolution argument spends. It is also the reason the compactness theorem had to be proved for *every* near-maximal slice rather than for one minimizing sequence: the whole top of the sweepout is close, as a [[def-varifold|varifold]], to a union of minimal spheres, so an estimate for minimal spheres controls all of it at once. Without it one would know that some slices resemble minimal spheres and have no way to bound the ones that do not.

Closeness in that sense turns into agreement of curvature integrals — the quantitative bridge from *looks like minimal spheres* to *decays like minimal spheres*:

![[lem-varifold-quadratic-form]]

Varifold closeness is weak: it says the surfaces agree when tested against continuous functions, and says nothing directly about their curvature. The lemma is what upgrades it, and it is the last step before the estimate. The index bound — at most one — is what makes the upgrade available, since it limits how badly a slice can fail to be stable and so how far its second-variation data can drift from the limit's.
