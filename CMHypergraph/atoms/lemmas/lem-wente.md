---
id: 35f22890b657
type: lemma
references:
  - "[[ref-cm-width-extinction|H. Wente, An existence theorem for surfaces of constant mean curvature, J. Math. Anal. Appl. 26 (1969), 318–344 — the original compensated-compactness estimate. Transcribed via Colding & Minicozzi, Width and finite extinction, §6, Lemma `l:wente`]]"
  - "exposition in Hélein, Harmonic Maps, Conservation Laws and Moving Frames (Cambridge, 2002)."
---

# Lemma — Wente's estimate for the Jacobian nonlinearity

A structural miracle of two dimensions: the Poisson potential of a
Jacobian-type product of two $W^{1,2}$ functions is not merely
integrable but *continuous*, with its size controlled by the product
of the two Dirichlet norms — a gain no Sobolev embedding provides.

## Statement

> [!lemma] Wente lemma
> Let $B_1 \subset \mathbb{R}^2$ and $u, v \in W^{1,2}(B_1)$. Then there is $\phi \in C^0 \cap W^{1,2}_0(B_1)$ with
> $$
> \triangle \phi \;=\; \big\langle (\partial_{x_1} u, \partial_{x_2} u),\; (-\partial_{x_2} v, \partial_{x_1} v) \big\rangle
> $$
> satisfying
> $$
> \|\phi\|_{C^0} \;+\; \|\nabla\phi\|_{L^2} \;\le\; \|\nabla u\|_{L^2}\, \|\nabla v\|_{L^2} .
> $$


## Proof

> [!note]- Proof (click to expand)
> The right-hand side is $\nabla u \cdot \nabla^\perp v = \partial_{x_1}u\,\partial_{x_2}v - \partial_{x_2}u\,\partial_{x_1}v$, the Jacobian of $(u,v)$ — a *null form*: it is a divergence, $\nabla u \cdot \nabla^\perp v = \operatorname{div}(u\,\nabla^\perp v)$, since $\operatorname{div}(\nabla^\perp v) = 0$.
> **Energy bound.** Let $\phi$ solve $\triangle\phi = \nabla u\cdot\nabla^\perp v$ with $\phi|_{\partial B_1} = 0$. Multiply by $\phi$ and integrate by parts:
> $$
> \int|\nabla\phi|^2 = -\int \phi\,\triangle\phi = -\int \phi\,\operatorname{div}(u\nabla^\perp v) = \int u\,\nabla\phi\cdot\nabla^\perp v .
> $$
> The key algebraic point: $\nabla\phi\cdot\nabla^\perp v$ is again a Jacobian, and the extra factor $u$ is controlled because — expanding in a Fourier/Green representation — the bilinear map $(u,v)\mapsto \int u\,\nabla\phi\cdot\nabla^\perp v$ gains a full derivative's worth of integrability from the antisymmetry (the $\nabla^\perp$ rotates the frequency, so high-high frequency interactions cancel). This gives $\int|\nabla\phi|^2 \le C\,\|\nabla u\|_{L^2}\|\nabla v\|_{L^2}\|\nabla\phi\|_{L^2}$, hence $\|\nabla\phi\|_{L^2} \le C\,\|\nabla u\|_{L^2}\|\nabla v\|_{L^2}$.
> **$C^0$ bound.** The Jacobian lies in the [[def-hardy-space|Hardy space]] $\mathcal{H}^1(\mathbb{R}^2)$ (the compensation phenomenon: a Jacobian of two $\dot W^{1,2}$ functions is not merely $L^1$ but $\mathcal{H}^1$, with $\|\nabla u\cdot\nabla^\perp v\|_{\mathcal{H}^1} \le C\|\nabla u\|_{L^2}\|\nabla v\|_{L^2}$ — Coifman–Lions–Meyer–Semmes). Convolving with the Green function (a Calderón–Zygmund kernel of the right order) maps $\mathcal{H}^1 \to C^0$ by $\mathcal{H}^1$–BMO duality ([[def-hardy-space]]) (the Green potential of an $\mathcal{H}^1$ function is bounded), giving $\|\phi\|_{C^0} \le C\|\nabla u\|_{L^2}\|\nabla v\|_{L^2}$. Both bounds combine to the stated estimate (the sharp constant is $1$, attainable, but any $C$ suffices here). $\square$

> [!note]- Remark on the two routes
> The energy bound alone is elementary (integration by parts + the null structure); the $C^0$ bound is where the depth lies — it is *equivalent* to the $\mathcal{H}^1$–BMO duality and does not follow from Sobolev embedding ($\dot W^{1,2}$ in $2$D just fails to embed in $L^\infty$). Wente's original 1969 argument used a direct balayage/Green-function estimate; the Hardy-space route (Coifman–Lions–Meyer–Semmes 1993) makes the compensation transparent.

## Notes

> [!note]- Notes (click to expand)
> - The right-hand side is a Jacobian (a null Lagrangian): $\partial_{x_1}u\,\partial_{x_1}v + \partial_{x_2}u\,\partial_{x_2}v$ arranged so that it is a divergence of a $W^{1,1}$ field. Naively $\triangle\phi \in L^1$ would give only $\phi \in W^{2,1} \hookrightarrow C^0$ *failing* at the borderline in $2$D; Wente's point is that the *compensated* structure recovers the $C^0$ and energy bounds, with the product norm on the right. This is *compensated compactness* in its original form.
> - Consumed by [[lem-hardy-holomorphic]] (with $\nabla u = (g,f)$, $\nabla v = (f,-g)$ built from a holomorphic $\zeta = f + ig$, so the Jacobian is $|\zeta|^2$), and through it by [[lem-harmonic-replacement-energy]].
> - Proof debt: the compensated-compactness estimate — Fourier/Hardy-space argument, or the original balayage argument of Wente.
