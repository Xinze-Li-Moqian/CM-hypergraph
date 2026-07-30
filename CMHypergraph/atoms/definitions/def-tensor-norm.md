---
id: db280061e60c
type: definition
references:
  - "[[ref-leeriemannian|Lee, Introduction to Riemannian Manifolds, ch. 2]]"
  - "[[ref-petersen|Petersen, Riemannian Geometry, ch. 1]]"
---

# Definition — tensor norm

The metric measures more than vectors: it grades every tensor at every
point by one number — the root sum of squares of its components in any
orthonormal frame.

## Statement

> [!definition] Tensor norm
> Let $(V, g)$ be a finite-dimensional inner-product space. The inner product extends to each space of tensors on $V$: with respect to any orthonormal basis, $\langle S, T \rangle$ is the sum over all indices of the products of components, and
> $$
> |T|_g \;=\; \sqrt{\langle T, T \rangle}
> $$
> — the value independent of the chosen orthonormal basis. On a Riemannian manifold $(M, g)$, the *pointwise tensor norm* $|T|_g$ of a tensor field $T$ is this norm applied at each point, with $V = T_pM$ and covectors measured by duality.

## Notes

> [!note]- Notes (click to expand)
> - Equivalently: raise every lower index with $g^{-1}$ and contract against a copy of $T$ — the coordinate-free form of "sum of squared components".
> - Every norm appearing in the curvature bounds of this network is an instance: $|{\operatorname{Rm}}| \le r^{-2}$ in noncollapsing, $|{\operatorname{Rm}}| \le 1$ in normalization, $|\nabla f|$ in the entropy, $|\nabla_h^j T|_h$ in closeness.
