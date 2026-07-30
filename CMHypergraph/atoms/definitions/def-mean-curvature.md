---
id: 726f2f6d6e71
type: definition
references:
  - "[[ref-docarmo|do Carmo, Riemannian Geometry, ch. 6]]"
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §1]]"
---

# Definition — mean curvature

The average bending of a surface: the trace of its second fundamental
form — and the gradient of area, so its vanishing marks the critical
surfaces.

## Statement

> [!definition] Mean curvature
> Let $\Sigma \subset M$ be an [[def-immersion|immersed]] hypersurface with [[def-second-fundamental-form|second fundamental form]] $A$ and principal curvatures $\kappa_1, \dots, \kappa_{n-1}$. The *mean curvature* is
> $$
> H \;=\; \operatorname{tr} A \;=\; \kappa_1 + \cdots + \kappa_{n-1} .
> $$

## Notes

> [!note]- Notes (click to expand)
> - $H$ is the first variation of area: moving $\Sigma$ with normal speed $\phi$ changes area at rate $-\int_\Sigma H \phi$. So $H$ points in the direction of fastest area decrease, and $H \equiv 0$ is the Euler–Lagrange equation of the area functional — the defining condition of a [[def-minimal-surface|minimal surface]].
> - Convention: some authors divide by $n-1$ to take the literal mean; here $H$ is the unnormalized trace, as in the surface literature this network follows.
