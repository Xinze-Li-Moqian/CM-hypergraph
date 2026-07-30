---
id: d326d9acf47f
type: theorem
references:
  - "[[ref-coldingminicozzi|Hersch (1970); the proof is the balancing argument, given in Colding & Minicozzi, Appendix A]]"
---

# Theorem — Hersch's inequality

A sharp ceiling on the first eigenvalue of the sphere: whatever metric
the $2$-sphere carries, the product of its lowest vibration frequency
and its area cannot exceed the round value $8\pi$.

## Statement

> [!theorem] Hersch's inequality
> Let $g$ be a Riemannian metric on $S^2$ and $\lambda_1(g)$ the first nonzero [[def-eigenvalue|eigenvalue]] of its [[def-laplacian|Laplacian]]. Then
> $$
> \lambda_1(g)\, \operatorname{Area}(S^2, g) \;\le\; 8\pi ,
> $$
> with equality exactly for the round metric.

## Proof

> [!note]- Proof (click to expand)
> Let $\eta$ be a first eigenfunction of $\triangle_g$, so $\lambda_1(g) = \int_{S^2}|\nabla\eta|^2 / \int_{S^2}\eta^2$, and normalize $\int_{S^2}\eta^2 = 1$.
> 1. **Balanced test functions.** Take a [[def-conformal-map|conformal diffeomorphism]] $\Phi : (S^2, g) \to (S^2, g_{\mathrm{round}})$ (uniformization), and by [[lem-hersch-balancing]] compose it with an automorphism so the coordinates $\phi_i = x_i \circ \Phi$ satisfy $\int_{S^2} \eta\, \phi_i = 0$ — the $\phi_i$ are admissible in the Rayleigh quotient for $\lambda_1$.
> 2. **Rayleigh + $\sum\phi_i^2 = 1$.** the variational characterization of the first [[def-eigenvalue|eigenvalue]] gives $\int |\nabla\phi_i|^2 \ge \lambda_1(g) \int \phi_i^2$ for each $i$; summing and using $\sum_i \phi_i^2 = 1$ (as $\Phi$ maps into $S^2$),
> $$
> \sum_i \int_{S^2} |\nabla\phi_i|^2 \;\ge\; \lambda_1(g)\, \operatorname{Area}(S^2, g) .
> $$
> 3. **Conformal invariance evaluates the left side.** By [[lem-dirichlet-conformal-invariance]], $\int|\nabla\phi_i|^2 = \int_{\mathrm{round}}|\nabla x_i|^2$, and by [[lem-round-sphere-spectrum]] the sum is $2\operatorname{Area}(S^2_{\mathrm{round}}) = 8\pi$. Hence $\lambda_1(g)\operatorname{Area}(S^2, g) \le 8\pi$. Equality forces $\Phi$ to be an isometry up to scale, i.e. $g$ round. $\square$

## Notes

> [!note]- Notes (click to expand)
> - Scale-invariant — both factors scale oppositely — so it constrains the *shape*, not the size. The three ingredients are independent: balancing makes the coordinates admissible, conformal invariance transports their energy to the round sphere, and the round spectrum $\lambda_1 = 2$ supplies the number $8\pi$.
> - Consumed by [[lem-area-decay-index-one]], whose stability integral is bounded by exactly this argument run on the minimal surface instead of on $S^2$.
