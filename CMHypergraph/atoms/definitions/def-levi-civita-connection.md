---
id: 49305bf06128
type: definition
references:
  - "[[ref-leeriemannian|Lee, Introduction to Riemannian Manifolds, ch. 5]]"
  - "[[ref-docarmo|do Carmo, Riemannian Geometry, ch. 2]]"
---

# Definition — Levi-Civita connection

The metric's own way of differentiating vector fields: the one notion of
directional derivative that needs no extra choices, under which parallel
transport preserves lengths and angles.

## Statement

> [!definition] Levi-Civita connection
> Let $(M, g)$ be a Riemannian manifold. The *Levi-Civita connection* $\nabla$ is the connection on $TM$ that is
>
> 1. *metric*: $\ X\, g(Y, Z) = g(\nabla_X Y, Z) + g(Y, \nabla_X Z)$, and
> 2. *torsion-free*: $\ \nabla_X Y - \nabla_Y X = [X, Y]$.

## Notes

> [!note]- Notes (click to expand)
> - Existence and uniqueness are the fundamental theorem of Riemannian geometry; the connection is produced explicitly by the Koszul formula $2 g(\nabla_X Y, Z) = X g(Y,Z) + Y g(X,Z) - Z g(X,Y) + g([X,Y],Z) - g([X,Z],Y) - g([Y,Z],X)$.
