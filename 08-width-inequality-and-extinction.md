---
topic: minmax-ricci-flow-extinction
type: topic
section: "8"
---

# The width inequality and extinction

## The two evolution facts

The estimate needs two facts about the flow. The rate constant comes from the evolution of scalar curvature:

![[thm-curvature-evolution]]

and its maximum-principle consequence — the clock behind the fading correction:

![[lem-scalar-curvature-lower-bound]]

## The width inequality

These assemble into the width inequality, proved by running a near-optimal time-$t_0$ sweepout as a competitor at later times:

![[thm-width-evolution]]

The three constants — which matter and which does not:

![[rem-width-constants]]

## Finite extinction

Finally the inequality forces extinction — pure calculus:

![[lem-width-inequality-forces-extinction]]

which cashes out as [[cor-no-immortal-flow]] for smooth flows and, with the topology and surgery compatibility of the next section, as [[thm-finite-time-extinction]].
