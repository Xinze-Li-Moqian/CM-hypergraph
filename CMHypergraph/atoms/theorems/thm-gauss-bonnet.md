---
id: 03d3037acd7c
type: theorem
references:
  - "[[ref-docarmo|do Carmo, Differential Geometry of Curves and Surfaces, §4.5]]"
  - "[[ref-leeriemannian|Lee, Introduction to Riemannian Manifolds, ch. 9]]"
  - "[[ref-coldingminicozzi|The branched version: Colding & Minicozzi, §2]]"
---

# Theorem — Gauss–Bonnet

Topology fixes the total curvature: however a closed surface is bent,
its curvature integrates to $2\pi$ times its Euler characteristic —
the oldest local-to-global theorem, and the ultimate source of the
$4\pi$ that extinguishes the Ricci flow.

## Statement

> [!theorem] Gauss–Bonnet
> Let $(\Sigma, g)$ be a closed oriented Riemannian surface with Gauss curvature $K$ — its own [[def-sectional-curvature|sectional curvature]]. Then
> $$
> \int_\Sigma K \, dA \;=\; 2\pi\, \chi(\Sigma),
> $$
> where $\chi$ is the Euler characteristic. For a *branched* surface — a [[def-branched-immersion|branched conformal immersion]] with branch points $p_i$ of orders $b_i > 0$ — the identity gains the branching:
> $$
> \int_\Sigma K \, dA \;=\; 2\pi \Big( \chi(\Sigma) + \sum_i b_i \Big).
> $$


## Proof

> [!note]- Proof (click to expand)
> **Smooth case, via the connection.** Choose a global unit tangent frame off a single point $p$ (possible on $S^2 \setminus \{p\}$, contractible), with connection $1$-form $\omega$ ($\nabla e_1 = \omega\, e_2$). The Gauss curvature is $K\, d\mathrm{vol} = d\omega$ (definition of curvature of the connection). By Stokes on $\Sigma \setminus B_\epsilon(p)$,
> $$
> \int_{\Sigma \setminus B_\epsilon(p)} K\, d\mathrm{vol} = \int_{\Sigma\setminus B_\epsilon} d\omega = -\int_{\partial B_\epsilon} \omega \;\to\; 2\pi\, (\text{winding of the frame around } p) = 2\pi\, \chi(\Sigma)
> $$
> as $\epsilon \to 0$: the total turning of the frame around a small loop is $2\pi$ times the index of the frame's singularity, and the sum of such indices is $\chi(\Sigma)$ by Poincaré–Hopf. For general triangulated $\Sigma$ this is the angle-excess form $\sum(\text{interior angle excess}) = 2\pi\chi$; either way $\int_\Sigma K = 2\pi\chi(\Sigma)$.
> **Branched case.** A branch point of order $b_i$ is a cone point where the surface wraps $b_i + 1$ times: the frame acquires an extra turning of $2\pi b_i$ there. Poincaré–Hopf gains $\sum_i b_i$, giving $\int_\Sigma K\, d\mathrm{vol} = 2\pi\big(\chi(\Sigma) + \sum_i b_i\big)$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - For the sphere, $\chi(S^2) = 2$: the total curvature of any metric sphere is exactly $4\pi$. This single number is the extinction rate of [[lem-minimal-sphere-area-decay]] and hence the $-4\pi$ of [[thm-width-evolution]] — and branch points, adding $2\pi b_i$ each, only push the total higher, which is why they "only help" in the area-decay inequality.
> - The theorem is the prototype of every local-to-global statement in this network: pointwise geometry (curvature) summed against a topological invariant. Its role here is exactly that of a conservation law.
> - Proof debt — classical: angle-excess summation over a triangulation, or Stokes on the connection form. Euler characteristic joins the ground notions.
