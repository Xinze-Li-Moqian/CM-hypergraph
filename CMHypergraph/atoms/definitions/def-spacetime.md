---
id: 61a8ed57a333
type: definition
references:
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, ch. 14 — the space-time formalism]]"
  - "[[ref-kleinerlott|Kleiner & Lott, §68]]"
---

# Definition — space-time of a flow

One manifold carrying a whole evolution: a time function slices it, a time field transports along it, and a metric lives on the slices.

## Statement

> [!definition] Space-time
> A *space-time* is a smooth $(n+1)$-manifold ${\mathcal M}$ together with
> 1. a smooth *time function* $\mathbf{t} : {\mathcal M} \to \mathbb{R}$ whose image is an interval;
> 2. a *time vector field* $\chi$ with $\chi(\mathbf{t}) = 1$;
> 3. a *horizontal metric* $G$ — a smoothly varying Riemannian metric on the level sets of $\mathbf{t}$.
>
> The level set $M_t = \mathbf{t}^{-1}(t)$ is the *time-$t$ slice*; each $(M_t, G|_{M_t})$ is a Riemannian $n$-manifold.

## Notes

> [!note]- Notes (click to expand)
> - **The product model.** ${\mathcal M} = M \times I$ with $\mathbf{t}$ the projection and $\chi = \partial_t$: there a horizontal metric is nothing but a path of metrics on $M$. The abstraction exists for the non-product case — the [[def-surgery-spacetime|surgery space-time]], whose slices change topology at singular times.
> - **$\chi$ is the identification between nearby slices.** Transporting along its flow is what "the same point at a later time" means; a point survives exactly as long as its flow line does. This is the object that lets curvature bounds and paths be stated across the whole evolution at once.
> - No equation yet: a space-time is the stage. Requiring the horizontal metric to evolve by the Ricci equation along $\chi$ is [[def-generalized-ricci-flow]].
