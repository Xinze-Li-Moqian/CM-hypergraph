---
id: 58bbff87ea0d
type: theorem
---

# Theorem — Finite-time extinction

## Statement

> [!theorem] Finite-time extinction
> Let $M$ be a [[def-closed-manifold|closed]] $3$-manifold whose [[def-fundamental-group|fundamental group]] is a [[def-free-product|free product]] of finite groups and infinite cyclic groups, and let $g_0$ be any Riemannian metric on $M$. Then:
>
> 1. $M$ contains no [[def-embedding|embedded]], [[def-locally-separating|locally separating]] $\mathbb{R}P^2$, so the [[def-ricci-flow-with-surgery|Ricci flow with surgery]] of [[thm-surgery-flow-exists]] with initial metric $(M, g_0)$ is defined for all $t \in [0, \infty)$;
> 2. this flow becomes extinct in finite time:
>
> $$
> \exists\, T < \infty : \quad M_t = \emptyset \ \text{ for all } t \ge T .
> $$

## Proof

> [!note]- Proof — citation chain (click to expand)
> 1. **The flow exists — conclusion 1.** By [[lem-free-product-three-manifolds]] (conclusion 1), $M$ contains no embedded locally separating $\mathbb{R}P^2$. The hypotheses of [[thm-surgery-flow-exists]] are therefore satisfied by $(M, g_0)$, and it yields a Ricci flow with surgery $({\mathcal M}, G)$ defined for all $t \in [0, \infty)$ with time-zero slice $(M, g_0)$.
> 2. **Every component carries a sweepout class.** The group hypothesis propagates: at each surgery time, conclusion 3 of [[thm-surgery-flow-exists]] presents the pre-surgery slice as a connected sum of the post-surgery components and the discarded ones, so by [[lem-free-product-three-manifolds]] (conclusion 3) and induction over the (discrete) surgery times, every component of every slice $M_t$ has fundamental group a free product of finite and infinite cyclic groups. By conclusion 2 of the same lemma no prime factor of such a component is aspherical, so [[lem-nonaspherical-sweepout-class]] provides a nontrivial class of sweepouts on every non-empty component.
> 3. **The width machine runs forever — a contradiction.** Suppose $M_t \neq \emptyset$ for all $t$. Step 2 verifies the hypothesis of [[lem-surgery-preserves-width-inequality]]: its width function $W(t) \ge 0$ is defined for all $t \in [0, \infty)$, satisfies the differential inequality of [[thm-width-evolution]] between surgery times with a fixed constant $C$, and does not increase across them — so the inequality holds on $[0, \infty)$ in the limsup-of-forward-difference-quotients sense, downward jumps only strengthening the integrated form. But [[lem-width-inequality-forces-extinction]] forbids such a $W$ from existing past a finite time $T^*(C, W(0))$.
> 4. **Extinction — conclusion 2.** Hence $M_T = \emptyset$ for some $T \le T^*$; an empty slice stays empty for all later times, so $M_t = \emptyset$ for every $t \ge T$. $\square$
## Notes

> [!note]- Notes (click to expand)
> - Perelman states the hypothesis as "no prime factor is acyclic"; that this is equivalent to the free-product condition is elementary $3$-manifold topology ([[cor-0-5]] in the pool).
> - **Two min-max routes to the proof**, structurally parallel — a width, a filling, a monotonicity formula forcing the width negative if the flow never dies:
>   1. *Loop families and curve shortening* (Perelman's third paper; the ch-18/19 route of the pool): realize a class of $\pi_3$ by a two-parameter family of loops, fill each loop by a least-area disk, and evolve the family by the curve-shortening flow — with the ramp trick to avoid its singularities. Width decreases at a definite rate.
>   2. *Sphere sweepouts and harmonic maps* (Colding–Minicozzi): min-max over $S^2$-sweepouts of the same class, filled by harmonic-map theory, giving $\frac{d}{dt} W \le -4\pi + \frac{3}{4(t+C)}\, W$ — no curve shortening needed.
>
>   Route 2 is an order of magnitude shorter in machinery and **its network is now built**: [[def-sweepout-width]] and [[def-dirichlet-energy]] (the objects), [[prop-minmax-minimal-spheres]] (the realization, debt), [[lem-minimal-sphere-area-decay]] and [[lem-scalar-curvature-lower-bound]] (the two rates, debts), [[thm-width-evolution]] (the inequality, proved as a citation chain), and [[lem-width-inequality-forces-extinction]] (the calculus, proved). What remains before this card gets its proof: the topological input (a nontrivial sweepout class from the free-product hypothesis, via $\pi_3 \neq 0$ on non-aspherical prime factors), the reduction of the hypothesis to prime decomposition, and surgery compatibility (surgeries only remove components or decrease the width). Route 1 stays as the pool-supported cross-check.
> - Pool material: [[thm-18-1]] (the extinction engine), the ch-18 curve-shrinking chain (lem-18-*), [[caozhu-cor-cz-finite-extinction-topological-classification]] as a cross-check.
