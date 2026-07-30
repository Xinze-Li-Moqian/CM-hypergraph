---
id: a2e3df614fd9
type: lemma
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §6, Proposition `c:hardy`]]"
---

# Lemma — A Hardy inequality for a holomorphic weight

The modulus of a holomorphic function is a good weight: a function
vanishing on the boundary, weighted by $|\zeta|^2$, has its $L^2$ mass
controlled by its Dirichlet energy — an endpoint estimate the Sobolev
embedding just misses.

## Statement

> [!lemma] Holomorphic Hardy inequality
> Let $\zeta$ be a [[def-holomorphic|holomorphic]] function on $B_1 \subset \mathbb{R}^2$ and $h \in W^{1,2}_0(B_1)$. Then
> $$
> \int_{B_1} h^2\, |\zeta|^2 \;\le\; 8\, \left( \int_{B_1} |\nabla h|^2 \right)\left( \int_{B_1} |\zeta|^2 \right) .
> $$

## Proof

> [!note]- Proof (click to expand)
> Write the [[def-holomorphic|holomorphic]] $\zeta = f + i g$ with $f, g$ its real and imaginary parts; the Cauchy–Riemann equations give $\partial_{x_1} f = \partial_{x_2} g$ and $\partial_{x_2} f = -\partial_{x_1} g$. Since $B_1$ is simply connected, there are $u, v$ with $\nabla u = (g, f)$ and $\nabla v = (f, -g)$, and then
> $$
> |\nabla u|^2 = |\nabla v|^2 = \big\langle (\partial_{x_1}u, \partial_{x_2}u),\, (-\partial_{x_2}v, \partial_{x_1}v)\big\rangle = |\zeta|^2 .
> $$
> By [[lem-wente]] there is $\phi$ with $\triangle\phi = |\zeta|^2$, $\phi|_{\partial B_1} = 0$, and $\|\phi\|_{C^0} + \|\nabla\phi\|_{L^2} \le \int|\zeta|^2$. Applying Stokes' theorem to $\operatorname{div}(h^2\nabla\phi)$ and Cauchy–Schwarz,
> $$
> \int h^2 |\zeta|^2 = \int h^2\, \triangle\phi = -\int \nabla(h^2)\cdot\nabla\phi \le \int |\nabla h^2|\,|\nabla\phi| \le 2\left(\int h^2|\nabla h|^2\right)^{1/2}\|\nabla\phi\|_{L^2}.
> $$
> Bounding $\int h^2|\nabla h|^2 \le (\sup|h|^2)\int|\nabla h|^2$ and $\|\nabla\phi\|_{L^2} \le \int|\zeta|^2$, together with the $C^0$ bound on the potential and one more Cauchy–Schwarz, yields the constant $8$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - Why not Sobolev: on $B_1 \subset \mathbb{R}^2$ the product of an $L^2$ and a $W^{1,2}$ function lies in $L^p$ only for $p < 2$; the holomorphy of $\zeta$ (via Wente's compensated structure) is exactly what recovers the endpoint $p = 2$.
> - This is CM's Proposition `c:hardy` (§6). It feeds [[lem-harmonic-replacement-energy]] by controlling the cross term in the energy-difference estimate.
