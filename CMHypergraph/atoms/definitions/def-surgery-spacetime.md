---
id: 34e0d13a763e
type: definition
references:
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, Ricci Flow and the Poincaré Conjecture, ch. 14 — Definitions 14.1–14.6]]"
  - "[[def-14-1]]"
  - "[[def-14-2]]"
  - "[[def-14-3]]"
  - "[[def-14-4]]"
  - "[[def-14-6]]"
  - "[[ref-kleinerlott|Kleiner & Lott, Notes on Perelman's papers, §68]]"
  - "[[ref-bamler-surgery|Bamler, Ricci flow with surgery, §7.1]]"
---

# Definition — surgery space-time

The stage on which a flow that survives surgery lives: a space-time whose time-slices are allowed to change at finitely many moments — material may end, and new material may be born — while everything between those moments looks like an ordinary product.

## Statement

> [!definition] Surgery space-time
> A *surgery space-time* is a [[def-spacetime|space-time]] — a smooth manifold ${\mathcal M}$ carrying a time function $\mathbf{t}$ and a vector field $\chi$ with $\chi(\mathbf{t}) = 1$ — except that at a discrete set of [[def-singular-time|singular times]] the time-slices are allowed to change. Away from the singular slices every point is a [[def-smooth-point|smooth point]]; a singular slice may in addition contain [[def-exposed-point|exposed points]] and [[def-singular-point|singular points]]. The smooth and exposed points together form a smooth manifold with boundary, each boundary component contained in a single time-slice; within such a slice, the closure of the exposed region is bounded by the singular points.

## Notes

> [!note]- Notes (click to expand)
> ![[surgery-spacetime.svg|695]]
>
> - **The picture.** Between singular times the space-time is a product. At a singular time $T$ three things happen at once: a region of the manifold is *discarded* — its flow lines end just before $T$ and the space-time simply has no material there at time $T$; new material is *glued in*, forming the exposed region — points whose flow lines are born at $T$; and the frontier where new material meets the surviving part of the slice consists of the singular points. In the flows constructed for the main theorems the discarded regions are necks of blown-up curvature, the exposed regions are caps, and the frontier is a disjoint union of $2$-spheres — the spheres along which the necks were cut.
> - **Coexistence without contradiction.** The pre-surgery and post-surgery manifolds never occupy the same time-slice: what is removed lives on right-open time intervals and never reaches the singular time, while what replaces it exists from the singular time onward. This is the bookkeeping that lets one smooth manifold ${\mathcal M}$ carry the whole history.
> - **What remains a debt here.** The chart-level axioms — the three local models, their overlap conditions, and the glued tangent bundle — are the pool's [[def-14-1]] through [[def-14-8]]; they graduate with the surgery chapter.
