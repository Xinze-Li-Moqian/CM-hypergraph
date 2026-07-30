---
id: 7959f285ebd4
type: definition
references:
  - "Hélein, Harmonic Maps, Conservation Laws and Moving Frames; Schoen–Yau, Lectures on Harmonic Maps"
---

# Definition — weakly harmonic map

A harmonic map in the integral sense: a finite-energy map that is
critical for the energy against smooth variations, without assuming in
advance that it is smooth enough to write the equation classically.

## Statement

> [!definition] Weakly harmonic map
> A map $u \in W^{1,2}(\Sigma, M)$ is *weakly harmonic* if it is a [[def-critical-point|critical point]] of the [[def-dirichlet-energy|energy]]: for every smooth variation $u_s$ through $W^{1,2}$ maps into $M$ with $u_0 = u$,
> $$
> \frac{d}{ds}\Big|_{s=0} E(u_s) = 0 ,
> $$
> equivalently $\triangle u \perp T_u M$ weakly — $\int_\Sigma \langle \nabla u, \nabla \varphi\rangle = 0$ for all $\varphi$ tangent to $M$ along $u$.

## Notes

> [!note]- Notes (click to expand)
> - "Weak" = only $W^{1,2}$ assumed, not smoothness. That a weakly harmonic map from a *surface* is in fact smooth is [[thm-helein-regularity|Hélein's theorem]] — the non-trivial regularity that the whole harmonic-map analysis rests on.
> - The energy-minimizing map with given boundary values is weakly harmonic; below the small-energy threshold it is unique and, by [[lem-epsilon-regularity-harmonic|ε-regularity]], smooth.
