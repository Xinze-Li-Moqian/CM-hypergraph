---
id: 2eefaea55e3c
type: definition
references:
  - "Standard; do Carmo / Evans, Partial Differential Equations, ch. 5; used throughout Sacks–Uhlenbeck"
---

# Definition — Sobolev space of maps

Maps with derivatives in an $L^p$ sense: the completion in which variational problems are posed, large enough to contain limits of finite-energy maps, small enough that the derivatives it demands exist.

## Statement

> [!definition] $W^{1,p}(\Sigma, M)$
> For a compact Riemannian domain $\Sigma$, an [[def-isometric-embedding|isometrically embedded]] closed target $M \subset \mathbb{R}^N$, and $1 \le p < \infty$, the *Sobolev space* $W^{1,p}(\Sigma, M)$ is the set of maps $u \in W^{1,p}(\Sigma, \mathbb{R}^N)$ — measurable, with $u$ and its [[def-weak-derivative|weak gradient]] $\nabla u$ in $L^p$ ([[def-lp-space]]) — whose values lie in $M$ almost everywhere. The norm is $\|u\|_{W^{1,p}} = \big(\int_\Sigma |u|^p + |\nabla u|^p\big)^{1/p}$.

## Notes

> [!note]- Notes (click to expand)
> - $W^{1,2}$ is the [[def-dirichlet-energy|energy]] space (finite Dirichlet energy); $W^{1,2\alpha}$ with $\alpha > 1$ is smaller — the natural space of the [[def-alpha-energy|α-energy]]. Larger $p$ demands more integrable derivatives.
> - The critical exponent in dimension two: $W^{1,2}(\Sigma^2)$ *fails* to embed in $C^0$ (the borderline Sobolev case), while $W^{1,p}$ with $p > 2$ embeds compactly in $C^0$ — the gain that makes the α-energy well-behaved.
