---
id: 164f541303fb
type: definition
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §1]]"
  - "[[ref-perelman3|Perelman, Finite extinction time…, §1]]"
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, ch. 18]]"
---

# Definition — sweepout and width

Sweep the manifold by a one-parameter family of 2-spheres, from a point to a point; somewhere in the middle the family must pass through a large sphere. The width is the smallest possible size of that unavoidable largest sphere.

## Statement

> [!definition] Sweepout and width
> Let $(M, g)$ be a [[def-closed-manifold|closed]] Riemannian $3$-manifold. A *sweepout* is a continuous map
> $$
> \beta : [0, 1] \longrightarrow C^0 \cap W^{1,2}(S^2, M)
> $$
> such that $\beta(0)$ and $\beta(1)$ are constant maps. For a homotopy class $[\beta]$ of sweepouts, the *width* is
> $$
> W(g, [\beta]) \;=\; \min_{\gamma \in [\beta]} \, \max_{s \in [0,1]} \, E(\gamma(s)),
> $$
> where $E$ is the [[def-dirichlet-energy|energy]] and $W^{1,2}(S^2, M)$ the [[def-sobolev-space|Sobolev space]] of maps.

## Notes

> [!note]- Notes (click to expand)
> - **The mapping space.** $C^0 \cap W^{1,2}(S^2, M)$ is the space of continuous maps $S^2 \to M$ with square-integrable first derivatives — the natural domain of the [[def-dirichlet-energy|energy]], large enough to contain the sweepouts and their limits, small enough that energy is defined. (Sources also write $L^2_1$ for $W^{1,2}$; the two notations are the same [[def-sobolev-space|Sobolev space]].) A sweepout with constant endpoints is a loop in this space, so its homotopy classes form $\pi_1$ of it.
>
> - A sweepout with constant endpoints is a loop in the mapping space based at the constants; its homotopy classes form $\pi_1$ of that space, which is $\pi_3(M)$ — this identification is [[lem-sweepout-classes-are-pi3]], and a nontrivial class exists exactly when $\pi_3(M) \neq 0$.
> - $W \ge 0$ always; positivity of $W$ for a nontrivial class is a theorem (part of the min-max realization), not part of the definition.
> - By [[prop-energy-area-width-equal]] the width may equivalently be defined with $\operatorname{Area}$ in place of $E$; energy is used because it is better behaved under limits.
> - The width is the min-max shadow of the geometry: under Ricci flow it satisfies a differential inequality that no immortal flow can sustain.
