---
id: 27fc30a9c964
type: definition
references:
  - "Standard; Evans, Partial Differential Equations, ch. 5"
---

# Definition — weak derivative

Differentiation defined by integration by parts: a locally integrable
function is the weak derivative of another if it obeys the integration-
by-parts identity against every test function — no classical
differentiability required.

## Statement

> [!definition] Weak derivative
> Let $u \in L^1_{\mathrm{loc}}(\Omega)$, $\Omega \subset \mathbb{R}^n$ open. A function $v \in L^1_{\mathrm{loc}}(\Omega)$ is the *weak partial derivative* $\partial_i u$ if
> $$
> \int_\Omega u\, \partial_i \varphi \;=\; -\int_\Omega v\, \varphi \qquad \text{for all } \varphi \in C^\infty_c(\Omega) .
> $$
> The *weak gradient* $\nabla u = (\partial_1 u, \dots, \partial_n u)$ collects them.

## Notes

> [!note]- Notes (click to expand)
> - It extends the classical derivative (they agree when $u$ is $C^1$) to the merely integrable functions that variational problems produce as limits. A [[def-sobolev-space|Sobolev]] map is one whose weak gradient exists and lies in $L^p$ ([[def-lp-space]]).
> - The integration-by-parts identity is exactly the [[def-weakly-harmonic-map|weak formulation]] used to define weakly harmonic maps.
