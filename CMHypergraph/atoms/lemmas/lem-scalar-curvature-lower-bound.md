---
id: b69be57535f2
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §1]]"
  - "[[ref-hamilton3mprc|the evolution equation and maximum principle are Hamilton's]]"
  - "[[ref-bamler-surgery|Bamler, Ricci flow with surgery, §2.5]]"
---

# Lemma — Scalar curvature bounded below by the flow clock

The worst scalar curvature improves like $-1/t$: whatever the initial metric, after time $t$ the scalar curvature is no worse than $-\tfrac{3}{2}\big/(t + C)$ — the flow forgets negative curvature at a
universal rate.

## Statement

> [!lemma] Scalar curvature lower bound
> Let $(M, g(t))$, $t \in [0, T)$, be a [[def-ricci-flow|Ricci flow]] on a [[def-closed-manifold|closed]] $3$-manifold. Then there is $C = C(g(0)) > 0$ such that the [[def-scalar-curvature|scalar curvature]] satisfies
> $$
> \min_M R(\cdot, t) \;\ge\; -\frac{3}{2\,(t + C)} \qquad \text{for all } t \in [0, T).
> $$


## Proof

> [!note]- Proof (click to expand)
> By [[thm-curvature-evolution]] the scalar curvature evolves by $\partial_t R = \triangle R + 2|\operatorname{Ric}|^2$. In dimension three $|\operatorname{Ric}|^2 \ge \tfrac13 R^2$ (an orthonormal-frame Cauchy–Schwarz: the trace of $\operatorname{Ric}$ is $R$, so its squared norm is at least $R^2/3$), hence
> $$
> \partial_t R \;\ge\; \triangle R + \tfrac23 R^2 .
> $$
> Let $\rho(t) = \min_M R(\cdot, t)$. At an interior spatial minimum $\triangle R \ge 0$, so by the scalar [[thm-maximum-principle|maximum principle]] $\rho$ satisfies the differential inequality $\rho' \ge \tfrac23 \rho^2$ in the sense of forward difference quotients (compared against the ODE). The ODE $y' = \tfrac23 y^2$ with $y(0) = \rho(0) < 0$ has solution $y(t) = -\tfrac{3}{2(t + C)}$ where $C = -\tfrac{3}{2\rho(0)} > 0$; since $\rho' \ge \tfrac23\rho^2$ and $\rho(0) = y(0)$, comparison gives $\rho(t) \ge y(t) = -\tfrac{3}{2(t+C)}$ for all $t$. (If $\rho(0) \ge 0$ then $\rho$ stays $\ge 0$ and the bound holds trivially with any $C$.) $\square$
## Notes

> [!note]- Notes (click to expand)
> - The mechanism (the proof debt): the scalar curvature evolves by the equation of [[thm-curvature-evolution]], giving $\partial_t R \ge \triangle R + \tfrac{2}{3} R^2$ in dimension three; the maximum principle compares $\min_M R$ with the solution of the ODE $y' = \tfrac{2}{3} y^2$, which is exactly $-\tfrac{3}{2}/(t + C)$.
> - The constant $\tfrac{3}{2}$ here becomes the $\tfrac{3}{4}$ in the width inequality after multiplication by $\operatorname{Area}/2$ — both constants matter for extinction; $C$ does not.
