---
id: eb3a7b3efc09
type: definition
references:
  - "Standard critical-point theory; Struwe, Variational Methods"
---

# Definition — critical point of a functional

A map where a functional stops changing to first order: the derivative
of the functional vanishes in every direction — the solutions of the
associated Euler–Lagrange equation.

## Statement

> [!definition] Critical point
> Let $\mathcal{F} : X \to \mathbb{R}$ be a $C^1$ functional on a Banach manifold $X$ of maps. A point $u \in X$ is a *critical point* of $\mathcal{F}$ if the differential vanishes, $d\mathcal{F}(u) = 0$ — equivalently $\frac{d}{ds}\big|_{s=0} \mathcal{F}(u_s) = 0$ for every smooth variation $u_s$ with $u_0 = u$. The value $\mathcal{F}(u)$ is a *critical value*.

## Notes

> [!note]- Notes (click to expand)
> - Critical points of the [[def-dirichlet-energy|energy]] are the [[def-minimal-surface|harmonic]] maps (its Euler–Lagrange equation is the harmonic map equation); critical points of the [[def-alpha-energy|α-energy]] are the *α-harmonic maps*.
> - Minimizers are critical points; but critical points need not minimize — the min-max / [[def-mountain-pass|mountain-pass]] ones are saddles, which is why the realizing spheres can have [[def-minimal-surface-index|index]] one.
