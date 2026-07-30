---
id: 4e48480d2dd4
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §1, the paragraph before Proposition 3.1]]"
  - "[[ref-hatcher|the adjunction is standard, e.g. Algebraic Topology]]"
---

# Lemma — Sweepout classes are the third homotopy group

The bridge from topology to min-max: a sweepout is a loop in the space
of spheres, so its homotopy classes are the fundamental group of that
mapping space — which is the third homotopy group of the manifold.

## Statement

> [!lemma] Sweepout classes are $\pi_3$
> Let $M$ be a manifold and let $\Omega = C^0 \cap W^{1,2}(S^2, M)$ be the space of finite-[[def-dirichlet-energy|energy]] continuous maps $S^2 \to M$, based at the constant maps. Then the homotopy classes of [[def-sweepout-width|sweepouts]] — loops in $\Omega$ based at the constants — form the [[def-fundamental-group|fundamental group]] $\pi_1(\Omega)$, and there is a natural isomorphism
> $$
> \pi_1\big(\Omega\big) \;\cong\; \pi_3(M) .
> $$
> In particular, a nontrivial sweepout class exists if and only if $\pi_3(M) \neq 0$.


## Proof

> [!note]- Proof (click to expand)
> The based mapping-space adjunction: for based spaces, $\operatorname{Map}_*(S^n, Y)$ has $\pi_k(\operatorname{Map}_*(S^n, Y)) \cong \pi_{k+n}(Y)$, because a based map $S^k \to \operatorname{Map}_*(S^n, Y)$ is the same as a based map $S^k \wedge S^n = S^{k+n} \to Y$ (exponential law / smash-hom adjunction). A [[def-sweepout-width|sweepout]] is a path in $\Omega = C^0\cap W^{1,2}(S^2, M)$ from the constant maps to themselves — i.e. a based loop, a based map $S^1 \to \operatorname{Map}_*(S^2, M)$ — so its homotopy classes form $\pi_1(\Omega)$. Applying the adjunction with $k = 1$, $n = 2$, $Y = M$:
> $$
> \pi_1(\Omega) \;\cong\; \pi_1(\operatorname{Map}_*(S^2, M)) \;\cong\; \pi_{1+2}(M) = \pi_3(M).
> $$
> The Sobolev completion $C^0 \cap W^{1,2}$ has the same weak homotopy type as continuous maps (smooth/continuous maps are dense and the inclusion is a homotopy equivalence on each component), so the $\pi_1$ is unchanged. Hence nontrivial sweepout classes exist iff $\pi_3(M) \neq 0$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - **Whose $\pi_1$ this is.** Not $S^2$'s and not $M$'s: the space $\Omega$ has one *point* per entire map $S^2 \to M$, so it is an infinite-dimensional space of spheres-in-$M$, and the question $\pi_1(\Omega)$ asks is about *families*: can a given one-parameter family of spheres be contracted, through families of finite-energy spheres, to a constant family? A [[def-sweepout-width|sweepout]] is exactly a loop in this space, and $[\beta]$ is the obstruction to contracting the whole family at once.
> - **Closing up at the constants.** The endpoints $\beta(0), \beta(1)$ are constant maps, and the constant maps form a copy of $M$ inside $\Omega$; since $M$ is connected, any sweepout closes up to a based loop. When $\pi_1(M) \neq 1$ the closing path is a genuine choice: unbased sweepout classes are $\pi_3(M)$ *modulo the $\pi_1(M)$-action*, not $\pi_3(M)$ itself. The distinction is harmless downstream — the orbit of a nonzero element is nonzero, and existence of a nontrivial class is all the width consumes.
> - **What is at stake.** For the trivial class the width vanishes: the constant family lies in $[\beta]$, so $W(g, [\beta]) = 0$ and the min-max has nothing to grip. A nontrivial class is a family that cannot be contracted, forcing every competitor to pass through a sphere of definite energy; that $W > 0$ then actually holds is conclusion 1 of [[prop-minmax-minimal-spheres]], a theorem rather than part of the definition.
> - The isomorphism is the based mapping-space adjunction: $\pi_k(\operatorname{Map}_*(S^n, M)) \cong \pi_{k+n}(M)$, here with $k = 1$, $n = 2$. The Sobolev completion does not change the homotopy type, so $W^{1,2}$ maps give the same $\pi_1$ as continuous ones.
> - This is the hinge between the two halves of the extinction argument: [[lem-nonaspherical-sweepout-class]] produces the nontrivial element of $\pi_3(M)$ from the topology of $M$, and this lemma turns it into the nontrivial sweepout class that [[prop-minmax-minimal-spheres]] and [[thm-width-evolution]] consume.
> - Proof debt — classical algebraic topology: the mapping-space adjunction and the density of smooth maps in the Sobolev space.
