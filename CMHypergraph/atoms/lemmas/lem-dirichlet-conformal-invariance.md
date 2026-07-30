---
id: 4dc7eb0ec4ee
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, Appendix A, (A.12)]]"
  - "standard for harmonic maps of surfaces"
---

# Lemma — Conformal invariance of the Dirichlet energy in two dimensions

Energy does not see conformal stretching of a surface: precomposing a
map with a conformal diffeomorphism leaves its Dirichlet energy
unchanged — the fact that is special to dimension two.

## Statement

> [!lemma] Conformal invariance of energy ($\dim = 2$)
> Let $\Phi : (\Sigma^2, h) \to (S^2, g_{S^2})$ be a [[def-conformal-map|conformal diffeomorphism]] of surfaces and $u : S^2 \to \mathbb{R}^k$ a map. Then the [[def-dirichlet-energy|Dirichlet energies]] agree:
> $$
> \int_\Sigma |\nabla (u \circ \Phi)|_h^2 \;=\; \int_{S^2} |\nabla u|_{g_{S^2}}^2 .
> $$


## Proof

> [!note]- Proof (click to expand)
> In dimension two the Dirichlet energy density transforms by the power $\lambda^{n-2}$ of the conformal factor, which is $\lambda^0 = 1$. Explicitly: let $\Phi^* g_{S^2} = \lambda^2 h$ ($\lambda > 0$, since $\Phi$ is [[def-conformal-map|conformal]]). The energy density of $u \circ \Phi$ at $p \in \Sigma$ in the metric $h$ is
> $$
> |\nabla(u\circ\Phi)|_h^2 = h^{ij}\, \partial_i(u\circ\Phi)\,\partial_j(u\circ\Phi) = h^{ij}\, (\Phi^* \nabla u)_i (\Phi^* \nabla u)_j = (\Phi^* g_{S^2})^{ij}\lambda^2\,\cdots
> $$
> more cleanly, in $g$-orthonormal coordinates the differential $d\Phi$ scales lengths by $\lambda$, so $|\nabla(u\circ\Phi)|_h^2 = \lambda^2\, |\nabla u|_{g_{S^2}}^2 \circ \Phi$ pointwise, while the area element transforms by $d\mathrm{vol}_h = \lambda^{-2}\, \Phi^* d\mathrm{vol}_{g_{S^2}}$ (as $\Phi^* g_{S^2} = \lambda^2 h$ gives $d\mathrm{vol}_{\Phi^*g_{S^2}} = \lambda^2 d\mathrm{vol}_h$, i.e. $\Phi^* d\mathrm{vol}_{g_{S^2}} = \lambda^2 d\mathrm{vol}_h$). Hence
> $$
> \int_\Sigma |\nabla(u\circ\Phi)|_h^2\, d\mathrm{vol}_h = \int_\Sigma \big(\lambda^2 |\nabla u|^2\circ\Phi\big)\, d\mathrm{vol}_h = \int_\Sigma |\nabla u|^2\circ\Phi\; \Phi^* d\mathrm{vol}_{g_{S^2}} = \int_{S^2} |\nabla u|_{g_{S^2}}^2\, d\mathrm{vol}_{g_{S^2}},
> $$
> the two factors of $\lambda^2$ cancelling and the change of variables $\Phi$ (a diffeomorphism) finishing. $\square$

## Notes

> [!note]- Notes (click to expand)
> - Why only in dimension two: under a conformal change $h \mapsto \lambda^2 h$ on an $n$-manifold, $|\nabla u|^2$ scales by $\lambda^{-2}$ and the volume form by $\lambda^{n}$, so the energy density scales by $\lambda^{n-2}$ — invariant exactly when $n = 2$. This is the analytic miracle behind the whole harmonic-map min-max.
> - It is CM's (A.12): applied to the coordinate functions $x_i$, $\int_\Sigma |\nabla\phi_i|^2 = \int_{S^2}|\nabla x_i|^2$.
