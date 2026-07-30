---
id: 70b4baae3253
type: theorem
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, Theorem in §1 and §3]]"
---

# Theorem — The energy-decreasing map

The tightening step of the min-max: any sweepout with no non-constant
harmonic slice can be deformed to one of no greater energy, whose
near-maximal slices are quantitatively close to being energy-minimizing
on every small ball.

## Statement

> [!theorem] Energy-decreasing map
> There are $\epsilon_0 > 0$ and a continuous $\Psi : [0, \infty) \to [0, \infty)$ with $\Psi(0) = 0$, depending on $M$, with the following property. Given $\tilde\gamma \in \Omega$ with no non-constant harmonic slice and $W > 0$, there is a [[def-sweepout-width|sweepout]] $\gamma$ homotopic to $\tilde\gamma$ with $E(\gamma(\cdot, t)) \le E(\tilde\gamma(\cdot, t))$ for every $t$, such that for each $t$ with $E(\tilde\gamma(\cdot, t)) \ge W/2$: for any finite collection $\mathcal{B}$ of disjoint closed balls in $S^2$ with $\int_{\cup \mathcal{B}} |\nabla\gamma|^2$ small, the [[def-dirichlet-energy|energy]] of $\gamma$ on $\tfrac18\mathcal{B}$ exceeds that of its energy-minimizing (harmonic) replacement by at most $\Psi\big(E(\tilde\gamma(\cdot,t)) - E(\gamma(\cdot,t))\big)$.


## Proof

> [!note]- Proof — citation chain (click to expand)
> Iterate [[def-harmonic-replacement|harmonic replacement]] over the good-ball collections. By [[lem-good-balls]], for each $t$ there are $\le 2$ ball collections $\mathcal{B}_j(t)$ covering the high-gradient part of $\tilde\gamma(\cdot,t)$ with small energy on each. Define $\gamma(\cdot,t) = H(\tilde\gamma(\cdot,t), \mathcal{B}_1(t), \mathcal{B}_2(t))$ — replacement lowers energy, giving $E(\gamma(\cdot,t)) \le E(\tilde\gamma(\cdot,t))$.
> **Continuity** in $t$ (so $\gamma \in \Omega$) uses [[lem-harmonic-replacement-continuity]] and [[lem-nonharmonic-interval]], which patch the per-$t$ replacements into a continuous family.
> **The modulus $\Psi$.** By the two-ball gap [[lem-harmonic-replacement-gap]], the energy drop controls the residual improvement's square; inverting, the residual (how far $\gamma(\cdot,t)$ is from energy-minimizing on small balls) is bounded by $\Psi(E(\tilde\gamma) - E(\gamma))$ with $\Psi(s) = C\sqrt{s} \to 0$ as $s \to 0$ — the almost-minimizing property (B). $\square$

## Notes

> [!note]- Notes (click to expand)
> - This is CM's Theorem $p{:}tilde$ (§1, constructed in §3). It is the *pull-tight* construction of min-max: replacing each slice by a controlled harmonic replacement lowers energy, and the deformed family's top slices are almost energy-minimizing on small balls — the hypothesis of the compactness step [[thm-almost-minimizing-compactness]]. The modulus $\Psi$ makes "almost" quantitative: if the energy barely dropped, the slice was already almost harmonic.
> - The construction is iterated [[def-harmonic-replacement|harmonic replacement]]; its convergence rests on the two-ball gap [[lem-harmonic-replacement-gap]] (squaring the residual, so the modulus $\Psi$ exists), over the single-ball engine [[lem-harmonic-replacement-energy]].
> - Proof debt (§3), the remaining machinery to card: continuity of harmonic replacement in $C^0 \cap W^{1,2}$ (`l:approx`), the interval/covering structure of non-harmonic slices (`l:sf`), and the good-balls construction over the family (`l:goodballs`).
