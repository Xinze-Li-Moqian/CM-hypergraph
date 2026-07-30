---
id: 393fa3eb0f25
type: lemma
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §5, Lemma `l:comp`]]"
---

# Lemma — An ODE comparison with hyperbolic growth

A convexity-type differential inequality forces hyperbolic growth: if a
non-negative function bends up at least as fast as itself (minus a
constant) and is somewhere large, its integral is at least a $\sinh$.

## Statement

> [!lemma] ODE comparison
> Let $f \ge 0$ be $C^2$ on $[-2\ell, 2\ell]$ with $f'' \ge f - a$ for a constant $a > 0$. If $\max_{[-\ell,\ell]} f \ge 2a$, then
> $$
> \int_{-2\ell}^{2\ell} f \;\ge\; 2\sqrt{2}\, a\, \sinh(\ell/\sqrt{2}) .
> $$


## Proof

> [!note]- Proof (click to expand)
> Let $x_0 \in [-\ell, \ell]$ achieve the maximum of $f$ there; by the reflection symmetry $x \mapsto -x$ assume $x_0 \ge 0$. At a maximum $f'(x_0) \ge 0$ (interior: $=0$; endpoint $x_0 = \ell$: $\ge 0$). Since $f(x_0) \ge 2a$, the hypothesis $f'' \ge f - a$ gives $f''(x_0) \ge f(x_0) - a \ge a > 0$.
> **Monotonicity on $[x_0, 2\ell]$.** Claim $f' > 0$ on $(x_0, 2\ell]$. If not, let $y > x_0$ be the first zero of $f'$. Then $f' \ge 0$ on $[x_0, y]$, so $f \ge f(x_0) \ge 2a$ there, so $f'' \ge f - a \ge a > 0$ on $[x_0, y]$ — but then $f'$ is strictly increasing on $[x_0, y]$, contradicting $f'(y) = 0 \le f'(x_0)$. So $f$ is increasing on $[x_0, 2\ell]$, hence $f \ge 2a$ there, and the hypothesis gives
> $$
> f'' \;\ge\; f - a \;\ge\; f - \tfrac12 f \;=\; \tfrac12 f \qquad \text{on } [x_0, 2\ell]. \tag{$\ast$}
> $$
> **Riccati comparison.** From $f'' \ge \tfrac12 f$, $f(x_0) \ge 2a$, $f'(x_0) \ge 0$, the standard comparison with the solution of $y'' = \tfrac12 y$ (i.e. $y = f(x_0)\cosh(t/\sqrt2)$, whose rate $1/\sqrt2$ is $\sqrt{1/2}$) gives
> $$
> f(x_0 + t) \;\ge\; f(x_0)\, \cosh(t/\sqrt2) \;\ge\; 2a\, \cosh(t/\sqrt2), \qquad t \in [0,\, 2\ell - x_0].
> $$
> **Integrate.** Since $x_0 \le \ell$, the interval $[x_0, x_0 + \ell] \subset [-2\ell, 2\ell]$, so integrating over $t \in [0, \ell]$,
> $$
> \int_{-2\ell}^{2\ell} f \;\ge\; \int_0^{\ell} 2a\,\cosh(t/\sqrt2)\, dt \;=\; 2a\sqrt2\, \sinh(\ell/\sqrt2). \qquad \square
> $$

## Notes

> [!note]- Notes (click to expand)
> - This is CM's Lemma `l:comp` (§5) — the elementary calculus core that converts the harmonic-map differential inequality [[lem-cylinder-angular-differential-inequality]] into the exponential decay of [[lem-harmonic-cylinder-decay]]. The $\sinh$ is why a long cylinder makes the middle angular energy exponentially small.
