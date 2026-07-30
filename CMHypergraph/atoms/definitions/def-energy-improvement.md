---
id: fb3293386b35
type: definition
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §3, where the notation is introduced]]"
---

# Definition — the energy improvement of a slice

How much energy a single harmonic replacement can shed from a map: the
supremum, over small-energy ball collections, of the drop from replacing
on them. Zero exactly when the map is already harmonic.

## Statement

> [!definition] Energy improvement $e_{\sigma, \epsilon}(t)$
> For a map $\sigma(\cdot, t) : S^2 \to M$ and $\epsilon > 0$, the *energy improvement at scale $\epsilon$* is
> $$
> e_{\sigma, \epsilon}(t) \;=\; \sup_{\mathcal{B}} \Big( E(\sigma(\cdot,t)) - E\big[H(\sigma(\cdot,t), \mathcal{B})\big] \Big),
> $$
> the supremum over finite collections $\mathcal{B}$ of disjoint closed balls on each of which $\sigma(\cdot,t)$ has [[def-dirichlet-energy|energy]] at most $\epsilon$, and $H$ the [[def-harmonic-replacement|harmonic replacement]].

## Notes

> [!note]- Notes (click to expand)
> - $e_{\sigma,\epsilon}(t) \ge 0$, and $= 0$ iff $\sigma(\cdot,t)$ is already harmonic on every small ball (nothing to improve). It measures how far a slice is from harmonic, in energy.
> - It is the quantity the tightening tracks: [[lem-good-balls]] extracts, from the balls achieving it, collections that decrease energy by a definite fraction of $e_{\sigma,\epsilon}$; [[lem-nonharmonic-interval]] shows it varies slowly in $t$.
