---
id: 895a9b841840
type: definition
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §2, (2.6)–(2.8)]]"
  - "the second variation is classical, §1.7 of the CM lecture notes"
---

# Definition — Jacobi operator of a minimal surface

The Hessian of area at a minimal surface: the linear operator whose
sign decides whether a normal push raises or lowers area to second
order — stability, made into a spectrum.

## Statement

> [!definition] Jacobi operator (stability operator)
> Let $\Sigma \subset M$ be an [[def-immersion|immersed]] [[def-minimal-surface|minimal]] surface with unit normal $\mathbf{n}$. For a normal variation with speed $\phi \in C^\infty(\Sigma)$, the *Jacobi operator* (or *stability operator*) is
> $$
> L_\Sigma \phi \;=\; \triangle_\Sigma \phi \;+\; |A|^2\, \phi \;+\; \operatorname{Ric}(\mathbf{n}, \mathbf{n})\, \phi ,
> $$
> where $\triangle_\Sigma$ is the intrinsic [[def-laplacian|Laplacian]] of $\Sigma$, $|A|^2$ the [[def-second-fundamental-form-norm|squared second fundamental form]], and $\operatorname{Ric}$ the ambient [[def-ricci-curvature|Ricci curvature]].

## Notes

> [!note]- Notes (click to expand)
> - $L_\Sigma$ is the second variation of area: deforming $\Sigma$ to $\Sigma_r = \{x + r\phi(x)\mathbf{n}(x)\}$,
>   $$
>   \frac{\partial^2}{\partial r^2}\Big|_{r=0} \operatorname{Area}(\Sigma_r) \;=\; -\int_\Sigma \phi\, L_\Sigma \phi ,
>   $$
>   so a direction $\phi$ with $\int \phi L_\Sigma \phi > 0$ *lowers* area — an instability. This is CM's (2.6) and (2.8).
> - The potential $|A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n)$ collects the two ways a minimal surface can be pushed down: by its own bending and by ambient positive curvature. On a positively curved $M$ every minimal sphere is unstable — which is why min-max, not minimization, produces them.
> - $L_\Sigma$ is elliptic and self-adjoint; on a closed $\Sigma$ its spectrum is discrete and bounded below, giving the finite [[def-minimal-surface-index|index]].
