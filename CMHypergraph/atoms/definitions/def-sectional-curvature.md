---
id: 92bd10fc5db9
type: definition
references:
  - "[[ref-petersen|Petersen, Riemannian Geometry, ch. 3]]"
  - "[[ref-docarmo|do Carmo, Riemannian Geometry, ch. 4]]"
---

# Definition — sectional curvature

The curvature of a manifold, one plane at a time: what a
two-dimensional slice through a point would feel — positive like a
sphere, zero like a plane, negative like a saddle.

## Statement

> [!definition] Sectional curvature
> Let $(M, g)$ be a Riemannian manifold, $p \in M$, and $\sigma \subset T_p M$ a $2$-dimensional plane spanned by vectors $X, Y$. The *sectional curvature* of $\sigma$ is
> $$
> K(\sigma) \;=\; \frac{\langle \operatorname{Rm}(X, Y)\, Y,\; X \rangle}{|X|^2 |Y|^2 - \langle X, Y \rangle^2},
> $$
> where $\operatorname{Rm}$ is the [[def-curvature-tensor|curvature tensor]]; the value is independent of the chosen spanning vectors.

## Notes

> [!note]- Notes (click to expand)
> - Geometric meaning: $K(\sigma)$ is the Gauss curvature at $p$ of the surface swept out by the geodesics tangent to $\sigma$. The model values: $+1$ for the unit sphere, $0$ for Euclidean space, $-1$ for hyperbolic space.
> - The traces recover the coarser curvatures: the [[def-ricci-curvature|Ricci curvature]] in a direction is the sum of sectional curvatures over planes containing it, and the [[def-scalar-curvature|scalar curvature]] is twice the sum over an orthonormal set of planes.
> - In dimension $3$ — the dimension of this network — the sectional curvatures carry the *same* information as the full curvature tensor: there is no Weyl part. This is why pinching statements about sectional curvature control everything.
> - "Bounded sectional curvature" means $\sup_\sigma |K(\sigma)| < \infty$ — the standing completeness-grade hypothesis for flows on noncompact manifolds.
