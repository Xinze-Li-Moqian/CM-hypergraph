---
id: 396b1c75bf01
type: definition
references:
  - "Standard real analysis; Evans, Partial Differential Equations, App."
---

# Definition — Lebesgue space Lᵖ

Functions integrable to the p-th power: the basic Banach spaces of
measure theory, in which the derivatives of Sobolev maps are asked to
lie.

## Statement

> [!definition] $L^p$ space
> Let $(\Omega, \mu)$ be a measure space and $1 \le p < \infty$. The *Lebesgue space* $L^p(\Omega)$ is the space of (equivalence classes of, up to $\mu$-null sets) measurable functions $f : \Omega \to \mathbb{R}^N$ with
> $$
> \|f\|_{L^p} = \Big(\int_\Omega |f|^p \, d\mu\Big)^{1/p} < \infty ,
> $$
> a Banach space. For $p = \infty$, $\|f\|_{L^\infty} = \operatorname{ess\,sup}|f|$.

## Notes

> [!note]- Notes (click to expand)
> - Measurable functions and the Lebesgue measure/integral are taken as ground (measure theory); $L^p$ is the first structured space built on them.
> - The gradient of a [[def-sobolev-space|Sobolev]] map lies in $L^p$; the [[def-dirichlet-energy|Dirichlet energy]] is the square of the $L^2$ norm of the gradient.
