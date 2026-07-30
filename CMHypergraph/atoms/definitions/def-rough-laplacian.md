---
id: 7eae1d0f8299
type: definition
references:
  - "[[ref-leeriemannian|Lee, Introduction to Riemannian Manifolds]]"
  - "[[ref-petersen|Petersen, Riemannian Geometry]]"
  - "[[ref-chowknopf|Chow & Knopf — the operator driving the curvature evolution equations]]"
---

# Definition — rough Laplacian

The Laplacian a connection alone can build: differentiate twice covariantly and trace — no exterior calculus, no sign conventions borrowed from topology.

## Statement

> [!definition] Rough Laplacian
> Let $(M, g)$ be a Riemannian manifold and $\nabla$ its [[def-levi-civita-connection|Levi-Civita connection]], extended to tensor fields. The *rough Laplacian* of a tensor field $T$ is the [[def-trace|trace]] of its second covariant derivative:
> $$
> \triangle\, T \;=\; \operatorname{tr}_g \nabla^2 T \;=\; g^{ij}\, \nabla_i \nabla_j\, T .
> $$

## Notes

> [!note]- Notes (click to expand)
> - On functions it is the ordinary [[def-laplacian|Laplacian]]; the point of the name is the extension to arbitrary tensor bundles.
> - "Rough" distinguishes it from the Hodge Laplacian on forms: the two differ by curvature terms (the Weitzenböck formula). Since the difference is zeroth-order, parabolic arguments — regularity, maximum principles — are insensitive to the choice, and the flow literature works with the rough one.
> - Where it works here: the reaction–diffusion equations of [[thm-curvature-evolution]] ($\partial_t \operatorname{Rm} = \triangle \operatorname{Rm} + Q$), and through them [[thm-shi-estimates]] and every maximum-principle comparison.
> - The extension of $\nabla$ to tensors and its iterates $\nabla^j$ are ground notions (see [[notation]]).
