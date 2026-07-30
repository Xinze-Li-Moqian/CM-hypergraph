---
id: 447f02a832f9
type: definition
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §3 (\"Harmonic replacement\")]]"
  - "[[ref-sacksuhlenbeck|Sacks & Uhlenbeck — existence, uniqueness and smoothness of small-energy minimizers; source of the threshold constant]]"
  - "C. B. Morrey, Multiple Integrals in the Calculus of Variations (1966)."
---

# Definition — harmonic replacement

Locally minimize, keep the rest: inside a ball, swap a map for the
energy-minimizer with the same boundary values; outside, leave it
unchanged. The one move the tightening iterates.

## Statement

> [!definition] Harmonic replacement
> Let $u : S^2 \to M$ be a $C^0 \cap W^{1,2}$ map and $\mathcal{B}$ a finite collection of disjoint closed balls in $S^2$ on each of which $u$ has small [[def-dirichlet-energy|energy]]. The *harmonic replacement* $H(u, \mathcal{B})$ is the map equal to $u$ outside $\cup_{\mathcal{B}} B$ and, on each ball $B \in \mathcal{B}$, equal to the energy-minimizing ([[def-weakly-harmonic-map|weakly harmonic]]) map with the same boundary values $u|_{\partial B}$. For two collections, $H(u, \mathcal{B}_1, \mathcal{B}_2)$ replaces first on $\mathcal{B}_1$, then on $\mathcal{B}_2$.

## Notes

> [!note]- Notes (click to expand)
> - Small energy is what makes it well-defined and single-valued: below the [[thm-sacks-uhlenbeck|Sacks–Uhlenbeck]] threshold $\epsilon_{SU}$ the energy-minimizing map with given boundary values exists, is unique, and is smooth.
> - Harmonic replacement never raises energy, and by the strict convexity of energy near a harmonic map — the gap estimate of [[lem-harmonic-replacement-energy]] — it lowers energy by a definite amount unless $u$ was already harmonic. Iterating it is the *energy-decreasing map* [[thm-energy-decreasing-map]]; the two-collection gap is quantified by [[lem-harmonic-replacement-gap]].
