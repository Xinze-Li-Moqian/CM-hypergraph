---
id: 15fa9f1153d8
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §2, equation (2.1)]]"
  - "[[ref-hamiltonsurvey|the computation is Hamilton's]]"
---

# Lemma — First variation of area under Ricci flow

How a fixed surface's area responds when the ambient metric flows:
each area element shrinks at a rate read off from the ambient
curvature across the surface's normal.

## Statement

> [!lemma] First variation of area under Ricci flow
> Let $(M, g(t))$ be a [[def-ricci-flow|Ricci flow]] on a $3$-manifold and $\Sigma \subset M$ a fixed closed [[def-immersion|immersed]] surface with unit normal $\mathbf{n}$. Then
> $$
> \frac{d}{dt}\Big|_{t=0} \operatorname{Area}_{g(t)}(\Sigma) \;=\; -\int_\Sigma \big[\, R - \operatorname{Ric}(\mathbf{n}, \mathbf{n}) \,\big],
> $$
> where $R$ is the [[def-scalar-curvature|scalar curvature]] and $\operatorname{Ric}$ the [[def-ricci-curvature|Ricci curvature]] of $M$.


## Proof

> [!note]- Proof (click to expand)
> The surface $\Sigma$ is fixed; only the metric moves, by $\partial_t g = -2\operatorname{Ric}$. The area of $\Sigma$ in $g(t)$ is $\int_\Sigma d\mathrm{vol}_{g(t)|_\Sigma}$, and the area element of an induced metric varies by half the trace of the variation of the induced metric:
> $$
> \frac{d}{dt}\Big|_{t=0} d\mathrm{vol}_{g(t)|_\Sigma} = \tfrac12\, \operatorname{tr}_\Sigma\big(\partial_t g|_\Sigma\big)\, d\mathrm{vol} = \tfrac12\,\operatorname{tr}_\Sigma(-2\operatorname{Ric})\, d\mathrm{vol} = -\operatorname{tr}_\Sigma\operatorname{Ric}\; d\mathrm{vol}.
> $$
> For an orthonormal frame $e_1, e_2, \mathbf{n}$ adapted to $\Sigma$, $\operatorname{tr}_\Sigma\operatorname{Ric} = \operatorname{Ric}(e_1,e_1) + \operatorname{Ric}(e_2,e_2) = \big(\operatorname{Ric}(e_1,e_1)+\operatorname{Ric}(e_2,e_2)+\operatorname{Ric}(\mathbf{n},\mathbf{n})\big) - \operatorname{Ric}(\mathbf{n},\mathbf{n}) = R - \operatorname{Ric}(\mathbf{n},\mathbf{n})$, since the full trace of $\operatorname{Ric}$ is the [[def-scalar-curvature|scalar curvature]] $R$. Integrating over $\Sigma$,
> $$
> \frac{d}{dt}\Big|_{t=0}\operatorname{Area}(\Sigma) = -\int_\Sigma \big[R - \operatorname{Ric}(\mathbf{n},\mathbf{n})\big]. \qquad \square
> $$

## Notes

> [!note]- Notes (click to expand)
> - The surface does not move — only $g(t)$ does. The area form of the induced metric changes at half the trace (over $\Sigma$) of $\partial_t g = -2\operatorname{Ric}$, and $\operatorname{tr}_\Sigma \operatorname{Ric} = \operatorname{Ric}(e_1,e_1) + \operatorname{Ric}(e_2,e_2) = R - \operatorname{Ric}(\mathbf{n},\mathbf{n})$ for an orthonormal frame $e_1, e_2, \mathbf{n}$ — the identity behind the formula.
> - This is CM's (2.1); it holds for *any* surface, minimality is used only afterward. Proof debt: the first-variation computation, classical.
