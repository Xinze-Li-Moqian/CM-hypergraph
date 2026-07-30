---
id: 5deedd60ce7b
type: definition
references:
  - "[[ref-hamilton3mprc|Hamilton, Three-manifolds with positive Ricci curvature — where the equation is introduced]]"
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, ch. 3]]"
  - "[[ref-chowknopf|Chow & Knopf, chs. 2–3]]"
  - "[[ref-bamler-surgery|Bamler, Ricci flow with surgery, §2.1]]"
---

# Definition — Ricci flow

The heat equation for Riemannian metrics: the metric moves against its own Ricci curvature, so positively curved directions contract and negatively curved ones expand.

## Statement

> [!definition] Ricci flow
> Let $M$ be a smooth manifold. A *Ricci flow* on $M$ is a smooth one-parameter family of Riemannian metrics $g(t)$, $t$ in an interval $I \subseteq \mathbb{R}$, satisfying
> $$
> \partial_t\, g(t) \;=\; -2 \operatorname{Ric}\big(g(t)\big),
> $$
> where $\operatorname{Ric}$ is the [[def-ricci-curvature|Ricci curvature]] of $g(t)$.

## Notes

> [!note]- Notes (click to expand)
> - The equation is only weakly parabolic — the degeneracy is pure diffeomorphism gauge — and [[thm-short-time-existence]] gives unique short-time solvability on closed manifolds after the DeTurck fix.
> - The model collapse: on an Einstein metric with $\operatorname{Ric} = \lambda g$ the flow just rescales, $g(t) = (1 - 2\lambda t)\, g(0)$; the round $S^3$ dies at $t = 1/(2\lambda)$ — extinction in miniature, and the reason a $1/(t+C)$ correction haunts every estimate.
> - Symmetries the arguments lean on: diffeomorphism invariance and [[lem-rescaling-invariance|parabolic rescaling]] — zoom space by $\lambda$, time by $\lambda^2$.
> - The space-time repackaging — slices, a time field, and the same equation as a Lie-derivative identity, so that it survives topology change — is [[def-generalized-ricci-flow]].
