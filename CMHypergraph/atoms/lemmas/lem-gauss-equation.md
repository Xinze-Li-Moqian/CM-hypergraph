---
id: bbb81ad6879b
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §2, equation (2.3)]]"
  - "[[ref-docarmo|do Carmo, Differential Geometry…, §6]]"
  - "[[ref-leeriemannian|Lee, Introduction to Riemannian Manifolds, ch. 8]]"
---

# Lemma — Gauss equation

The intrinsic curvature of a surface is its ambient curvature minus a bending term: what the surface feels equals what the space provides, corrected by how the surface is embedded.

## Statement

> [!lemma] Gauss equation (surface in a 3-manifold)
> Let $\Sigma \subset M$ be an [[def-immersion|immersed]] surface in a Riemannian $3$-manifold, with [[def-second-fundamental-form|second fundamental form]] $A$ and unit normal $\mathbf{n}$. Then the intrinsic Gauss curvature $K_\Sigma$ of $\Sigma$ and the ambient [[def-sectional-curvature|sectional curvature]] $K_M$ of the [[def-tangent-plane|tangent plane]] to $\Sigma$ satisfy
> $$
> K_\Sigma \;=\; K_M \;+\; \det A .
> $$
> For a [[def-minimal-surface|minimal]] surface ($\operatorname{tr} A = 0$), $\det A = -\tfrac12 [[def-second-fundamental-form-norm|\lvert A\rvert^2]]$, so
> $$
> K_\Sigma \;=\; K_M \;-\; \tfrac12 |A|^2 ,
> $$
> with $|A|^2$ (the [[def-second-fundamental-form-norm|squared norm]]) the sum of squared principal curvatures.


## Proof

> [!note]- Proof (click to expand)
> Let $\nabla$ be the ambient [[def-levi-civita-connection|connection]] and $\nabla^\Sigma$ the induced one on $\Sigma$; the Gauss formula splits $\nabla_X Y = \nabla^\Sigma_X Y + A(X,Y)\,\mathbf{n}$ for tangent $X, Y$ (the [[def-second-fundamental-form|second fundamental form]] $A$ is the normal part). Feeding this into the ambient curvature $\operatorname{Rm}(X,Y)Y = \nabla_X\nabla_Y Y - \nabla_Y\nabla_X Y - \nabla_{[X,Y]}Y$ and taking the tangential inner product with $X$ for an orthonormal tangent frame $\{e_1, e_2\}$ ($X=e_1, Y=e_2$): the ambient sectional curvature $K_M = \langle \operatorname{Rm}(e_1,e_2)e_2, e_1\rangle$ picks up, from the normal terms of the Gauss formula, exactly
> $$
> K_M = K_\Sigma - \big(A(e_1,e_1)A(e_2,e_2) - A(e_1,e_2)^2\big) = K_\Sigma - \det A ,
> $$
> where $K_\Sigma = \langle \operatorname{Rm}^\Sigma(e_1,e_2)e_2, e_1\rangle$ is the intrinsic Gauss curvature and $\det A = \kappa_1\kappa_2$ the product of principal curvatures. Rearranging, $K_\Sigma = K_M + \det A$.
> For a [[def-minimal-surface|minimal]] surface $\operatorname{tr} A = \kappa_1 + \kappa_2 = 0$, so $\kappa_2 = -\kappa_1$ and $\det A = -\kappa_1^2 = -\tfrac12(\kappa_1^2 + \kappa_2^2) = -\tfrac12|A|^2$, giving $K_\Sigma = K_M - \tfrac12|A|^2$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - $\det A$ is the product of principal curvatures — the extrinsic bending; when the surface is minimal the principal curvatures are $\pm\lambda$, so $\det A = -\lambda^2 = -\tfrac12|A|^2 \le 0$: a minimal surface is intrinsically *less* curved than its ambient plane.
> - This is CM's (2.3). Combined with $K_M = \tfrac12(R - 2\operatorname{Ric}(\mathbf{n},\mathbf{n})) + \operatorname{Ric}(\mathbf{n},\mathbf{n})$ bookkeeping it turns the first-variation integrand into intrinsic curvature plus manifestly non-negative terms — the step that lets Gauss–Bonnet act.
> - Proof debt: the Gauss equation is the tangential part of the ambient curvature tensor decomposed along $\Sigma$; classical.
