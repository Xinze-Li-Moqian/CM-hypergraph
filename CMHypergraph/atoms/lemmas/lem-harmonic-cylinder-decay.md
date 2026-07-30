---
id: 2c51bc5e3cbe
type: lemma
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §5, Proposition `c:ann2`]]"
---

# Lemma — Angular energy decays on a long harmonic cylinder

A small-energy harmonic map on a long cylinder is almost independent of
the angle in the middle: its angular energy there is a small fraction
of the total — the analytic fact that no energy hides in a neck.

## Statement

> [!lemma] Harmonic cylinder decay
> Given $\delta > 0$ there are $\epsilon_2 > 0$ and $\ell \ge 1$ (depending on $\delta$ and $M$) such that if $u$ is a non-constant $C^3$ [[def-minimal-surface|harmonic]] map from the flat cylinder $\mathcal{C}_{-3\ell, 3\ell}$ to $M$ with [[def-dirichlet-energy|energy]] $\le \epsilon_2$, then
> $$
> \int_{\mathcal{C}_{-\ell, \ell}} |u_\theta|^2 \;<\; \delta \int_{\mathcal{C}_{-2\ell, 2\ell}} |\nabla u|^2 .
> $$

## Proof

> [!note]- Proof (click to expand)
> Set $f(t) = \int_{\{t\}} |u_\theta|^2$. By [[lem-cylinder-angular-differential-inequality]], $f'' \ge \tfrac32 f - a$ with $a = 2\sup|A|^2 \int|\nabla u|^4$; since $E(u) \le \epsilon_2$ is small, $|\nabla u|$ is small (harmonic regularity) so $a$ is small. If the conclusion failed, $\max_{[-\ell,\ell]} f$ would be a definite fraction of the total energy, in particular $\ge 2a$, and [[lem-ode-comparison-sinh]] would force $\int_{-2\ell}^{2\ell} f \ge 2\sqrt2\, a\, \sinh(\ell/\sqrt2)$ — growing exponentially in $\ell$, exceeding the total energy $\epsilon_2$ once $\ell$ is large. Choosing $\ell$ large and $\epsilon_2$ small gives the bound. $\square$

## Notes

> [!note]- Notes (click to expand)
> - This is CM's Proposition `c:ann2` (§5): the "no energy in the neck" for genuinely harmonic maps. The perturbation to $\nu$-almost harmonic maps is [[lem-almost-harmonic-cylinder-decay]].
> - The mechanism is the $\sinh$: exponential growth of any persistent angular energy is incompatible with a fixed small total, so the angular energy must decay into the middle of a long cylinder.
