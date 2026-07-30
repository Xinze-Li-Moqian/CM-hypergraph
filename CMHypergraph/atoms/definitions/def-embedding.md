---
id: 133eea9b7287
type: definition
references:
  - "[[ref-leesmooth|Lee, Introduction to Smooth Manifolds, ch. 5]]"
  - "[[ref-docarmo|do Carmo, ch. 0]]"
---

# Definition — embedding

A faithful copy of one manifold inside another: no collapsing of
directions, no self-crossings, and no sneaking back arbitrarily close to
itself.

## Statement

> [!definition] Embedding
> A smooth map $f : N \to M$ is an *embedding* if $df$ is injective at every point (an [[def-immersion|immersion]]) and $f$ is a homeomorphism onto its image with the subspace topology. An *embedded submanifold* of $M$ is the image of an embedding.

## Notes

> [!note]- Notes (click to expand)
> - **Picture.** Three circles mapped into the plane:
>   ![[embedding.svg]]
> - The three failures are independent: collapsing kills the immersion condition, the figure-eight kills injectivity, and a curve spiraling into a limit is injectively immersed but its image topology is not that of the circle.
> - For compact $N$, an injective immersion is automatically an embedding.
