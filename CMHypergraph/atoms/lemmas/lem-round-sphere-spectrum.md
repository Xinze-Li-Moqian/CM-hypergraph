---
id: db9a4cc9146c
type: lemma
references:
  - "[[ref-coldingminicozzi|Standard spectral geometry (spherical harmonics); Colding & Minicozzi, Appendix A]]"
---

# Lemma — First eigenvalue of the round two-sphere

The lowest tone of the round sphere is 2, and its eigenfunctions are
the ambient coordinates restricted to the sphere — the fact that pins
the constant in Hersch's inequality.

## Statement

> [!lemma] $\lambda_1(S^2) = 2$
> On the unit round $2$-sphere $S^2 \subset \mathbb{R}^3$, the first nonzero [[def-eigenvalue|eigenvalue]] of the [[def-laplacian|Laplacian]] is $\lambda_1(S^2) = 2$, and its eigenspace is spanned by the restrictions of the linear coordinate functions $x_1, x_2, x_3$:
> $$
> \triangle_{S^2}\, x_i + 2\, x_i \;=\; 0 .
> $$
> Consequently $\int_{S^2} |\nabla x_i|^2 = 2 \int_{S^2} x_i^2$, and summing over $i$ (using $\sum_i x_i^2 = 1$) gives $\sum_i \int_{S^2} |\nabla x_i|^2 = 2\operatorname{Area}(S^2) = 8\pi$.


## Proof

> [!note]- Proof (click to expand)
> Let $x_i : \mathbb{R}^3 \to \mathbb{R}$ be a linear coordinate, restricted to $S^2$. As a function on $\mathbb{R}^3$, $x_i$ is harmonic ($\triangle_{\mathbb{R}^3} x_i = 0$) and homogeneous of degree $1$. For a degree-$k$ harmonic polynomial $p$ on $\mathbb{R}^n$, the spherical Laplacian of its restriction satisfies $\triangle_{S^{n-1}} p = -k(k+n-2)\, p$ (separate $\triangle_{\mathbb{R}^n}$ in polar coordinates: $\triangle_{\mathbb{R}^n} = \partial_r^2 + \tfrac{n-1}{r}\partial_r + \tfrac1{r^2}\triangle_{S^{n-1}}$, apply to $r^k p|_{S^{n-1}}$, use harmonicity). Here $n = 3$, $k = 1$: $\triangle_{S^2} x_i = -1\cdot(1 + 3 - 2)\, x_i = -2\, x_i$, so $x_i$ is an [[def-eigenvalue|eigenfunction]] with eigenvalue $2$.
> That $2$ is the *first* nonzero eigenvalue and the $x_i$ span its eigenspace is the $k=1$ case of the spherical-harmonic decomposition ($\lambda_k = k(k+1)$, multiplicity $2k+1$; $k=1$ gives $\lambda_1 = 2$, multiplicity $3$).
> Then $\int_{S^2}|\nabla x_i|^2 = -\int_{S^2} x_i \triangle_{S^2} x_i = 2\int_{S^2} x_i^2$ by integration by parts; summing over $i$ and using $\sum_i x_i^2 = 1$ on $S^2$ gives $\sum_i \int |\nabla x_i|^2 = 2\int_{S^2} 1 = 2\operatorname{Area}(S^2) = 8\pi$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - The coordinate functions are the degree-one spherical harmonics; $\lambda_k(S^2) = k(k+1)$, so $\lambda_1 = 2$. This is the exact value that makes Hersch's bound $8\pi$ (and not merely "a constant").
> - The summed identity $\sum_i \int|\nabla x_i|^2 = 2\operatorname{Area}(S^2) = 8\pi$ is CM's (A.13) — the numerical heart of [[thm-hersch]].
