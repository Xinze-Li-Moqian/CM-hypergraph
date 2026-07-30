---
id: 42ebabd5cb39
type: lemma
rigor: outline
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §3, Lemma `l:patch`]]"
---

# Lemma — The two-ball replacement gap

The quantitative engine of the tightening: replacing on two overlapping
ball collections lowers energy by at least a definite multiple of the
square of the further improvement still available — so the iteration
cannot stall while any energy remains to be shed.

## Statement

> [!lemma] Two-ball replacement gap
> There is $\kappa > 0$ (depending on $M$) such that if $u : S^2 \to M$ is $C^0 \cap W^{1,2}$ and $\mathcal{B}_1, \mathcal{B}_2$ are finite collections of disjoint closed balls on each of which $u$ has [[def-dirichlet-energy|energy]] at most $\epsilon_1/3$, then the [[def-harmonic-replacement|harmonic replacement]] satisfies
> $$
> E(u) - E\big[H(u, \mathcal{B}_1, \mathcal{B}_2)\big] \;\ge\; \kappa \, \Big( E(u) - E\big[H(u, \tfrac12\mathcal{B}_2)\big] \Big)^2 ,
> $$
> and for any $\mu \in [1/8, 1/2]$,
> $$
> \frac{\big(E(u) - E[H(u, \mathcal{B}_1)]\big)^{1/2}}{\kappa} + E(u) - E\big[H(u, 2\mu\mathcal{B}_2)\big] \;\ge\; E\big[H(u, \mathcal{B}_1)\big] - E\big[H(u, \mathcal{B}_1, \mu\mathcal{B}_2)\big] .
> $$


## Proof

> [!note]- Proof outline (click to expand)
> Both inequalities follow from the single-ball convexity [[lem-harmonic-replacement-energy]] summed over the balls, with the overlap bookkeeping of the two collections.
> For the first: on each ball of $\mathcal{B}_2$, replacing $u$ by its [[def-harmonic-replacement|harmonic replacement]] lowers energy by at least $\tfrac12\int|\nabla(\text{replacement} - u)|^2$ (the gap lemma), and the residual improvement still available on $\tfrac12\mathcal{B}_2$ is bounded by the $W^{1,2}$ distance to harmonic; comparing the two via Cauchy–Schwarz over the balls produces the *square*: $E(u) - E[H(u,\mathcal{B}_1,\mathcal{B}_2)] \ge \kappa(E(u) - E[H(u,\tfrac12\mathcal{B}_2)])^2$, with $\kappa$ from the gap constant and the overlap multiplicity.
> The second inequality is the telescoping identity $E(u) - E[H(u,\mathcal{B}_1,\mu\mathcal{B}_2)] = (E(u) - E[H(u,\mathcal{B}_1)]) + (E[H(u,\mathcal{B}_1)] - E[H(u,\mathcal{B}_1,\mu\mathcal{B}_2)])$ rearranged, with the cross term controlled by the first-collection improvement via the gap lemma applied on $\mathcal{B}_1$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - This is CM's Lemma `l:patch` (§3). The *square* on the right is the point: it makes the gap comparable to the residual improvement, so the modulus $\Psi$ of [[thm-energy-decreasing-map]] can be built and the iterated replacement converges. The two half-scaled collections ($\tfrac12\mathcal{B}_2$, $2\mu\mathcal{B}_2$) track how replacement on one collection interacts with the next.
> - Rests on the single-ball strict convexity [[lem-harmonic-replacement-energy]] (CM's `l:trivmap`), summed over the balls with the overlap bookkeeping.
> - Proof debt: §3 — the summation-and-overlap argument.
