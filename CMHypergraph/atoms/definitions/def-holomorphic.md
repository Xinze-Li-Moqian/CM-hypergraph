---
id: ed1e207c5c46
type: definition
references:
  - "Standard complex analysis; used in Colding–Minicozzi §6"
---

# Definition — holomorphic function

A complex-differentiable function of one complex variable: it satisfies
the Cauchy–Riemann equations, equivalently its differential is complex-
linear — the rigidity that makes its modulus a good weight.

## Statement

> [!definition] Holomorphic function
> A function $\zeta = f + ig : \Omega \to \mathbb{C}$ on an open $\Omega \subset \mathbb{R}^2 \cong \mathbb{C}$ is *holomorphic* if it is complex-differentiable, equivalently if its real and imaginary parts satisfy the *Cauchy–Riemann equations*
> $$
> \partial_{x_1} f = \partial_{x_2} g, \qquad \partial_{x_2} f = -\partial_{x_1} g ,
> $$
> equivalently $\partial_{\bar z}\zeta = 0$ where $\partial_{\bar z} = \tfrac12(\partial_{x_1} + i\partial_{x_2})$.

## Notes

> [!note]- Notes (click to expand)
> - Consequence used in the harmonic-map analysis: for holomorphic $\zeta$, $|\zeta|^2$ is a Jacobian ($|\nabla u|^2 = |\zeta|^2$ for potentials $u,v$ from the Cauchy–Riemann system), so it lies in the [[lem-wente|Wente]] / Hardy-space regime — this is why the [[lem-hardy-holomorphic|holomorphic Hardy inequality]] holds.
> - A [[def-conformal-map|conformal]] map of surfaces is, in local complex coordinates, holomorphic (or antiholomorphic).
