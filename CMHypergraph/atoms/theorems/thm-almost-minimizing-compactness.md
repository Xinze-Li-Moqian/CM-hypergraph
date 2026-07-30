---
id: 8c0e2ac4b13f
type: theorem
rigor: outline
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, Proposition in §2, proof §5]]"
---

# Theorem — Compactness of almost energy-minimizing maps

The limit step of the min-max: a sequence of spheres that are nearly
area-maximal and nearly energy-minimizing on small balls converges, in
the bubble-tree sense, to a finite collection of harmonic spheres.

## Statement

> [!theorem] Compactness of almost-minimizing maps
> Let $\epsilon_0, E_0 > 0$ with $\epsilon_0 < \epsilon_{SU}$ (the Sacks–Uhlenbeck constant), and let $u^j : S^2 \to M$ be $C^0 \cap W^{1,2}$ maps with $E(u^j) \le E_0$ satisfying: (A) $\operatorname{Area}(u^j) > E(u^j) - 1/j$; and (B) on every finite collection $\mathcal{B}$ of disjoint balls with $\int_{\cup\mathcal{B}}|\nabla u^j|^2 < \epsilon_0$, the [[def-dirichlet-energy|energy]] of $u^j$ on $\tfrac18\mathcal{B}$ exceeds its [[def-harmonic-replacement|harmonic replacement]]'s by at most $1/j$. Then a subsequence *[[def-bubble-convergence|bubble]]-converges* to a collection of branched [[def-conformal-map|conformal]] [[def-minimal-surface|minimal]] $2$-spheres $u_0, \dots, u_m$ with $\sum_i E(u_i) = \lim_j E(u^j)$, each of [[def-minimal-surface-index|index]] at most one.

## Proof

> [!note]- Proof outline (click to expand)
> 1. **Concentration set.** With $E(u^j) \le E_0$ bounded, weak $W^{1,2}$ compactness gives a subsequence $u^j \rightharpoonup u_0$ and a finite set $\mathcal{S}_0$ where energy concentrates, finite by [[lem-energy-quantization]]. Off $\mathcal{S}_0$, hypothesis (B) — the maps are $\nu_j$-[[def-almost-harmonic-map|almost harmonic]] with $\nu_j \to 0$ — plus elliptic estimates upgrade weak to strong $W^{1,2}$ convergence, so $u_0$ is harmonic there: this is (B1) of [[def-bubble-convergence]].
> 2. **Rescale the bubbles.** At each $x \in \mathcal{S}_0$, rescale by the conformal dilations tracking the concentration scale; the rescaled maps are again almost harmonic of bounded energy, so by the same argument converge to a harmonic bubble $u_i$ — (B2), with scale separation (B3) from the standard bubbling combinatorics.
> 3. **No energy lost in the necks.** The regions between body and bubbles are long thin cylinders; on them $u^j$ is almost harmonic of small energy, so [[lem-almost-harmonic-cylinder-decay]] (iterated) forces the angular — hence total — energy there to vanish in the limit. This is the no-loss clause (B4).
> 4. **Conclude.** Steps 1–3 are exactly bubble convergence; the limits $u_i$ are branched conformal minimal spheres (harmonic + conformal), of [[def-minimal-surface-index|index]] at most one (a min-max output, not consumed by the extinction argument), and by [[thm-bubble-implies-varifold]] the convergence is varifold. $\square$
## Notes

> [!note]- Notes (click to expand)
> - This is CM's Proposition $p{:}gl2$ (§2, proved §5). Hypothesis (B) is exactly what [[thm-energy-decreasing-map]] delivers; conclusion is bubble convergence to harmonic spheres, which by [[thm-bubble-implies-varifold]] gives the varifold approximation the extinction argument needs.
> - The proof is now a citation chain: weak compactness + almost-harmonicity give the body and bubbles, and the cylinder decay [[lem-almost-harmonic-cylinder-decay]] gives no energy loss in the necks — bubble convergence, promoted to varifold by [[thm-bubble-implies-varifold]]. Remaining debts: the [[thm-sacks-uhlenbeck|Sacks–Uhlenbeck]] concentration threshold $\epsilon_{SU}$ and the strong-convergence elliptic estimates (blackboxed harmonic-map analysis).
