---
id: 887bed206587
type: definition
references:
  - "[[ref-hatcher|Hatcher, Algebraic Topology, §1.B]]"
---

# Definition — aspherical manifold

A space whose homotopy theory is entirely group theory: every sphere of dimension two or more contracts, so the fundamental group is the only invariant left standing.

## Statement

> [!definition] Aspherical manifold
> A connected manifold $M$ is **aspherical** if $\pi_n(M) = 0$ for every $n \ge 2$ — equivalently, if its universal cover is contractible.

## Notes

> [!note]- Notes (click to expand)
> - **The equivalence.** A covering projection induces isomorphisms on $\pi_n$ for $n \ge 2$, so the universal cover $\widetilde M$ is [[def-simply-connected|simply connected]] with all higher homotopy groups those of $M$; if these vanish, every homotopy group of $\widetilde M$ vanishes and Whitehead's theorem contracts it. The converse is the same isomorphism read backwards. Aspherical spaces are exactly the $K(\pi, 1)$'s — classifying spaces of their fundamental groups.
> - **For closed $3$-manifolds** the condition is checkable: $M$ is aspherical iff it is irreducible with infinite [[def-fundamental-group|fundamental group]] — an essential sphere would survive in $\pi_2$ (by the [[thm-sphere-theorem|sphere theorem]] read backwards), and a finite group forces the universal cover to be a compact homotopy sphere. Hyperbolic manifolds and $T^3$ are aspherical; $S^3$, the [[def-spherical-space-form|spherical space forms]] and the two [[def-s2-bundle-over-s1|sphere bundles over the circle]] are not.
> - **Where it enters this graph: negatively.** [[lem-nonaspherical-sweepout-class]] turns "no aspherical prime factor" into $\pi_3(M) \neq 0$ — the fuel of the width argument; [[lem-free-product-three-manifolds]] (conclusion 2) shows the free-product group hypothesis rules aspherical factors out, since a closed aspherical $3$-manifold has infinite, torsion-free, freely indecomposable fundamental group. Perelman's extinction hypothesis is stated in exactly these terms.
> - Higher homotopy groups $\pi_n$ are declared ground notions (see [[notation]]).
