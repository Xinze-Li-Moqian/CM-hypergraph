---
topic: minmax-ricci-flow-extinction
type: topic
section: "4"
---

# Tightening the sweepout

The goal of this section is a single statement: any sweepout can be replaced by a homotopic one, no more energetic anywhere, whose *near-maximal* slices are almost harmonic. Once that is available, a minimizing sequence of sweepouts has near-maximal slices that are almost harmonic and almost area-maximizing — exactly the hypotheses the compactness theorem of the next section wants.

The difficulty is not improving one slice; it is improving all of them at once, continuously, without raising the energy anywhere. Three ingredients do it.

## Slices can be smoothed first

![[lem-sweepout-density]]

## How much a slice can be improved

![[def-energy-improvement]]

A slice is harmonic exactly when its improvement is zero, so the improvement is a measure of failure — and, crucially, a measure that does not collapse at a single parameter value:

![[lem-nonharmonic-interval]]

That is what turns a pointwise choice into a continuous one: around every non-harmonic slice there is an interval on which the available improvement stays comparable, so a finite cover of the parameter interval suffices.

## A continuous choice of balls

![[lem-good-balls]]

The clause that matters is *at most two are positive at a time*: the family of replacements is built from a partition of unity with overlaps of order two, and the two-ball gap of the previous section is what controls the overlap.

## The output

![[def-almost-harmonic-map]]

![[thm-energy-decreasing-map]]

The map $\Psi$ is the quantitative content: a slice whose energy is within $\Psi(\nu)$ of the maximum is $\nu$-almost harmonic. Letting the sweepout run down a minimizing sequence sends $\nu \to 0$.
