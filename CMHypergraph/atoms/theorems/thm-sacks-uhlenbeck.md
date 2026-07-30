---
id: e93dbb145f82
type: theorem
references:
  - "[[ref-sacksuhlenbeck|J. Sacks & K. Uhlenbeck, The existence of minimal immersions of 2-spheres, Ann. of Math. 113 (1981), 1–24]]"
  - "[[ref-cm-width-extinction|used throughout Colding & Minicozzi, Width and finite extinction]]"
---

# Theorem — Sacks–Uhlenbeck: harmonic maps and the energy threshold

The foundational existence theorem of harmonic-map min-max: below a
universal energy threshold, boundary-value problems have unique smooth
energy-minimizers, and above it, energy escaping to a point reappears
as a bubble — a harmonic sphere.

## Statement

> [!theorem] Sacks–Uhlenbeck
> There is a constant $\epsilon_{SU} > 0$ (depending on the closed target $M$) with the following properties.
>
> 1. *(Minimizers below threshold.)* For a disc $B \subset \mathbb{R}^2$ and boundary values of [[def-dirichlet-energy|energy]] less than $\epsilon_{SU}$, there is a unique energy-minimizing (weakly [[def-minimal-surface|harmonic]]) map $B \to M$ with those boundary values, and it is smooth.
> 2. *(Bubbling.)* A sequence of almost-harmonic maps $S^2 \to M$ of bounded energy has a subsequence converging, away from finitely many points where energy concentrates in quantities $\ge \epsilon_{SU}$, to a harmonic map; the concentrated energy is recovered, after [[def-conformal-map|conformal]] rescaling, as harmonic *bubbles*.


## Proof

> [!note]- Proof — citation chain (click to expand)
> **1. Existence.** In two dimensions the energy $E$ is *critical* — minimizing sequences bubble, Palais–Smale fails, so existence is not automatic. Sacks–Uhlenbeck perturb to the subcritical [[def-alpha-energy|α-energy]]: by [[lem-alpha-energy-critical-points]], for $\alpha > 1$ critical points $u_\alpha$ (α-harmonic maps) exist and are smooth, with uniformly bounded energy; by [[lem-alpha-energy-limit]], as $\alpha \to 1$ they converge to a harmonic map off finitely many bubble points. On a disc with small boundary energy this limit is the unique minimizer of conclusion 1 (below the threshold $\epsilon_0$ of [[lem-epsilon-regularity-harmonic]], where $E$ is convex on the relevant maps). Set $\epsilon_{SU} := \epsilon_0$.
> **2. Bubbling.** For a sequence of almost-harmonic maps of bounded energy, weak $W^{1,2}$ compactness gives $u^j \rightharpoonup u_0$, strong (so $u_0$ harmonic) off the finite concentration set by [[lem-energy-quantization]] and $\epsilon$-regularity ([[lem-epsilon-regularity-harmonic]]); at each concentration point, conformal rescaling plus [[lem-removable-singularity-harmonic]] produces a harmonic-sphere bubble $u_1, \dots, u_m$. $\square$
## Notes

> [!note]- Notes (click to expand)
> - The threshold $\epsilon_{SU}$ is the quantum of energy below which no bubbling occurs — it bounds the number of bubbles ($\le E_0/\epsilon_{SU}$) and makes [[def-harmonic-replacement|harmonic replacement]] well-defined. It is the constant in the hypotheses of [[thm-almost-minimizing-compactness]] and the small-energy regime of the whole §3–§6 machinery.
> - Blackbox for this graph: a deep external theorem, carded here as a node so the min-max argument stays self-contained (every "by Sacks–Uhlenbeck" is an in-graph link), but not proved.
