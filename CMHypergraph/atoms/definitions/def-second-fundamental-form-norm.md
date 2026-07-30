---
id: d43dd4668d2c
type: definition
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §2]]"
  - "[[ref-leeriemannian|Lee, Introduction to Riemannian Manifolds, ch. 8]]"
---

# Definition — norm of the second fundamental form

The total bending at a point: the sum of squared principal curvatures
— the quantity whose integral measures how far a surface is from
totally geodesic.

## Statement

> [!definition] $|A|^2$
> Let $\Sigma \subset M$ be an [[def-immersion|immersed]] hypersurface with [[def-second-fundamental-form|second fundamental form]] $A$ and principal curvatures $\kappa_1, \dots, \kappa_{n-1}$. Then
> $$
> |A|^2 \;=\; \sum_{i,j} A_{ij}^2 \;=\; \kappa_1^2 + \cdots + \kappa_{n-1}^2 ,
> $$
> the [[def-tensor-norm|tensor norm]] of $A$ in the induced metric.

## Notes

> [!note]- Notes (click to expand)
> - $|A|^2 = 0$ exactly when $A \equiv 0$ — the surface is *totally geodesic* (ambient geodesics tangent to it stay in it).
> - For a surface in a $3$-manifold, $|A|^2 = \kappa_1^2 + \kappa_2^2$ and $\det A = \kappa_1 \kappa_2$, so $|A|^2 = H^2 - 2\det A$; when $H = 0$ this gives $\det A = -\tfrac12 |A|^2$ — the identity the minimal-surface area estimates consume.
