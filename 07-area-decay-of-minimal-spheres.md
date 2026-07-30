---
topic: minmax-ricci-flow-extinction
type: topic
section: "7"
---

# Area decay of minimal spheres

This section produces the number the whole argument runs on: a minimal sphere sitting in a manifold moving by Ricci flow loses area at least as fast as $4\pi$ per unit time. The route to it is short and worth following, because each step explains where one piece of that number comes from.

## What minimal means

The estimate rests on how a surface bends inside a $3$-manifold — its [[def-second-fundamental-form|second fundamental form]], the trace that is the [[def-mean-curvature|mean curvature]], and the [[def-second-fundamental-form-norm|squared norm]] the estimates spend — and on the surfaces for which the bending balances out:

![[def-minimal-surface]]

## The area first variation

How the area of a fixed surface responds when the ambient metric moves by Ricci flow — the first-variation identity:

![[lem-area-first-variation-under-flow]]

The surface is held still and the metric moves underneath it. Since Ricci flow moves the metric by $-2\operatorname{Ric}$, the area element changes at a rate given by the Ricci curvature traced over the two directions tangent to the surface — that is, by the ambient scalar curvature minus the Ricci curvature in the normal direction. Nothing about minimality has been used yet; this is true of any surface.

The Gauss equation converts the ambient integrand into an intrinsic one:

![[lem-gauss-equation]]

This is where minimality is spent, and it is the step that makes the argument work. The integrand so far is ambient — it asks about the curvature of $M$ in a direction off the surface, which is not something the flow controls uniformly. The Gauss equation trades it for data the surface itself carries: its own intrinsic curvature, plus the squared norm of its second fundamental form. For a minimal surface the mean curvature vanishes, so the trade leaves no cross terms, and $|A|^2$ enters with a sign that helps rather than hurts. The ambient question has become an intrinsic one.

## The −4π rate

Gauss–Bonnet on the sphere then extracts the topological $-4\pi$:

![[thm-gauss-bonnet]]

The intrinsic curvature is now integrated over the whole surface, and for a sphere that integral is not an estimate but an identity: $2\pi\chi(S^2) = 4\pi$, whatever the metric. This is the origin of the constant, and it is why the constant is immune to everything the flow does. The manifold can shrink, the surface can distort, the metric can degenerate — the total curvature of a sphere is $4\pi$ because the surface is a sphere.

What is left over is the scalar-curvature term, and it is the only part of the estimate that depends on the geometry rather than the topology:

![[lem-minimal-sphere-area-decay]]

So the decay splits cleanly in two. A fixed topological loss of $4\pi$ per unit time, which nothing can weaken; and a correction proportional to the area and to the worst scalar curvature in the manifold, which the previous section's maximum principle will show fades like $1/t$. The next section does nothing but let those two race.

## The stability operator and index

The second-variation data — the [[def-jacobi-operator|Jacobi operator]] and the [[def-minimal-surface-index|index]]. The realization theorem delivers spheres of index at most one; the sharp rate of the reducible case is where that bound is spent.

![[lem-area-variation-jacobi]]
