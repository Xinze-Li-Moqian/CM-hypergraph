---
id: 6f08a8024b8c
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, Appendix A, Lemma A.1 and its proof (A.1)–(A.14)]]"
---

# Lemma — Index-one minimal spheres lose area no faster than 16π

A lower bound on the decay: an index-at-most-one minimal $2$-sphere loses area at rate at most $16\pi$ — the index hypothesis, run through the Hersch argument, caps the stability integral at $8\pi$.

## Statement

> [!lemma] Index-one area decay
> Let $(M, g(t))$ be a [[def-ricci-flow|Ricci flow]] on a $3$-manifold and $\Sigma \subset M$ a [[def-minimal-surface|branched minimal]] [[def-immersion|immersion]] of $S^2$ with [[def-minimal-surface-index|index]] at most one. Then the stability integral is bounded,
> $$
> \int_\Sigma \big[ |A|^2 + \operatorname{Ric}(\mathbf{n}, \mathbf{n}) \big] \;\le\; 8\pi ,
> $$
> and consequently
> $$
> \frac{d}{dt}\Big|_{t=0} \operatorname{Area}_{g(t)}(\Sigma) \;\ge\; -16\pi .
> $$

## Proof

> [!note]- Proof (click to expand)
> 1. **Bound the stability integral by $8\pi$.** By [[lem-second-eigenvalue-test]], the index hypothesis gives $\int_\Sigma |\nabla\phi|^2 \ge \int_\Sigma [|A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n)]\phi^2$ for every $\phi \perp \eta$ (all $\phi$, if stable). Take a [[def-conformal-map|conformal]] $\Phi : \Sigma \to S^2$, balance it by [[lem-hersch-balancing]] so the coordinates $\phi_i = x_i\circ\Phi$ satisfy $\int_\Sigma \eta\phi_i = 0$, apply the inequality to each and sum using $\sum_i\phi_i^2 = 1$:
> $$
> \int_\Sigma \big[ |A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n)\big] \;\le\; \sum_i \int_\Sigma |\nabla\phi_i|^2 .
> $$
> By [[lem-dirichlet-conformal-invariance]] and [[lem-round-sphere-spectrum]] the right side is $2\operatorname{Area}(S^2) = 8\pi$ — the [[thm-hersch|Hersch]] argument applied to $\Sigma$.
> 2. **Convert to area decay.** By [[lem-area-variation-jacobi]], $\frac{d}{dt}\operatorname{Area}(\Sigma) = -4\pi\chi(S^2) - \int_\Sigma[|A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n)]$. With $\chi(S^2) = 2$ and step 1,
> $$
> \frac{d}{dt}\Big|_{t=0}\operatorname{Area}(\Sigma) \;=\; -8\pi - \int_\Sigma[|A|^2 + \operatorname{Ric}(\mathbf n,\mathbf n)] \;\ge\; -8\pi - 8\pi \;=\; -16\pi . \qquad \square
> $$

## Notes

> [!note]- Notes (click to expand)
> - The two rates serve opposite ends. The [[lem-minimal-sphere-area-decay|Gauss–Bonnet bound]] $\frac{d}{dt}\operatorname{Area} \le -4\pi$ (an *upper* bound) forces decay and drives extinction; this Hersch bound $\ge -16\pi$ (a *lower* bound) limits how fast area drops — needed in the reducible case, where one tracks a stable sphere in a fixed isotopy class and must know its area cannot vanish too abruptly.
> - The index-one hypothesis is exactly what min-max delivers ([[prop-minmax-minimal-spheres]]).
