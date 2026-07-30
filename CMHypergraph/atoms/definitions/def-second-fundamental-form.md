---
id: 1ba4b1f06bde
type: definition
references:
  - "[[ref-docarmo|do Carmo, Riemannian Geometry, ch. 6]]"
  - "[[ref-leeriemannian|Lee, Introduction to Riemannian Manifolds, ch. 8]]"
---

# Definition — second fundamental form

How a surface curves inside its ambient space: the normal component of
how tangent directions turn — the extrinsic bending that intrinsic
geometry cannot see.

## Statement

> [!definition] Second fundamental form
> Let $\Sigma \subset M$ be an [[def-immersion|immersed]] hypersurface with unit normal $\mathbf{n}$, and $\nabla$ the ambient [[def-levi-civita-connection|Levi-Civita connection]]. The *second fundamental form* is the symmetric bilinear form on $T\Sigma$
> $$
> A(X, Y) \;=\; \langle \nabla_X Y, \, \mathbf{n} \rangle , \qquad X, Y \in T\Sigma .
> $$
> Its eigenvalues with respect to the induced metric are the *principal curvatures* $\kappa_1, \dots, \kappa_{n-1}$.

## Notes

> [!note]- Notes (click to expand)
> - Symmetry is torsion-freeness of $\nabla$: $A(X,Y) - A(Y,X) = \langle \nabla_X Y - \nabla_Y X, \mathbf n\rangle = \langle [X,Y], \mathbf n\rangle = 0$ since $[X,Y]$ is tangent.
> - It measures purely extrinsic data: a plane rolled into a cylinder has $A \neq 0$ but is intrinsically flat. The [[lem-gauss-equation|Gauss equation]] is exactly the bookkeeping that separates $A$ from the intrinsic curvature.
> - The trace and squared norm of $A$ are the [[def-mean-curvature|mean curvature]] and $|A|^2$ (see [[def-second-fundamental-form-norm]]).
