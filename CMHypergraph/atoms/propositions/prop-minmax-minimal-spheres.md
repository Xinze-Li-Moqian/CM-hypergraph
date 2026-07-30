---
id: abf7406b9119
type: proposition
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §3]]"
  - "[[ref-jost|Jost, Theorem 4.2.1 — the statement the source's proof cites]]"
  - "building on Sacks–Uhlenbeck, Siu–Yau/Meeks–Yau, and Colding–De Lellis for the approximation property; index bound as in Micallef–Moore"
---

# Proposition — Min-max realization by minimal spheres

The width is not an abstract infimum: it is realized by an actual collection of minimal 2-spheres, and every nearly-maximal slice of a good sweepout sequence looks like such a collection.

## Statement

> [!proposition] Min-max realization by minimal spheres
> Let $(M, g)$ be a [[def-closed-manifold|closed]] Riemannian $3$-manifold and $[\beta]$ a nontrivial class of [[def-sweepout-width|sweepouts]]. Then:
>
> 1. the [[def-sweepout-width|width]] $W(g, [\beta])$ is positive;
> 2. there are sweepouts $\gamma^j \in [\beta]$ with $\max_s E(\gamma^j_s) \to W(g, [\beta])$, and branched [[def-conformal-map|conformal]] [[def-minimal-surface|minimal immersions]] $u_0, \dots, u_m : S^2 \to M$, each with $\operatorname{Area}(u_i) = E(u_i)$, such that
> $$
> W(g, [\beta]) \;=\; \sum_{i=0}^{m} E(u_i),
> $$
> the $u_i$ arising as limits of conformal rescalings of near-maximal slices $\gamma^j_{s_j}$;
> 3. the sequence $\gamma^j$ may be chosen so that, for every $\epsilon > 0$, there are $J$ and $\delta > 0$ such that: if $j > J$ and $E(\gamma^j_s) > W(g, [\beta]) - \delta$, then $\gamma^j_s$ is $\epsilon$-close in the [[def-varifold|varifold distance]] to a union of [[def-minimal-surface|branched minimal]] $2$-spheres, each of [[def-minimal-surface-index|index]] at most one.

## Proof

> [!note]- Proof — citation chain (click to expand)
> The long companion paper proves this as its min-max existence theorem; the argument has three moves.
> 1. **Tighten.** Start from a sweepout $\tilde\gamma^j$ with $\max_s E \to W$. If some slice is a non-constant harmonic sphere the tightening terminates there, a degenerate case the sketch does not follow through; otherwise [[thm-energy-decreasing-map]] deforms it to $\gamma^j$ of no greater energy whose near-maximal slices are almost energy-minimizing on every small ball — hypothesis (B) of the next step — with the deficit controlled by $\Psi$. Positivity of $W$ (conclusion 1) is where a nontrivial $\pi_3$ class ([[lem-sweepout-classes-are-pi3]]) is used.
> 2. **Extract minimal spheres.** Along a near-maximal subsequence, hypotheses (A) area $\approx$ energy and (B) almost-minimizing are met, so [[thm-almost-minimizing-compactness]] gives bubble convergence to branched conformal minimal spheres $u_0, \dots, u_m$ of index at most one with $W = \sum_i E(u_i)$ — conclusions 1 and 2.
> 3. **Varifold approximation.** By [[thm-bubble-implies-varifold]], bubble convergence is varifold convergence, so every slice with $E > W - \delta$ is $\epsilon$-close in the varifold distance to $\bigcup_i \Sigma_i$ — conclusion 3. $\square$
## Notes

> [!note]- Notes (click to expand)
> - **A gap in the sketch.** Step 1 sets aside the case of a slice that is already a non-constant harmonic sphere, and does not say how the three conclusions are recovered there. The companion paper treats it; nothing in this pool does.
>
> - **The index bound is not consumed by finite extinction.** Conclusion 2 records that the realizing spheres have index at most one ([[thm-micallef-moore-index]]), but the extinction argument uses only their *existence* and the $-4\pi$ area decay of [[lem-minimal-sphere-area-decay]] — which holds for *any* minimal sphere, index or not. The index bound is needed only for the sharper $-16\pi$ estimate ([[lem-area-decay-index-one]]) of the reducible case (Appendix A), which the simply-connected Poincaré situation never invokes. So $\lceil$index $\le 1\rceil$ is a genuine output of the min-max, carried for completeness, not a load-bearing hypothesis downstream.
>
> - Conclusion 3 is what the evolution argument actually consumes: *every* slice that could compete for the maximum is geometrically a union of minimal spheres, so an area-decay estimate for minimal spheres controls the whole top of the sweepout.
> - Every term is now carded: branched conformal minimal immersion is [[def-minimal-surface]], the [[def-minimal-surface-index|index]] and the [[def-varifold|varifold distance]] have their cards; only the min-max machinery producing them remains the proof debt.
> - The proof is a citation chain over the three pillars of the long paper: [[thm-energy-decreasing-map]] (tighten), [[thm-almost-minimizing-compactness]] (extract), [[thm-bubble-implies-varifold]] (varifold) — each a debt card, but the min-max is no longer a single black box.
> - **The source's own proof is a citation.** In the short paper this proposition rests on the classical chain: Sacks–Uhlenbeck give the harmonic spheres (with possible energy loss), Siu–Yau/Meeks–Yau rule the loss out, and the statement actually cited is Jost's min-max theorem — now carded, statement checked against the book, as [[thm-minmax-harmonic-maps]] — with the index bound not stated there but following as in Micallef–Moore ([[thm-micallef-moore-index]]). The card's proof instead follows the expanded companion paper's self-contained route, which re-proves that black box; Jost's theorem stays in the references as the parallel source.
