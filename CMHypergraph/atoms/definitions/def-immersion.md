---
id: beb310bb711f
type: definition
references:
  - "[[ref-leesmooth|Lee, Introduction to Smooth Manifolds, ch. 4]]"
  - "[[ref-docarmo|do Carmo, Riemannian Geometry, ch. 0]]"
---

# Definition — immersion

A map that is injective to first order: its differential never
collapses a direction, so the image is smooth wherever the map is —
even where it crosses itself.

## Statement

> [!definition] Immersion
> A smooth map $f : N \to M$ between manifolds is an *immersion* if its differential $df_p$ is injective at every point $p \in N$. An *immersed submanifold* is the image of an immersion, carrying the smooth structure of the domain.

## Notes

> [!note]- Notes (click to expand)
> - Weaker than an [[def-embedding|embedding]]: an immersion may self-intersect (a figure-eight is an immersed circle) and need not be a homeomorphism onto its image. Injectivity of $df$ controls only the local picture — the map is a local embedding near each point.
> - For a surface $\Sigma \looparrowright M$ this is exactly what is needed to pull back the ambient metric to a Riemannian metric on $\Sigma$ and to define its [[def-second-fundamental-form|second fundamental form]].
