---
id: 7b38eb569b59
type: theorem
references:
  - "[[ref-jost|Jost, Two-dimensional geometric variational problems, Theorem 4.2.1; proof §§4.2–4.3]]"
  - "[[ref-coldingminicozzi|cited as the min-max input in Colding & Minicozzi, §3]]"
---

# Theorem — Min-max for harmonic maps with energy identity

The general saddle-point existence theorem behind the width: minimizing the maximal energy of a family of maps is realized — with no energy loss — by a harmonic map together with finitely many harmonic bubbles.

## Statement

> [!theorem] Min-max for harmonic maps with energy identity
> Let $\Sigma$ be a [[def-closed-manifold|closed]] surface, $M$ a closed Riemannian manifold, and $A$ a compact parameter space. Fix a continuous $h_0 : \Sigma \times A \to M$, let $H$ be the class of all maps homotopic to $h_0$, and let $k$ be the [[def-minmax-value|min-max value]]
> $$
> k \;=\; \inf_{f \in H} \, \sup_{t \in A} \, E\big(f(\cdot, t)\big),
> $$
> where $E$ is the [[def-dirichlet-energy|Dirichlet energy]] on $\Sigma$ and, if $\partial A \neq \emptyset$, the values on $\partial A$ are fixed so that the supremum cannot be attained there. Then there exist a [[def-weakly-harmonic-map|harmonic]] map $u_0 : \Sigma \to M$ and finitely many (possibly none) nonconstant [[def-conformal-map|conformal]] harmonic maps
> $$
> u_i : S^2 \to M \qquad (i = 1, \dots, m)
> $$
> with
> $$
> E(u_0) \;+\; \sum_{i=1}^{m} E(u_i) \;=\; k .
> $$
> The maps arise from a min-max sequence: there are $f_n \in H$, $t_n \in A$ and finitely many points $x_1, \dots, x_\ell \in \Sigma$ such that $f_n(\cdot, t_n) \to u_0$ weakly in the [[def-sobolev-space|Sobolev space]] $W^{1,2}(\Sigma, M)$ and uniformly on compact subsets of $\Sigma \setminus \{x_1, \dots, x_\ell\}$, and each $u_i$ is extracted by conformal rescaling around one of the $x_j$.

## Notes

> [!note]- Notes (click to expand)
> - **Checked against the book** (the source is archived locally): the statement is §4.2, the proof is completed in §4.3, resting on the local replacement result Lemma 4.1.4. The source writes the target as $N$; the lettering here follows the pool's cast ([[notation]]), where the target is always $M$. Jost describes the method as reminiscent of the curve-shortening construction of unstable closed geodesics — a saddle-point route distinct from both the Sacks–Uhlenbeck α-energy perturbation and Struwe's heat flow.
> - **The equality is the point.** Sacks–Uhlenbeck and Struwe obtain only $\le$ in the energy identity; Theorem 4.2.1's improvement is that the min-max value is fully accounted for by the limit and its bubbles — no energy is lost. This is exactly the "no loss" that makes $W = \sum_i E(u_i)$ available downstream.
> - **No index bound is stated here.** For min-max over one-parameter families, the bound $\lceil$index $\le 1\rceil$ follows as in Micallef–Moore — carded as [[thm-micallef-moore-index]].
> - **Where the graph consumes it.** This is the theorem the short extinction paper cites to realize the width by minimal spheres: specialize $\Sigma = S^2$, $A = [0,1]$ with the endpoint slices pinned at constant maps ([[def-sweepout-width]]); on $S^2$ a harmonic map is automatically conformal (its Hopf differential is a holomorphic quadratic differential on the sphere, hence zero), so $u_0$ too is a branched [[def-minimal-surface|minimal]] sphere. The carded proof of [[prop-minmax-minimal-spheres]] follows the self-contained companion-paper route instead; this card preserves the original citation route as an independent cross-check.
