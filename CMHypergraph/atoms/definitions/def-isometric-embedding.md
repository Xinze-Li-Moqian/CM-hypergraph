---
id: 063cfc22f517
type: definition
references:
  - "J. Nash, The imbedding problem for Riemannian manifolds (1956)"
---

# Definition — isometric embedding

An embedding that preserves the metric: distances and angles on the
submanifold agree with those it inherits from the ambient space — the
way a closed manifold sits in Euclidean space to do analysis on it.

## Statement

> [!definition] Isometric embedding
> A smooth [[def-embedding|embedding]] $\iota : (M, g) \to (\tilde M, \tilde g)$ of Riemannian manifolds is *isometric* if it pulls back the ambient metric to the given one, $\iota^* \tilde g = g$ — equivalently $\langle d\iota(X), d\iota(Y)\rangle_{\tilde g} = \langle X, Y\rangle_g$ for all tangent $X, Y$.

## Notes

> [!note]- Notes (click to expand)
> - Nash's theorem: every closed Riemannian manifold admits an isometric embedding into some $\mathbb{R}^N$. This is why the harmonic-map analysis may treat the target $M \subset \mathbb{R}^N$ as a submanifold of Euclidean space — writing $\triangle u$, the [[def-second-fundamental-form|second fundamental form]] $A$, and the [[def-tension-field|tension field]] via the ambient structure.
> - Taken as a standing setup ("$M \subset \mathbb{R}^N$ isometrically") throughout.
