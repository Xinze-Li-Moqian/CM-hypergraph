---
id: 103ec6d25234
type: definition
references:
  - "[[ref-leeriemannian|Lee, Introduction to Riemannian Manifolds, ch. 2]]"
  - "[[ref-docarmo|do Carmo, ch. 7]]"
---

# Definition — Riemannian distance

The shortest-path distance the metric induces: measure every curve by the metric, take the infimum.

## Statement

> [!definition] Riemannian distance
> Let $(M, g)$ be a connected Riemannian manifold. The *length* of a piecewise-smooth curve $\gamma : [a, b] \to M$ is $L(\gamma) = \int_a^b |\gamma'(t)|_g \, dt$, and the *Riemannian distance* is
> $$
> d(x, y) \;=\; \inf \big\{ L(\gamma) : \gamma \text{ a piecewise-smooth curve from } x \text{ to } y \big\} .
> $$
> The *metric ball* is $B(x, r) = \{ y \in M : d(x, y) < r \}$.

## Notes

> [!note]- Notes (click to expand)
> - $d$ is a metric and induces the manifold topology; locally, geodesics realize the infimum. (Classical; consumed nowhere yet, so not carded.)
