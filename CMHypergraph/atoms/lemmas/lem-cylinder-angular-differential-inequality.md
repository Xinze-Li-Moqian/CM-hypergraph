---
id: 099d570f5b3d
type: lemma
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §5, Lemma `l:difi`]]"
---

# Lemma — Angular energy of a harmonic map bends up

The differential inequality that drives cylinder decay: along a
harmonic map on a cylinder, the angular energy of each circle is a
convex-like function of the axial coordinate, up to a quartic error.

## Statement

> [!lemma] Angular [[def-dirichlet-energy|energy]] differential inequality
> For a $C^3$ [[def-minimal-surface|harmonic]] map $u$ from a cylinder $\mathcal{C}_{r_1, r_2} \subset \mathcal{C}$ to $M \subset \mathbb{R}^N$, with $u_\theta$ the angular derivative,
> $$
> \partial_t^2 \int_{\{t\}} |u_\theta|^2 \;\ge\; \tfrac{3}{2} \int_{\{t\}} |u_\theta|^2 \;-\; 2 \sup_M |A|^2 \int_{\{t\}} |\nabla u|^4 ,
> $$
> where the integrals are over the circle at axial coordinate $t$ and $A$ is the [[def-second-fundamental-form|second fundamental form]].


## Proof

> [!note]- Proof (click to expand)
> Differentiate the angular energy twice and integrate by parts in $\theta$ on the circle (no boundary):
> $$
> \tfrac12\, \partial_t^2\!\int_t |u_\theta|^2 = \int_t |u_{t\theta}|^2 + \int_t \langle u_\theta, u_{tt\theta}\rangle = \int_t |u_{t\theta}|^2 - \int_t \langle u_{\theta\theta}, u_{tt}\rangle .
> $$
> On the flat cylinder $\triangle u = u_{tt} + u_{\theta\theta}$, so $u_{tt} = \triangle u - u_{\theta\theta}$; substituting,
> $$
> = \int_t |u_{t\theta}|^2 - \int_t \langle u_{\theta\theta}, \triangle u - u_{\theta\theta}\rangle = \int_t |u_{t\theta}|^2 + \int_t |u_{\theta\theta}|^2 - \int_t \langle u_{\theta\theta}, \triangle u\rangle .
> $$
> The [[def-minimal-surface|harmonic]] map equation gives $\triangle u = A(u)(\nabla u, \nabla u)$ normal to $M$ with $|\triangle u| \le \sup_M|A|\,|\nabla u|^2$ (SY p.157: $\triangle_M u^i = g^{jk} A^i_{u}(\partial_j u, \partial_k u)$). Hence
> $$
> \tfrac12\, \partial_t^2\!\int_t |u_\theta|^2 \;\ge\; \int_t |u_{t\theta}|^2 + \int_t |u_{\theta\theta}|^2 - \sup_M|A|\int_t |u_{\theta\theta}|\,|\nabla u|^2 .
> $$
> Apply the absorbing inequality $2ab \le \tfrac12 a^2 + 2b^2$ to the last term (with $a = |u_{\theta\theta}|$, $b = \sup|A|\,|\nabla u|^2$): $\sup|A|\int|u_{\theta\theta}|\,|\nabla u|^2 \le \tfrac12\int|u_{\theta\theta}|^2 + 2\sup_M|A|^2\int|\nabla u|^4$. Dropping $\int|u_{t\theta}|^2 \ge 0$,
> $$
> \tfrac12\,\partial_t^2\!\int_t|u_\theta|^2 \;\ge\; \tfrac12\int_t|u_{\theta\theta}|^2 - 2\sup_M|A|^2\int_t|\nabla u|^4 .
> $$
> Finally $\int_t u_\theta = 0$ (a full loop), so [[def-wirtinger-inequality|Wirtinger]]'s inequality on $S^1$ gives $\int_t|u_\theta|^2 \le \int_t|u_{\theta\theta}|^2$; substituting and multiplying by $2$,
> $$
> \partial_t^2\!\int_t|u_\theta|^2 \;\ge\; \tfrac{3}{2}\int_t|u_\theta|^2 - 2\sup_M|A|^2\int_t|\nabla u|^4 . \qquad \square
> $$

## Notes

> [!note]- Notes (click to expand)
> - This is CM's Lemma `l:difi` (§5). The main term $\tfrac32 \int|u_\theta|^2$ is what feeds the $\sinh$ of [[lem-ode-comparison-sinh]] (with $a$ absorbing the quartic error, small when energy is small); the quartic term is controlled by the ambient curvature.
> - SY p.157 = Schoen–Yau, the harmonic map equation via the second fundamental form; Wirtinger on $S^1$ is the Poincaré inequality for mean-zero functions.
