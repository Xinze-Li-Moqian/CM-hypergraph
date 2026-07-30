---
id: 9587a7ac9140
type: lemma
rigor: outline
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §5, Propositions `p:perturb`, `c:c1`]]"
---

# Lemma — Angular energy decays on an almost-harmonic cylinder

The perturbation that the min-max actually needs: the cylinder decay
survives replacing "harmonic" by "almost harmonic" — and iterating it
over many periods still loses only a controlled multiple of the energy.

## Statement

> [!lemma] Almost-harmonic cylinder decay
> Given $\delta > 0$ there is $\mu > 0$ (depending on $\delta$ and $M$) such that if $u$ is a $\mu$-[[def-almost-harmonic-map|almost harmonic]] map from $\mathcal{C}_{-3\ell, 3\ell}$ to $M$ with [[def-dirichlet-energy|energy]] $\le \epsilon_2$, then
> $$
> \int_{\mathcal{C}_{-\ell, \ell}} |u_\theta|^2 \;\le\; \delta \int_{\mathcal{C}_{-3\ell, 3\ell}} |\nabla u|^2 .
> $$
> Iterated over $m$ periods: there is $\nu > 0$ such that a $\nu$-almost harmonic $u$ on $\mathcal{C}_{-(m+3)\ell, 3\ell}$ with energy $\le \epsilon_2$ satisfies $\int_{\mathcal{C}_{-m\ell, 0}} |u_\theta|^2 \le 7\delta \int_{\mathcal{C}_{-(m+3)\ell, 3\ell}} |\nabla u|^2$.


## Proof

> [!note]- Proof outline (click to expand)
> **Perturbation.** A $\mu$-[[def-almost-harmonic-map|almost harmonic]] map $u$ is $W^{1,2}$-close (within $\mu$ on each small ball) to its [[def-harmonic-replacement|harmonic replacement]] $v$. The harmonic $v$ satisfies the decay of [[lem-harmonic-cylinder-decay]]: $\int_{\mathcal{C}_{-\ell,\ell}}|v_\theta|^2 < \tfrac\delta2\int_{\mathcal{C}_{-2\ell,2\ell}}|\nabla v|^2$. The angular energies of $u$ and $v$ differ by $O(\mu)$ (triangle inequality in $W^{1,2}$), so for $\mu$ small enough $\int_{\mathcal{C}_{-\ell,\ell}}|u_\theta|^2 \le \delta\int_{\mathcal{C}_{-3\ell,3\ell}}|\nabla u|^2$.
> **Telescoping.** For the $m$-period version, apply the one-period estimate on each of the overlapping blocks $\mathcal{C}_{-(k+3)\ell,-(k-1)\ell}$ centered along the neck; summing the geometric-decay bounds over $k = 1,\dots,m$ gives $\int_{\mathcal{C}_{-m\ell,0}}|u_\theta|^2 \le 7\delta\int_{\mathcal{C}_{-(m+3)\ell,3\ell}}|\nabla u|^2$, the constant $7$ absorbing the overlaps. $\square$

## Notes

> [!note]- Notes (click to expand)
> - These are CM's Propositions `p:perturb` and `c:c1` (§5): the harmonic decay [[lem-harmonic-cylinder-decay]] transferred to almost-harmonic maps (the harmonic replacement of an almost-harmonic map is close, so the differential inequality holds up to a controlled error), and summed over the periods of a long neck.
> - This is the analytic heart of [[thm-almost-minimizing-compactness]]: it shows the necks between body and bubbles carry vanishing angular — hence total — energy, which is the no-loss clause (B4) of [[def-bubble-convergence]].
> - Proof debt: the perturbation estimate (almost-harmonic $\Rightarrow$ differential inequality up to error) and the telescoping sum over periods.
