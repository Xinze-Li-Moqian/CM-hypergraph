---
topic: minmax-ricci-flow-extinction
type: topic
section: "9"
---

# The reducible case and the sharp rate

For a reducible $M$ the prime factors split off in uniformly bounded time. The topological inputs — that the free-product hypothesis rules out the enemies and is inherited under connected sum, and that non-aspherical factors carry a sweepout class — carry the width argument across the decomposition.

![[lem-free-product-three-manifolds]]

![[lem-nonaspherical-sweepout-class]]

That the argument survives the surgery times — surgeries only remove components or lower the width — is the last ingredient.

![[lem-surgery-preserves-width-inequality]]

**The stable-sphere route.** In each non-trivial prime factor one tracks a $2$-sphere not bounding a $3$-ball — hence a *stable* minimal sphere in its isotopy class — whose area must reach zero in finite time. The sharp lower rate this needs is the $-16\pi$ bound proved below.

## The sharp −16π rate for index one

The sharp *lower* rate for index-one minimal spheres, by adapting Hersch's theorem. Hersch's inequality — sharp on the round sphere — is proved by balancing [[def-conformal-map|conformal]] coordinates against a first [[def-eigenvalue|eigenfunction]] and evaluating by conformal invariance and the round spectrum.

![[lem-hersch-balancing]]

![[lem-dirichlet-conformal-invariance]]

![[lem-round-sphere-spectrum]]

![[thm-hersch]]

The index hypothesis converts, on the orthogonal complement of the unstable direction, into a stability inequality; fed the balanced coordinates and closed by Hersch, it caps the stability integral at $8\pi$ — and hence the area-decay rate at $-16\pi$.

![[lem-second-eigenvalue-test]]

![[lem-area-decay-index-one]]
