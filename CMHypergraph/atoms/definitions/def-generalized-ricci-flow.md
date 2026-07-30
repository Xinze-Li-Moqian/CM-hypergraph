---
id: 15407bcc3652
type: definition
references:
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, ch. 14]]"
  - "[[ref-kleinerlott|Kleiner & Lott, §68]]"
---

# Definition — generalized Ricci flow

Ricci flow stated on a space-time: the same equation, written as a Lie derivative, so that it keeps making sense when the underlying manifold is not a product.

## Statement

> [!definition] Generalized Ricci flow
> An *$n$-dimensional generalized Ricci flow* is a [[def-spacetime|space-time]] $({\mathcal M}, \mathbf{t}, \chi, G)$ whose horizontal metric satisfies
> $$
> {\mathcal L}_\chi\, G \;=\; -2 \operatorname{Ric}(G)
> $$
> at every point: each time-slice, transported along the flow of $\chi$, evolves by [[def-ricci-flow|Ricci flow]].

## Notes

> [!note]- Notes (click to expand)
> - On a product space-time $M \times I$ this is exactly an ordinary Ricci flow $\partial_t g = -2\operatorname{Ric}(g)$ — the generalized notion adds nothing until the topology changes.
> - The gain is at surgery: on a [[def-surgery-spacetime|surgery space-time]] the same one-line equation governs the whole object — that pairing is [[def-ricci-flow-with-surgery]]. Curvature bounds are stated once over ${\mathcal M}$, and the paths crossing surgery times that the noncollapsing and canonical-neighborhood arguments need become first-class citizens.
> - At a singular slice the Lie derivative is one-sided.
