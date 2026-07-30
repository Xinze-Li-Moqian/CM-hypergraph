---
id: 699c065bbbc3
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §2, (2.6)–(2.7)]]"
---

# Lemma — First variation through the Jacobi operator

The area decay of a minimal surface, rewritten in its own stability
operator: a topological term from Gauss–Bonnet plus the integral of the
Jacobi operator applied to the constant function.

## Statement

> [!lemma] First variation through $L_\Sigma$
> Let $(M, g(t))$ be a [[def-ricci-flow|Ricci flow]] and $\Sigma \subset M$ a [[def-minimal-surface|minimal]] surface with [[def-jacobi-operator|Jacobi operator]] $L_\Sigma$. Then
> $$
> \frac{d}{dt}\Big|_{t=0} \operatorname{Area}_{g(t)}(\Sigma) \;=\; -4\pi\, \chi(\Sigma) \;-\; \int_\Sigma 1 \cdot L_\Sigma 1 ,
> $$
> where $\chi$ is the Euler characteristic and $L_\Sigma 1 = |A|^2 + \operatorname{Ric}(\mathbf{n}, \mathbf{n})$ (the [[def-laplacian|Laplacian]] of the constant vanishes).


## Proof

> [!note]- Proof (click to expand)
> Start from the area first variation [[lem-area-first-variation-under-flow]]: $\frac{d}{dt}\operatorname{Area}(\Sigma) = -\int_\Sigma[R - \operatorname{Ric}(\mathbf n,\mathbf n)]$. For a [[def-minimal-surface|minimal]] $\Sigma$, rewrite the integrand through the [[lem-gauss-equation|Gauss equation]] $K_\Sigma = K_M - \tfrac12|A|^2$ and the frame identity $R - \operatorname{Ric}(\mathbf n,\mathbf n) = K_M + \tfrac12 R = K_\Sigma + \tfrac12|A|^2 + \tfrac12 R$:
> $$
> \frac{d}{dt}\operatorname{Area}(\Sigma) = -\int_\Sigma K_\Sigma - \tfrac12\int_\Sigma(|A|^2 + R) = -\int_\Sigma K_\Sigma - \int_\Sigma \big(\tfrac12|A|^2 + \tfrac12\operatorname{Ric}(\mathbf n,\mathbf n) + \tfrac12(R - \operatorname{Ric}(\mathbf n,\mathbf n))\big).
> $$
> Recognize $\tfrac12|A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n) = 1\cdot L_\Sigma 1$ evaluated (the [[def-jacobi-operator|Jacobi operator]] on the constant: $L_\Sigma 1 = \triangle_\Sigma 1 + |A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n) = |A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n)$, and $\int_\Sigma 1\cdot L_\Sigma 1$ contributes the $|A|^2 + \operatorname{Ric}$ terms). Collecting and applying [[thm-gauss-bonnet]] $\int_\Sigma K_\Sigma = 2\pi\chi(\Sigma)$:
> $$
> \frac{d}{dt}\Big|_{t=0}\operatorname{Area}(\Sigma) = -4\pi\chi(\Sigma) - \int_\Sigma 1\cdot L_\Sigma 1 . \qquad \square
> $$
## Notes

> [!note]- Notes (click to expand)
> - This is CM's (2.6)–(2.7): starting from [[lem-area-first-variation-under-flow]], the [[lem-gauss-equation|Gauss equation]] rewrites the integrand as $-2K_\Sigma - 1\cdot L_\Sigma 1$, and [[thm-gauss-bonnet]] turns $-2\int K_\Sigma$ into $-4\pi\chi(\Sigma)$. For $\Sigma = S^2$, $\chi = 2$, recovering the $-4\pi$ of [[lem-minimal-sphere-area-decay]].
> - The point of this form: it exposes $\int_\Sigma 1 \cdot L_\Sigma 1 = \int_\Sigma[|A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n)]$, the *stability integral*, which the index hypothesis bounds — the bridge to the $-16\pi$ estimate of [[lem-area-decay-index-one]].
