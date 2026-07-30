---
id: c2b58e56dfc6
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §2, Lemma 2]]"
  - "[[ref-hamiltonsurvey|the area-evolution computation goes back to Hamilton]]"
---

# Lemma — Minimal spheres lose area at rate 4π

Under Ricci flow, every minimal 2-sphere loses area at the definite rate $4\pi$ — the Gauss–Bonnet constant of the sphere — plus a term
controlled by the worst scalar curvature.

## Statement

> [!lemma] Minimal spheres lose area at rate $4\pi$
> Let $(M, g(t))$ be a [[def-ricci-flow|Ricci flow]] on a $3$-manifold and let $\Sigma \subset M$ be a [[def-minimal-surface|branched minimal immersion]] of $S^2$ with respect to $g(0)$. Then
> $$
> \frac{d}{dt}\Big|_{t=0} \operatorname{Area}_{g(t)}(\Sigma) \;\le\; -4\pi \;-\; \frac{\operatorname{Area}_{g(0)}(\Sigma)}{2} \, \min_M R(0),
> $$
> where $R$ is the [[def-scalar-curvature|scalar curvature]] of $g(0)$.

## Proof

> [!note]- Proof (click to expand)
> Write $\mathbf{n}$ for the unit normal and $A$ for the [[def-second-fundamental-form|second fundamental form]] of $\Sigma$; let $\{p_i\}$ be the branch points, of orders $b_i > 0$.
>
> 1. **Area responds to the flow.** By [[lem-area-first-variation-under-flow]] applied to $\Sigma$,
> $$
> \frac{d}{dt}\Big|_{t=0} \operatorname{Area}_{g(t)}(\Sigma) \;=\; -\int_\Sigma \big[ R - \operatorname{Ric}(\mathbf{n}, \mathbf{n}) \big].
> $$
> 2. **Rewrite the integrand intrinsically.** In an orthonormal frame $e_1, e_2, \mathbf{n}$ adapted to $\Sigma$, the scalar curvature is $R = 2K_M + 2\operatorname{Ric}(\mathbf n,\mathbf n)$, where $K_M$ is the ambient [[def-sectional-curvature|sectional curvature]] of the tangent plane $T\Sigma$; hence $\operatorname{Ric}(\mathbf n,\mathbf n) = \tfrac12 R - K_M$ and
> $$
> R - \operatorname{Ric}(\mathbf n,\mathbf n) \;=\; \tfrac12 R + K_M .
> $$
> Replacing $K_M = K_\Sigma + \tfrac12|A|^2$ by the [[lem-gauss-equation|Gauss equation]] for the [[def-minimal-surface|minimal]] $\Sigma$ (where $\det A = -\tfrac12|A|^2$), the integrand is $K_\Sigma + \tfrac12|A|^2 + \tfrac12 R$, so
> $$
> \frac{d}{dt}\Big|_{t=0} \operatorname{Area}(\Sigma) \;=\; -\int_\Sigma K_\Sigma \;-\; \tfrac12 \int_\Sigma \big( |A|^2 + R \big) ,
> $$
> the form (2.2) of the source.
> 3. **Gauss–Bonnet supplies the $-4\pi$.** By the branched [[thm-gauss-bonnet]], $\int_\Sigma K_\Sigma = 2\pi\big(\chi(S^2) + \sum_i b_i\big) = 2\pi\big(2 + \sum_i b_i\big)$, so
> $$
> -\int_\Sigma K_\Sigma \;=\; -4\pi \;-\; 2\pi \sum_i b_i \;\le\; -4\pi .
> $$
> 4. **Bound the remaining integral.** Dropping the non-negative $|A|^2$ and bounding $R \ge \min_M R(0)$ pointwise,
> $$
> -\tfrac12 \int_\Sigma \big( |A|^2 + R \big) \;\le\; -\tfrac12 \int_\Sigma R \;\le\; -\tfrac12 \operatorname{Area}(\Sigma)\, \min_M R(0).
> $$
> Adding steps 3 and 4 gives the claim; the branch terms $-2\pi\sum_i b_i \le 0$ only strengthen it. $\square$

## Notes

> [!note]- Notes (click to expand)
> - The proof is a citation chain over three inputs — the first variation [[lem-area-first-variation-under-flow]], the [[lem-gauss-equation|Gauss equation]], and the branched [[thm-gauss-bonnet]] — each now a card of its own.
> - The constant $-4\pi$ is the engine of extinction: it does not degrade as the manifold shrinks, while the correction term is controlled by the scalar-curvature lower bound.
