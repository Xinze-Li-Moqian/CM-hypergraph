---
id: 4e233d365173
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §3, equation (3.5)]]"
---

# Lemma — Varifold closeness transfers curvature integrals

The quantitative content of varifold convergence: two surfaces close as
varifolds have nearly equal integrals of any tangent-plane quadratic
form — so an area-decay estimate proved for one transfers to the other.

## Statement

> [!lemma] Varifold closeness transfers curvature integrals
> There is a constant $C$ such that the following holds. Let $\Gamma$ and $\bigcup_i \Sigma_i$ be [[def-immersion|immersed]] surfaces in $(M, g)$ that are $\epsilon$-close in the [[def-varifold|varifold distance]], and let $F$ be a quadratic form on $M$ — a section of symmetric $2$-tensors. Then
> $$
> \left| \int_\Gamma \big[ \operatorname{tr} F - F(\mathbf{n}_\Gamma, \mathbf{n}_\Gamma) \big] \;-\; \sum_i \int_{\Sigma_i} \big[ \operatorname{tr} F - F(\mathbf{n}_{\Sigma_i}, \mathbf{n}_{\Sigma_i}) \big] \right| \;<\; C\, \epsilon\, \| F \|_{C^1} ,
> $$
> where $\mathbf{n}$ is the unit normal and $\operatorname{tr}$ the [[def-trace|trace]].


## Proof

> [!note]- Proof (click to expand)
> The integrand $\operatorname{tr} F - F(\mathbf n, \mathbf n)$ is a continuous function on the Grassmann bundle $G_2 M$: at a point $(x, P)$ with $P$ a tangent $2$-plane and $\mathbf n$ its unit normal, it equals $\operatorname{tr}(F|_P) = F(e_1,e_1) + F(e_2,e_2)$ for an orthonormal basis $e_1, e_2$ of $P$ — call it $\hat F(x, P)$, continuous in $(x,P)$ with $\|\hat F\|_{C^0} \le C\|F\|_{C^0}$ and Lipschitz constant $\le C\|F\|_{C^1}$.
> The surface integral is the pairing of $\hat F$ against the surface's [[def-varifold|varifold]]: $\int_\Sigma [\operatorname{tr} F - F(\mathbf n_\Sigma,\mathbf n_\Sigma)] = \int_{G_2 M} \hat F\, dV_\Sigma$. By hypothesis $\Gamma$ and $\bigcup_i\Sigma_i$ are $\epsilon$-close in the varifold distance, i.e. $|\int \hat F\, dV_\Gamma - \int \hat F\, dV_{\cup\Sigma_i}| \le \epsilon\, \|\hat F\|_{\text{Lip}}$ (definition of the weak-$*$ metric). Hence
> $$
> \Big| \int_\Gamma [\operatorname{tr} F - F(\mathbf n,\mathbf n)] - \sum_i \int_{\Sigma_i}[\operatorname{tr} F - F(\mathbf n,\mathbf n)]\Big| \le \epsilon\, \|\hat F\|_{\text{Lip}} \le C\,\epsilon\, \|F\|_{C^1}. \qquad \square
> $$

## Notes

> [!note]- Notes (click to expand)
> - The integrand $\operatorname{tr} F - F(\mathbf n, \mathbf n)$ is a function of the tangent plane alone — it is $F$ traced over $T\Sigma$. A [[def-varifold|varifold]] records exactly area-with-tangent-plane, so this integral is $\int_{G_2(M)} \langle F, \cdot\rangle\, dV$, continuous in the varifold weak-$*$ topology; the $C^1$ norm of $F$ controls the modulus of continuity. This is CM's (3.5).
> - Two consumers in the width evolution: with $F = g$ it gives $\operatorname{tr} g - g(\mathbf n,\mathbf n) = 2$, so areas agree up to $C\epsilon$ ($\operatorname{Area}(\Gamma) \approx \sum_i \operatorname{Area}(\Sigma_i)$); with $F = \operatorname{Ric}$ it makes the first-variation integrands of [[lem-area-first-variation-under-flow]] agree — which is how the area-decay estimate for the minimal spheres passes to the competing slice $\Gamma$.
> - Proof debt: an immediate consequence of the varifold approximation property ([[prop-minmax-minimal-spheres]], conclusion 3) and the definition of varifold distance; classical.
