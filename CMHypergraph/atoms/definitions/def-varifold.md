---
id: 33c61d3c595a
type: definition
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §3 and §4]]"
  - "the varifold framework is Almgren–Allard, exposition in Colding–De Lellis"
---

# Definition — varifold and varifold distance

A surface remembered only as mass with directions: forget the
parametrization, keep how much area sits at each point pointing which
way — the weak notion of surface under which min-max sequences
converge.

## Statement

> [!definition] Varifold; varifold distance
> A *$2$-varifold* in $M$ is a Radon measure $V$ on the [[def-tangent-plane|Grassmann bundle]] $G_2(M)$ — the bundle whose fibre over $x \in M$ is the set of $2$-planes in $T_x M$. An [[def-immersion|immersed]] surface $\Sigma$ induces the varifold $V_\Sigma(A) = \operatorname{area}\{x \in \Sigma : (x, T_x\Sigma) \in A\}$: its area measure, tagged with the tangent plane at each point.
>
> The *varifold distance* is any metric inducing the weak-$*$ topology on varifolds of bounded mass: $V_k \to V$ when $\int f \, dV_k \to \int f \, dV$ for every continuous compactly supported $f$ on $G_2(M)$.

## Notes

> [!note]- Notes (click to expand)
> - The point is what it *forgets* and what it *keeps*. It forgets the map — multiplicity, parametrization, and small necks collapse — so a sequence of surfaces with wildly varying parametrizations can still converge. It keeps area-with-direction, so any quantity of the form $\int_\Sigma \big[\operatorname{tr} F - F(\mathbf n, \mathbf n)\big]$, a function of the tangent plane, is continuous under the convergence.
> - That last property is exactly what [[prop-minmax-minimal-spheres]] conclusion 3 delivers to [[thm-width-evolution]]: a near-maximal slice, being varifold-close to a union of minimal spheres, has its curvature integrals close to theirs — so the area-decay estimate for the spheres transfers to the slice.
> - Proof debt of the *compactness* that makes this useful (bounded mass gives a convergent subsequence) is Allard's theory; carded here only as the target notion, its analytic development left to the harmonic-map chapter.
