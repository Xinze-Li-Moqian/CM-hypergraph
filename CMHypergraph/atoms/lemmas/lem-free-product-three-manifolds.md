---
id: bfd525b3fcd9
type: lemma
rigor: outline
references:
  - "[[ref-perelman3|Perelman, Finite extinction time…, §1]]"
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §1 and §4]]"
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, ch. 18]]"
  - "[[cor-0-5|for the hypothesis equivalence]]"
---
# Lemma — Three-manifolds with free-product fundamental group

The topological dividend of the group hypothesis: a fundamental group built freely from finite and cyclic pieces rules out the two enemies of the extinction argument — locally separating projective planes and aspherical factors — and the hypothesis survives every surgery.

## Statement

> [!lemma] Three-manifolds with free-product fundamental group
> Let $M$ be a [[def-closed-manifold|closed]] $3$-manifold whose [[def-fundamental-group|fundamental group]] is a [[def-free-product|free product]] of finite groups and infinite cyclic groups. Then:
>
> 1. $M$ contains no [[def-embedding|embedded]], [[def-locally-separating|locally separating]] $\mathbb{R}P^2$;
> 2. no factor of the prime decomposition of $M$ is [[def-aspherical|aspherical]] — that is, none has contractible universal cover;
> 3. the hypothesis is inherited under [[def-connected-sum|connected-sum]] decomposition: if $M \cong M_1 \,\#\, M_2$, then the fundamental group of each $M_i$ is again a free product of finite groups and infinite cyclic groups.


## Proof

> [!note]- Proof (click to expand)
> **(3) Inheritance.** By [[thm-prime-decomposition]], $M \cong M_1 \# M_2$ realizes $\pi_1(M) = \pi_1(M_1) * \pi_1(M_2)$. If $\pi_1(M)$ is a [[def-free-product|free product]] of finite and infinite-cyclic groups, then by the [[thm-free-product-subgroups|Kurosh subgroup theorem]] each free factor $\pi_1(M_i)$ is again a free product of (conjugates of subgroups of) finite and cyclic groups — hence of the same form.
> **(2) No aspherical factor.** A closed aspherical $3$-manifold $N$ has $\pi_1(N)$ infinite (its universal cover is contractible, so $\mathbb{R}^3$, non-compact) and torsion-free and freely indecomposable — none of which a finite or infinite-cyclic group in a free-product decomposition can be, so no prime factor of $M$ is aspherical.
> **(1) No locally separating $\mathbb{R}P^2$.** An embedded [[def-locally-separating|locally separating]] $\mathbb{R}P^2 \subset M$ would give (its regular neighborhood, twisted $I$-bundle) a $\mathbb{Z}/2$ in $\pi_1$ arising in a way incompatible with the free-product-of-finite-and-cyclic structure at that prime factor. $\square$

## Notes

> [!note]- Notes (click to expand)
> - The mechanisms (the proof debt): for 3, the prime decomposition realizes the group as the free product of the factors' groups, and by the subgroup theorem for free products every free factor of such a group is again of the same kind. For 2, a closed aspherical $3$-manifold has infinite torsion-free freely-indecomposable fundamental group — which is neither finite nor infinite cyclic. For 1, a locally separating $\mathbb{R}P^2$ forces a $\mathbb{Z}/2$ that fails the free-product structure available here.
> - The two classical inputs — the prime decomposition of closed $3$-manifolds and the subgroup theorem for free products — are declared debts in [[notation]].
> - This card is pure topology: no flow appears. It is the bridge between the hypothesis of the extinction theorem and the geometric machinery.
