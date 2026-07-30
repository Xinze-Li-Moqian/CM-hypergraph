---
id: 8a4ec87bb645
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, Appendix A, (A.3)–(A.6)]]"
---

# Lemma — Index one bounds the stability integral on a hyperplane

What an index-at-most-one minimal surface still controls: on the
functions orthogonal to its single unstable direction, the stability
form is nonnegative — a test-function inequality.

## Statement

> [!lemma] Index one on the orthogonal complement
> Let $\Sigma$ be a closed [[def-minimal-surface|minimal]] surface of [[def-minimal-surface-index|index]] at most one, with [[def-jacobi-operator|Jacobi operator]] $L_\Sigma = \triangle_\Sigma + |A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n)$. If the index is one, let $\eta > 0$ be a first [[def-eigenvalue|eigenfunction]]. Then for every $\phi$ with $\int_\Sigma \eta\phi = 0$,
> $$
> \int_\Sigma |\nabla\phi|^2 \;\ge\; \int_\Sigma \big[ |A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n) \big]\, \phi^2 .
> $$
> If the index is zero (stable), the inequality holds for *all* $\phi$.


## Proof

> [!note]- Proof (click to expand)
> Write $Q(\phi) = \int_\Sigma \big(|\nabla\phi|^2 - (|A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n))\phi^2\big) = -\int_\Sigma \phi\, L_\Sigma\phi$ for the quadratic form of the [[def-jacobi-operator|Jacobi operator]]. Its negative eigenvalues, counted with multiplicity, are the [[def-minimal-surface-index|index]].
> **Index zero (stable).** By definition of index $0$, $Q(\phi) \ge 0$ for all $\phi$ — which is the claim without restriction.
> **Index one.** There is exactly one direction of negativity: let $\eta$ be a first [[def-eigenvalue|eigenfunction]] ($L_\Sigma\eta + \lambda_1\eta = 0$, $\lambda_1 < 0$), which does not change sign, so take $\eta > 0$. The variational characterization of the *second* eigenvalue is
> $$
> \lambda_2 = \inf\Big\{ \tfrac{Q(\phi)}{\int\phi^2} : \phi \perp \eta,\ \phi \not\equiv 0\Big\}.
> $$
> Index one means exactly one eigenvalue is negative, so $\lambda_2 \ge 0$, i.e. $Q(\phi) \ge 0$ for every $\phi$ with $\int_\Sigma\eta\phi = 0$. Unwinding $Q \ge 0$: $\int|\nabla\phi|^2 \ge \int(|A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n))\phi^2$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - Restated: $-\int_\Sigma \phi L_\Sigma \phi \ge 0$ on the $L^2$-orthogonal complement of the first eigenfunction. This is CM's (A.3)–(A.6): index one means the *second* eigenvalue of $L_\Sigma$ is $\ge 0$, and the second [[def-eigenvalue|eigenvalue]]'s Rayleigh quotient is the infimum over $\phi \perp \eta$.
> - The first eigenfunction $\eta$ can be taken positive because a first eigenfunction of a Schrödinger operator does not change sign — so $\int_\Sigma \eta > 0$, and the orthogonality $\int \eta\phi = 0$ is a single linear constraint, satisfiable by the balancing of [[lem-hersch-balancing]].
