---
topic: minmax-ricci-flow-extinction
type: topic
section: "3"
---

# Harmonic replacement

The width is a min-max value, and the standard way to realize such a value is to push a family downhill until it stops moving: what it converges to is critical. For maps into a manifold the gradient flow is the harmonic map heat flow, which develops singularities of its own. The replacement construction avoids the flow entirely — it is a discrete downhill step, applied on small balls, and everything in this section is about making it behave well enough to run along a whole family at once.

## The threshold

Below a fixed energy, the Dirichlet problem on a disc is as well behaved as it could be: a minimizer exists and is the only critical point.

![[thm-sacks-uhlenbeck]]

That constant is what makes the whole scheme possible. On a ball where the map carries less energy than the threshold, "replace by the minimizer" is unambiguous.

## The step

![[def-harmonic-replacement]]

The step is only useful if it buys something quantitative. It does: the energy it saves controls how far the map was from harmonic in the first place, so a map that cannot be improved is nearly harmonic.

![[lem-harmonic-replacement-energy]]

Two analytic inputs stand behind that estimate. The nonlinearity in the harmonic map equation is a Jacobian, and Wente's estimate is what makes a Jacobian better than the product of its factors suggests:

![[lem-wente]]

![[lem-hardy-holomorphic]]

## Along a family

A sweepout is a continuous path of maps, so the replacement must be continuous in the map — otherwise improving each slice separately would tear the family apart.

![[lem-harmonic-replacement-continuity]]

One more property is needed, and it is the one that makes the bookkeeping in the next section possible: replacing on two collections of balls in turn cannot be much worse than the better of the two.

![[lem-harmonic-replacement-gap]]
