---
id: 502caf83aa04
type: proposition
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §7, Proposition `p:eq`]]"
---

# Proposition — The energy and area widths coincide

The two definitions of the width agree: minimizing the maximal energy
over sweepouts gives the same number as minimizing the maximal area —
so the whole extinction argument may be run with whichever is
convenient.

## Statement

> [!proposition] $W_E = W_A$
> For a [[def-closed-manifold|closed]] Riemannian $3$-manifold $M$ and a nontrivial class of [[def-sweepout-width|sweepouts]], the *[[def-dirichlet-energy|energy]] width* $W_E = \min_\gamma \max_t E(\gamma(\cdot, t))$ and the *area width* $W_A = \min_\gamma \max_t \operatorname{Area}(\gamma(\cdot, t))$ are equal.

## Proof

> [!note]- Proof — citation chain (click to expand)
> Always $\operatorname{Area}(u) \le E(u)$ pointwise (with equality for conformal maps), so $W_A \le W_E$.
> For the reverse: given a sweepout nearly achieving $W_A$, regularize it to smooth slices by [[lem-sweepout-density]]. Reparametrize each slice conformally — replacing $\tilde\gamma(\cdot, t)$ by $\tilde\gamma(\cdot, t) \circ h_t$ with $h_t$ the uniformizing map of the pulled-back metric — so that energy drops to area; by [[lem-conformal-parametrization-continuous]] the maps $h_t$ vary continuously, so the reparametrized family is again a sweepout in the same class. Its maximal energy is (up to $\epsilon$) the maximal area of the original, giving $W_E \le W_A + \epsilon$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - This is CM's Proposition `p:eq` (§7). It justifies defining the [[def-sweepout-width|width]] by energy — the analytically convenient choice, since energy is smooth under the flow and lower semicontinuous — while the geometric statements (area decay, extinction) are about area.
> - The equality is why the min-max realization [[prop-minmax-minimal-spheres]] can conclude with $\operatorname{Area}(u_i) = E(u_i)$: the realizing spheres are conformal, where the two agree.
