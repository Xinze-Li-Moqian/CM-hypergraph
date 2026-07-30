---
id: 97584a726445
type: definition
references:
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, Ricci Flow and the Poincaré Conjecture, ch. 14 — the second chart type of Definition 14.2]]"
  - "[[def-14-2]]"
  - "[[def-14-3]]"
  - "[[ref-bamler-surgery|Bamler, Ricci flow with surgery, §7.1]]"
---

# Definition — exposed point

The points where new material is born: a surgery cap, at the moment it
is glued in, consists of points that exist from that time onward but
have no past.

## Statement

> [!definition] Exposed point
> Let ${\mathcal M}$ be a [[def-spacetime|space-time]], with time function $\mathbf{t}$ and vector field $\chi$, and let $x$ be a point of the time-slice $M_t$. The point $x$ is an *exposed point* if it is not a [[def-smooth-point|smooth point]] but has a *forward* product neighbourhood: an [[def-embedding|embedding]] $U \times [t, b)$ into ${\mathcal M}$ — with $U$ an open set of $M_t$ containing $x$ and $b > t$ — on which $\mathbf{t}$ is the projection to $[t, b)$ and the curves $\{y\} \times [t, b)$ are the integral curves of $\chi$.
>
> The *exposed region* of ${\mathcal M}$ is the set of its exposed points.

## Notes

> [!note]- Notes (click to expand)
> - The flow line of an exposed point continues forward in time but not backward: the point is *born* at its time. Failure of smoothness is exactly the failure of a backward extension.
> - In the flows constructed for the main theorems the exposed regions are the surgery caps, glued in at the singular times; the exposed region always sits inside singular slices, since near a regular time the space-time is a product.
