---
id: 3db4febc7d6b
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §4]]"
  - "[[ref-perelman3|Perelman, Finite extinction time…, §1]]"
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, §18.1]]"
---

# Lemma — Non-aspherical manifolds carry a sweepout class

The topological fuel of the width argument: whenever no factor is aspherical, the third homotopy group is nontrivial, and a nontrivial family of spheres exists to sweep the manifold out.

## Statement

> [!lemma] Non-aspherical manifolds carry a sweepout class
> Let $M$ be a [[def-closed-manifold|closed]] $3$-manifold, not a point, no factor of whose prime decomposition is [[def-aspherical|aspherical]]. Then $\pi_3(M) \neq 0$; equivalently, there is a nontrivial class of [[def-sweepout-width|sweepouts]] of $M$.


## Proof

> [!note]- Proof (click to expand)
> By [[lem-sweepout-classes-are-pi3]] a nontrivial sweepout class exists iff $\pi_3(M) \neq 0$; so it suffices to show $\pi_3(M) \neq 0$. Split by $\pi_2$:
> **Case $\pi_2(M) = 0$.** No essential sphere, so (with no aspherical factor) $M$ is a connected sum of spherical space forms and $S^2$-bundles... in the homotopy-sphere case $M$ is simply connected with $\pi_2 = 0$, so its universal cover is $M$ itself, a closed simply connected $3$-manifold; by the [[thm-hurewicz|Hurewicz theorem]] $\pi_3(M) \cong H_3(M) \cong \mathbb{Z}$ (the fundamental class), nonzero.
> **Case $\pi_2(M) \neq 0$.** By the [[thm-sphere-theorem|sphere theorem]] there is an embedded essential $2$-sphere; the resulting $S^2 \times \mathbb{R}$ or $S^2\tilde\times \mathbb{R}$ geometry in a summand carries a nontrivial element of $\pi_3$ (the Hopf map into the $S^2$ factor composed with the sweep), so $\pi_3(M) \neq 0$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - The mechanisms (the proof debt), by cases on $\pi_2$: if $\pi_2(M) = 0$, the hypothesis forces the fundamental group to be finite, the universal cover is a closed [[def-simply-connected|simply connected]] $3$-manifold, and the Hurewicz theorem gives $\pi_3 \cong H_3 \cong \mathbb{Z}$; if $\pi_2(M) \neq 0$, the sphere theorem provides an essential embedded sphere and the resulting sphere geometry again yields a nontrivial $\pi_3$.
> - The equivalence between $\pi_3(M) \neq 0$ and the existence of a nontrivial sweepout class is [[lem-sweepout-classes-are-pi3]].
> - Sphere theorem and Hurewicz theorem are declared debts in [[notation]].
