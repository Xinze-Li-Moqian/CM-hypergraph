---
id: a3d1f8caa379
type: definition
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §4, Definition `d:bubble`]]"
  - "after Parker–Wolfson and Parker"
---

# Definition — bubble convergence

The convergence harmonic maps actually obey: strong away from finitely
many points, with the energy that concentrates at each point recovered
by rescaling — a body map plus finitely many bubbles blown up at the
concentration points.

## Statement

> [!definition] Bubble convergence
> A sequence $v^j : S^2 \to M$ of $W^{1,2}$ maps *bubble-converges* to a collection $u_0, \dots, u_m : S^2 \to M$ of $W^{1,2}$ maps if:
>
> - **(B1)** $v^j \rightharpoonup u_0$ weakly in $W^{1,2}$, and there is a finite set $\mathcal{S}_0 \subset S^2$ off which $v^j \to u_0$ strongly in $W^{1,2}(K)$ for every compact $K \subset S^2 \setminus \mathcal{S}_0$ — the *body map* $u_0$;
> - **(B2)** for each $i > 0$ there are a point $x_{\ell_i} \in \mathcal{S}_0$ and balls $B_{r_{i,j}}(y_{i,j})$ with $y_{i,j} \to x_{\ell_i}$, $r_{i,j} \to 0$, such that under the [[def-conformal-map|conformal]] dilations $D_{i,j}$ carrying a hemisphere to $B_{r_{i,j}}(y_{i,j})$, the rescaled maps $v^j \circ D_{i,j}$ converge as in (B1) to the *bubble* $u_i$;
> - **(B3)** distinct bubbles have separated scales: $r_{i_1,j}/r_{i_2,j} + r_{i_2,j}/r_{i_1,j} \to \infty$ for $i_1 \neq i_2$;
> - **(B4)** no [[def-dirichlet-energy|energy]] is lost in the limit: $\sum_i E(u_i) = \lim_j E(v^j)$.

## Notes

> [!note]- Notes (click to expand)
> - This is CM's Definition `d:bubble` (§4). It is CM's own notion — a slight weakening of the bubble-tree convergence originally developed for $J$-holomorphic curves (following Parker–Wolfson, see the References), here adapted to harmonic maps. In the min-max application the $v^j$ are almost-harmonic and the limits $u_i$ are harmonic.
> - Energy concentrating at a point of $\mathcal{S}_0$ is not lost — it reappears, at unit scale, as a bubble $u_i$ (B2), and (B4) accounts for all of it. This is what [[thm-bubble-implies-varifold]] promotes to varifold convergence.
