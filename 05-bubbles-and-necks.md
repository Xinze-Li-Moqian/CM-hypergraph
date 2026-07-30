---
topic: minmax-ricci-flow-extinction
type: topic
section: "5"
---

# Bubbles, necks, and varifold limits

Take a sequence of slices that is almost harmonic and almost area-maximizing, and ask what it converges to. Energy concentrates at finitely many points; rescaling at each recovers a harmonic sphere. The limit is therefore not one map but a body map together with finitely many bubbles.

![[def-bubble-convergence]]

The whole difficulty of the statement is clause (B4): that no energy is lost. The bubbles and the body are joined by long thin cylinders — the necks — and a priori energy can disappear into them, leaving a limit that carries strictly less area than the sequence. If that happened the min-max value would not be attained and the argument would collapse at its first step.

## Nothing survives in a long neck

The neck estimate is a decay statement, and it is proved by watching the *angular* part of the energy along the cylinder. For a harmonic map that quantity satisfies a differential inequality that forces growth in both directions:

![[lem-cylinder-angular-differential-inequality]]

A non-negative function whose second derivative is bounded below by itself cannot stay small in the middle and small at both ends:

![[lem-ode-comparison-sinh]]

Together they say a long harmonic cylinder of small energy has almost no angular energy in its middle — so the map there is almost independent of the angle, and a map independent of the angle carries no area:

![[lem-harmonic-cylinder-decay]]

The maps in the sequence are only *almost* harmonic, so the estimate has to survive that perturbation, which is where the tightening of the previous section pays off:

![[lem-almost-harmonic-cylinder-decay]]

## The compactness theorem

![[thm-almost-minimizing-compactness]]

## From bubbles to varifolds

Bubble convergence is a statement about maps; the extinction argument compares *surfaces*. The bridge is that the associated varifolds converge to the sum of the limit pieces — so a near-maximal slice really is close, as a surface, to a union of minimal spheres.

![[thm-bubble-implies-varifold]]

One last output of the min-max, not consumed by the extinction argument but part of what the scheme produces: a one-parameter family can only produce spheres of low index.

![[thm-micallef-moore-index]]
