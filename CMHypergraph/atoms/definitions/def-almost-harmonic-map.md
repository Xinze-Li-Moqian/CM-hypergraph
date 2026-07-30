---
id: dfc2e2d4ab8f
type: definition
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §5, Definition `d:ah`]]"
---

# Definition — almost harmonic map

A quantitative "nearly harmonic": on every small ball, the map is close
in energy to its own harmonic replacement — the property the tightened
sweepout slices satisfy, and the hypothesis the cylinder-decay analysis
runs on.

## Statement

> [!definition] $\nu$-almost harmonic map
> Let $\nu > 0$ and let $\mathcal{C}_{r_1, r_2} = [r_1, r_2] \times S^1$ be a flat cylinder, conformally the annulus $B_{e^{r_2}} \setminus B_{e^{r_1}} \subset \mathbb{R}^2$. A $W^{1,2}(\mathcal{C}_{r_1,r_2}, M)$ map $u$ is *$\nu$-almost harmonic* if for every finite collection $\mathcal{B}$ of disjoint closed balls in that annulus there is an energy-minimizing map $v$ on $\cup_{\mathcal{B}} \tfrac18 B$ agreeing with $u$ on $\cup_{\mathcal{B}} \tfrac18 \partial B$ with
> $$
> \int_{\cup_{\mathcal{B}} \frac18 B} |\nabla u - \nabla v|^2 \;\le\; \nu .
> $$

## Notes

> [!note]- Notes (click to expand)
> - This is CM's Definition `d:ah` (§5). It is exactly what the energy-decreasing map [[thm-energy-decreasing-map]] produces: after tightening, the near-maximal slices are $\nu$-almost harmonic with $\nu \to 0$ — hypothesis (B) of [[thm-almost-minimizing-compactness]].
> - Genuinely harmonic maps are $0$-almost harmonic. The definition measures the failure by the $W^{1,2}$ gap to the harmonic replacement, uniformly over all small balls.
