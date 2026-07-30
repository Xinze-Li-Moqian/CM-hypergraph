---
topic: minmax-ricci-flow-extinction
type: topic
section: "8"
---

# The width inequality and extinction

## The two evolution facts

The estimate needs two facts about the flow. The rate constant comes from the evolution of scalar curvature:

![[thm-curvature-evolution]]

and its maximum-principle consequence — the clock behind the fading correction:

![[lem-scalar-curvature-lower-bound]]

The second is what keeps the correction term from being a real threat. Scalar curvature under Ricci flow obeys a reaction–diffusion inequality whose reaction term has a sign, so its minimum can only improve; and it improves at a definite rate, so a metric that started with scalar curvature bounded below by $-c$ has, at time $t$, a bound that decays like $1/(t + C)$. The constant $C$ records how bad the initial metric was and nothing else.

## The width inequality

These assemble into the width inequality, proved by running a near-optimal time-$t_0$ sweepout as a competitor at later times:

![[thm-width-evolution]]

The competitor argument is worth stating plainly, because it is where the previous section is spent. To bound the width at time $t_1 > t_0$ from above, one does not need the optimal sweepout at $t_1$ — any sweepout will do, since the width is an infimum. So take a sweepout that was near-optimal at $t_0$ and simply keep it, letting the metric move underneath it. Its slices are no longer near-maximal at $t_1$, but the realization theorem says the ones that matter were close to minimal spheres at $t_0$, and minimal spheres are exactly the surfaces whose area decay we can compute. The width at $t_1$ is therefore bounded by the width at $t_0$ plus the area those spheres lost — which is the inequality.

The three constants — which matter and which does not:

![[rem-width-constants]]

## Finite extinction

The inequality now closes the argument by itself, and it is worth seeing how little it takes.

![[lem-width-inequality-forces-extinction]]

The correction term is a multiple of $W/(t+C)$, so it is removed exactly by dividing through: the quantity $W(t)\,(t+C)^{-3/4}$ has derivative at most $-4\pi\,(t+C)^{-3/4}$, with the correction cancelling against the derivative of the factor. What is left is a bound with no $W$ in it at all. Integrating it, the accumulated loss grows like $(t+C)^{1/4}$ — without limit, because the exponent $3/4$ is less than $1$.

That is the whole argument. The width is an energy, so it is non-negative; the bound above says it must eventually go below any given number. Both cannot hold past a certain time, and that time depends only on $C$ and $W(0)$. The flow cannot reach it.

The $-4\pi$ is what makes this work. It is the total curvature of a sphere, so it is a topological constant: the flow shrinks the manifold, and the rate does not shrink with it. A quantity losing a fixed amount per unit time cannot last, however small it becomes.

For a smooth flow this is already the conclusion:

![[cor-no-immortal-flow]]

Surgery is what turns it into a statement about the manifolds one actually cares about. A flow with surgery is not one flow but a sequence of them, and the argument survives the transition for a reason worth naming: surgery cuts along regions of large positive scalar curvature, so it can only raise $\min R$ — the constant $C$ is never reset, and the clock keeps running across the cut. The topological hypothesis, that the fundamental group is a free product of finite and cyclic groups, is what supplies a nontrivial sweepout class in the first place and rules out the one embedded surface that would obstruct the surgery construction. Together:

![[thm-finite-time-extinction]]
