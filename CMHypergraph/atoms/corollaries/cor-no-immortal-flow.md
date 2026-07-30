---
id: 8b58cfd8804b
type: corollary
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, Theorem 1.1, the concluding sentence]]"
  - "[[ref-perelman3|Perelman, Finite extinction time…]]"
---

# Corollary — No immortal flow with a sweepout class

The width inequality cashes out: on a manifold that can be swept by spheres, a smooth Ricci flow cannot live forever — the singularity is not an accident but an appointment.

## Statement

> [!corollary] No immortal flow with a sweepout class
> Let $M$ be a [[def-closed-manifold|closed]] $3$-manifold carrying a nontrivial class of [[def-sweepout-width|sweepouts]]. Then no [[def-ricci-flow|Ricci flow]] on $M$ is defined for all $t \in [0, \infty)$: the [[def-maximal-flow|maximal flow]] of every initial metric has finite maximal time.

## Proof

> [!note]- Proof (click to expand)
> Suppose $g(t)$ were defined for all $t \ge 0$, and let $[\beta]$ be a nontrivial class of sweepouts. By [[thm-width-evolution]], the [[def-sweepout-width|width]] $W(t) = W(g(t), [\beta])$ is nonnegative, continuous — the energies of a fixed sweepout vary smoothly with the metric — and defined on all of $[0, \infty)$, satisfying
> $$
> \frac{d}{dt} W \;\le\; -4\pi + \frac{3}{4(t + C)}\, W
> $$
> in the sense of the limsup of forward difference quotients. By [[lem-width-inequality-forces-extinction]], no such function exists past the finite time $T^*(C, W(0))$ — a contradiction. $\square$

## Notes

> [!note]- Notes (click to expand)
> - This is the smooth-flow half of the source theorem's "hence extinct": on such manifolds, surgery is not an optional refinement but a necessity — by [[thm-short-time-existence]], the flow that cannot live forever must die in a curvature blow-up, and only surgery continues past it.
> - Every closed [[def-simply-connected|simply connected]] $3$-manifold carries a nontrivial sweepout class ($\pi_3 \neq 0$, by [[lem-nonaspherical-sweepout-class]] via its homotopy-sphere case) — so in the Poincaré situation the appointment with the singularity is unconditional.
> - The full extinction statement — the flow *with surgery* has empty slices after finite time — is [[thm-finite-time-extinction]]; the bridge from this corollary to it is [[lem-surgery-preserves-width-inequality]].
