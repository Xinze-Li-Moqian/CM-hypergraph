---
id: c306c5b4bf85
type: definition
references:
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, Ricci Flow and the Poincaré Conjecture, ch. 3]]"
  - "[[ref-bamler-surgery|Bamler, Ricci flow with surgery, §2.7]]"
---

# Definition — maximal flow

The longest life a flow can have from a given start: the flow that
every other flow with the same initial metric is a piece of.

## Statement

> [!definition] Maximal flow
> Let $(M, g_0)$ be a Riemannian manifold. A [[def-ricci-flow|Ricci flow]] $g(t)$, $t \in [0, T)$ with $T \in (0, \infty]$ and $g(0) = g_0$, is the *maximal flow* of $g_0$ if every Ricci flow $h(t)$, $t \in [0, T')$, with $h(0) = g_0$ satisfies $T' \le T$ and $h(t) = g(t)$ for all $t \in [0, T')$. The time $T$ is the *maximal time* of $g_0$.

## Notes

> [!note]- Notes (click to expand)
> - The definition is a universal property, so the maximal flow is unique as soon as it exists: two maximal flows of the same $g_0$ restrict to each other.
> - Existence on a closed manifold — together with the fact that a finite maximal time is always a curvature blow-up — is [[thm-short-time-existence]]; the definition itself promises neither.
