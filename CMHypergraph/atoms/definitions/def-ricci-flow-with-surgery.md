---
id: 40add2962838
type: definition
references:
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, Ricci Flow and the Poincaré Conjecture, ch. 14 — Definitions 14.7–14.8]]"
  - "[[def-14-7]]"
  - "[[def-14-8]]"
  - "[[ref-kleinerlott|Kleiner & Lott, Notes on Perelman's papers, §68 (Ricci flow with surgery)]]"
  - "[[ref-perelman2|Perelman, Ricci flow with surgery on three-manifolds, §4]]"
  - "[[ref-caozhu|Cao & Zhu, §7.3]]"
  - "[[ref-bamler-surgery|Bamler, Ricci flow with surgery, §7.1 — an equivalent formulation]]"
---

# Definition — Ricci flow with surgery

A Ricci flow that is allowed to survive its singularities: whenever curvature concentrates in a neck, the offending region is cut out, the wounds are sealed with caps, and the flow restarts from the repaired manifold — all packaged into a *single* smooth space-time, so that "the flow" remains one object even as its topology changes.

## Statement

> [!definition] [[def-generalized-ricci-flow|Ricci flow]] with surgery
> A *Ricci flow with surgery* is a pair $({\mathcal M}, G)$ in which ${\mathcal M}$ is a [[def-surgery-spacetime|surgery space-time]] and $G$ is a *horizontal metric* on it — a smoothly varying Riemannian metric $G(t)$ on the time-slices — satisfying
> $$
> {\mathcal L}_\chi\, G \;=\; -2 \operatorname{Ric}(G)
> $$
> at every point of ${\mathcal M}$.

## Notes

> [!note]- Notes (click to expand)
> - **Why one space-time, not a list of flows.** An equivalent naive description: a sequence of ordinary Ricci flows on intervals $[t_i, t_{i+1}]$, the initial slice of each obtained from the final slice of the previous one by surgery. The space-time packaging makes the objects that *cross* surgery times first-class citizens: paths in ${\mathcal M}$ for the noncollapsing and canonical-neighborhood arguments, curvature bounds stated once over all of ${\mathcal M}$, and the field $\chi$ transporting a point forward through surgeries for exactly as long as it survives.
> - **The horizontal metric.** $G$ lives on the codimension-one subbundle of $T{\mathcal M}$ tangent to the time-slices ($\chi$ spans the complementary line); its curvature, Ricci and scalar curvature at a point of $M_t$ are simply those of the Riemannian manifold $(M_t, G(t))$. The flow equation ${\mathcal L}_\chi G = -2\operatorname{Ric}(G)$ says exactly: each slice, transported along the flow of $\chi$, evolves by Ricci flow. At a singular slice the derivative is one-sided.
> - **What remains a debt here.** The *surgery assumptions* — surgery only in $\delta$-necks, caps modeled on the [[def-standard-solution|standard solution]], pinched slices — are the separate debt registered in [[notation]]; the chart-level axioms of the underlying space-time live on [[def-surgery-spacetime]].
