---
id: da242a0ffc1a
type: definition
references:
  - "[[ref-leeriemannian|Lee, Introduction to Riemannian Manifolds, ch. 7]]"
  - "[[ref-docarmo|do Carmo, ch. 4]]"
---

# Definition — curvature tensor

The failure of second covariant derivatives to commute: carry a vector
around a tiny parallelogram by parallel transport and it comes back
rotated — $\operatorname{Rm}$ records that rotation.

## Statement

> [!definition] Curvature tensor
> Let $(M, g)$ be a Riemannian manifold with [[def-levi-civita-connection|Levi-Civita connection]] $\nabla$. The *curvature tensor* is
> $$
> \operatorname{Rm}(X, Y)Z \;=\; \nabla_X \nabla_Y Z - \nabla_Y \nabla_X Z - \nabla_{[X,Y]} Z ,
> $$
> and $|\operatorname{Rm}|$ is its norm with respect to $g$.

## Notes

> [!note]- Notes (click to expand)
> - **Picture.**
>   ![[curvature-holonomy.svg]]
> - $\operatorname{Rm}(X, Y)$ is the infinitesimal holonomy around the $XY$-parallelogram; the metric is flat (locally Euclidean) exactly when $\operatorname{Rm} \equiv 0$.
