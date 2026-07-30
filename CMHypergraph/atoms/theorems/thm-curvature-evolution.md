---
id: d9280cecb074
type: theorem
references:
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, ch. 3]]"
  - "[[ref-chowknopf|Chow & Knopf, ch. 6]]"
  - "[[ref-bamler-surgery|Bamler, Ricci flow with surgery, §2.4]]"
  - "[[ref-hamilton3mprc|the original computation]]"
---

# Theorem — Evolution equations of curvature

What the flow does to its own curvature: reaction–diffusion equations, with the Laplacian diffusing and a quadratic term reacting — the equations that every maximum-principle argument compares against.

## Statement

> [!theorem] Evolution equations of curvature
> Let $(M, g(t))$ be a [[def-ricci-flow|Ricci flow]]. Then:
>
> 1. the [[def-curvature-tensor|curvature tensor]] satisfies
> $$
> \partial_t\, {\operatorname{Rm}} \;=\; \triangle\, {\operatorname{Rm}} \;+\; Q({\operatorname{Rm}}),
> $$
> where $\triangle$ is the [[def-rough-laplacian|rough Laplacian]] on tensors and $Q({\operatorname{Rm}})$ is quadratic in ${\operatorname{Rm}}$, built from ${\operatorname{Rm}} \otimes {\operatorname{Rm}}$ by contractions with $g$ and $g^{-1}$ alone — the same expression on every manifold;
> 2. the [[def-scalar-curvature|scalar curvature]] satisfies
> $$
> \partial_t R \;=\; \triangle R \;+\; 2\, |{\operatorname{Ric}}|^2,
> $$
> with $\triangle$ the [[def-laplacian|Laplacian]], ${\operatorname{Ric}}$ the [[def-ricci-curvature|Ricci curvature]] and $|\cdot|$ the [[def-tensor-norm|tensor norm]]; in dimension three, consequently,
> $$
> \partial_t R \;\ge\; \triangle R + \tfrac{2}{3}\, R^2 .
> $$

## Notes

> [!note]- Notes (click to expand)
> - The structure is reaction–diffusion: $\triangle$ spreads curvature out, $Q$ concentrates it. Every preserved curvature condition and every lower bound in this network is a race between the two, refereed by [[thm-maximum-principle]] — whose "reaction ODE" is precisely $\tfrac{d}{dt}{\operatorname{Rm}} = Q({\operatorname{Rm}})$ with the diffusion deleted.
> - Direct consumers of conclusion 2: the mechanism of [[lem-scalar-curvature-lower-bound]] (compare with $y' = \tfrac23 y^2$) and, through the pinching set-up, [[thm-phi-pinching]]. Conclusion 1 feeds [[thm-shi-estimates]].
> - The dimension-three inequality uses $|{\operatorname{Ric}}|^2 \ge \tfrac{R^2}{3}$, an orthonormal-frame Cauchy–Schwarz. Proof debt — the analytic preliminaries: commuting derivatives and the second Bianchi identity.
> - **What $Q$ is, precisely.** Viewing the curvature as the symmetric operator ${\mathcal M}$ on $\Lambda^2$, Hamilton's computation gives $\partial_t {\mathcal M} = \triangle {\mathcal M} + {\mathcal M}^2 + {\mathcal M}^{\#}$, the $\#$ being the Lie-algebra square on $\Lambda^2 \cong \mathfrak{so}(3)$. The statement keeps only "quadratic" because that is the whole interface: every consumer — [[thm-shi-estimates]], the maximum-principle comparisons, [[thm-phi-pinching]] — uses the structure $\triangle + \text{quadratic}$ and nothing finer. The precise form belongs to the proof debt.
