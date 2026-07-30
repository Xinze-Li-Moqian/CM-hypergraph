---
id: d2bbc913fe9b
type: definition
---

# Definition — singular time

## Statement

> [!definition] Singular time
> Let $({\mathcal M}, G)$ be a [[def-generalized-ricci-flow|generalized Ricci flow]]. A time $t$ is *regular* if for some $\epsilon > 0$ there is a [[def-diffeomorphism|diffeomorphism]] $M_t \times (t - \epsilon, t + \epsilon) \to \mathbf{t}^{-1}\big((t-\epsilon, t+\epsilon)\big)$ compatible with time and the vector field. A time is *singular* if it is not regular.

## Notes

> [!note]- Notes (click to expand)
> - **Synonym.** For a [[def-ricci-flow-with-surgery|Ricci flow with surgery]] the singular times are exactly the times at which surgery is performed — there they are also called *surgery times*. (A forward remark: that notion is defined using this one.)
> - **Intuition.** Between surgery times the flow is an ordinary smooth Ricci flow. At a surgery time the smooth evolution breaks down — curvature blows up somewhere — the manifold is cut along neck spheres and capped, and the flow restarts from the new slice. "Regular" is the precise version of "nothing happens here": a neighborhood of the time looks like a product $M_t \times (t-\epsilon, t+\epsilon)$.
> - That the surgery times form a *discrete* set (no accumulation) is not part of the definition — it is the content of clause 2 of [[thm-surgery-flow-exists]], proved by the volume argument.
