---
id: 1b5bc55d8eb2
type: definition
references:
  - "Standard; Simon, Lectures on Geometric Measure Theory"
---

# Definition — tangent plane and the Grassmann bundle

A point plus a direction of surface through it: the two-plane a surface
occupies in the ambient tangent space, and the bundle of all such
planes — the space a varifold lives on.

## Statement

> [!definition] Tangent plane; Grassmann bundle
> For a Riemannian manifold $M$, the *Grassmann bundle* $G_2(M)$ is the bundle over $M$ whose fibre over $x$ is the *Grassmannian* $\mathrm{Gr}(2, T_x M)$ of $2$-dimensional linear subspaces (*tangent planes*) of $T_x M$. An [[def-immersion|immersed]] surface $\Sigma \subset M$ has, at each $x \in \Sigma$, a tangent plane $T_x\Sigma \in \mathrm{Gr}(2, T_x M)$, giving the *Gauss lift* $x \mapsto (x, T_x\Sigma)$ into $G_2(M)$.

## Notes

> [!note]- Notes (click to expand)
> - A [[def-varifold|varifold]] is a measure on $G_2(M)$ precisely because it records area *tagged with its tangent plane* — the Gauss lift pushes the area measure of $\Sigma$ forward to $G_2(M)$.
> - A quadratic form's tangent-plane trace $\operatorname{tr} F - F(\mathbf n,\mathbf n)$ is a continuous function on $G_2(M)$ ($\mathbf n$ the plane's normal) — the pairing behind [[lem-varifold-quadratic-form]].
