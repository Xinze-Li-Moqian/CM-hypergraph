---
id: c5bcbb9f857e
type: definition
references:
  - "[[ref-docarmo|do Carmo, Riemannian Geometry]]"
  - "[[ref-coldingminicozzi|Colding & Minicozzi, Appendix A]]"
---

# Definition — conformal map

An angle-preserving map: it may stretch, but the stretch is the same in
every direction at each point — so infinitesimal circles stay circles.

## Statement

> [!definition] Conformal map
> A smooth map $f : (N, h) \to (M, g)$ between Riemannian manifolds is *conformal* if there is a positive function $\lambda$ on $N$ with
> $$
> f^* g \;=\; \lambda^2\, h ,
> $$
> i.e. $f$ multiplies all lengths at a point by the same factor $\lambda(p)$. A *conformal diffeomorphism* is a conformal map that is a [[def-diffeomorphism|diffeomorphism]].

## Notes

> [!note]- Notes (click to expand)
> - Equivalently, $f$ preserves angles between tangent vectors. In dimension two this is a large and flexible class — every Riemann surface has many conformal automorphisms — which is what makes the balancing argument of [[lem-hersch-balancing]] possible.
> - The conformal automorphisms of the round $S^2$ form the Möbius group $\mathrm{PSL}(2,\mathbb{C})$; a *branched conformal immersion* ([[def-branched-immersion]]) is conformal where it is an immersion.
