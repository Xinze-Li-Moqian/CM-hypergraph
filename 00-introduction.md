---
topic: minmax-ricci-flow-extinction
type: topic
section: "0"
date: 2026-07-25
tags: [ricci-flow, minimal-surfaces, 3-manifolds]
---
# The min-max route to finite extinction of Ricci flow

How sweepouts by $2$-spheres force the Ricci flow with surgery to die in finite time: the width, its evolution inequality, and the extinction they force.

Ricci flow evolves a metric by its own curvature, smoothing it the way heat smooths temperature, and with surgery it keeps running past the singularities it makes along the way. Geometrization asks what the flow settles into after infinite time, and answering that is the hardest part  of the proof: pieces of the manifold can collapse, and the collapsing has to be analysed.

For the Poincaré conjecture that analysis is avoidable. If the flow on such a manifold simply *dies* — if every solution reaches a time after which nothing is left — then there is no long-time behaviour to study. Colding and Minicozzi showed it does, by watching a single number shrink. They wrote it twice: eight pages that give the argument and quote the min-max input it needs [[ref-coldingminicozzi]], and a companion that proves that input [[ref-cm-width-extinction]]. This is the two together.

The number is the *width*: sweep the manifold by a family of $2$-spheres, measure the largest energy the family must pass through, and take the best family. It is a mountain-pass value, and the point is that the flow drives it down at a rate the manifold's own shrinking cannot slow.

## The result

The route answers a question of Perelman: on a $3$-manifold whose prime decomposition has no aspherical factors, the Ricci flow with surgery becomes extinct in finite time. The point, in Colding and Minicozzi's words:

> If one is interested in geometrization of a homotopy three-sphere (or, more generally, a three-manifold without aspherical summands) and knew that the Ricci flow became extinct in finite time, then one would not need to analyze what happens to the flow as time goes to infinity. Thus, in particular, one would not need collapsing arguments.

## The mechanism

Everything turns on one estimate. The *width* $W(g(t))$ is a min-max energy over sphere sweepouts; under the flow it decreases at a definite rate:

![[thm-width-evolution]]

The $-4\pi$ is topological — it is the Gauss–Bonnet constant of the sphere — so it does not weaken as the flow shrinks the manifold. A non-negative quantity forced to fall at such a rate cannot last:

![[cor-no-immortal-flow]]

With the topology that supplies a sweepout class and the compatibility with surgery, this is the extinction theorem:

![[thm-finite-time-extinction]]

The sections that follow build the estimate in order. First the vocabulary and the width itself: the [[01-preliminaries|terms]], then [[02-the-width|the min-max value]] and the two functionals that define it.

Then the machinery that makes the width a theorem about surfaces rather than a definition — [[03-harmonic-replacement|harmonic replacement]], the discrete downhill step; [[04-tightening-the-sweepout|tightening]], which applies it along a whole family at once; and [[05-bubbles-and-necks|bubbles and necks]], where the limit is taken and the energy is shown not to escape. This is the part the eight-page note states and the companion proves.

Then the argument proper: [[06-realization-by-minimal-spheres|minimal spheres realize the width]]; [[07-area-decay-of-minimal-spheres|their area decays]] under the flow; [[08-width-inequality-and-extinction|the width inequality and the extinction it forces]]; and [[09-reducible-case|the reducible case]], with the sharp rate for stable spheres.
