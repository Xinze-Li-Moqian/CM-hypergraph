---
topic: minmax-ricci-flow-extinction
type: topic
section: "2"
---

# The width

The width is a min-max over *sweepouts* — one-parameter families of spheres running from a point to a point — measured by the [[def-dirichlet-energy|Dirichlet energy]] on the mapping space $C^0 \cap W^{1,2}(S^2, M)$ of continuous finite-energy maps ([[def-sobolev-space|Sobolev space]]).

![[def-sweepout-width]]

Abstractly, the width is a mountain-pass value — the one-parameter case of min-max over a compact parameter family. Two cards name the scheme the whole paper instantiates:

![[def-mountain-pass]]

![[def-minmax-value]]

The homotopy classes of sweepouts are what the topology feeds in: they are $\pi_1$ of the mapping space, hence $\pi_3$ of the manifold.

![[lem-sweepout-classes-are-pi3]]

A nontrivial class exists exactly when $\pi_3(M) \neq 0$ — the topological hypothesis of the extinction theorem.

## Energy or area

The width can be defined with either functional, and the extinction argument
needs both: the evolution inequality is proved for the energy, while the
comparison with minimal spheres is an area statement. They agree.

![[prop-energy-area-width-equal]]

The proof runs through the conformal parametrization of a metric on $S^2$,
which has to depend continuously on the metric for the sweepout to survive
the change of functional:

![[lem-conformal-parametrization-continuous]]
