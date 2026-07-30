---
id: 6f9d0727dd6d
type: definition
references:
  - "Ambrosetti & Rabinowitz (1973); Struwe, Variational Methods, ch. II"
---

# Definition — mountain-pass critical point

A saddle found by min-max: sweep across a mountain range from one
valley to another, and the lowest possible height of the highest point
of the best crossing is a critical value — a pass, not a peak or valley.

## Statement

> [!definition] Mountain-pass value
> Let $\mathcal{F} : X \to \mathbb{R}$ be a $C^1$ functional satisfying the [[def-palais-smale|Palais–Smale condition]]. Given two points $a, b \in X$ and the family $\Gamma$ of paths from $a$ to $b$, the *mountain-pass value* is
> $$
> c \;=\; \inf_{\gamma \in \Gamma}\ \max_{s \in [0,1]} \mathcal{F}(\gamma(s)) .
> $$
> If $c$ exceeds $\max(\mathcal{F}(a), \mathcal{F}(b))$, then $c$ is a *critical value*: there is a [[def-critical-point|critical point]] $u$ with $\mathcal{F}(u) = c$.

## Notes

> [!note]- Notes (click to expand)
> - The one-parameter min-max: the critical point has [[def-minimal-surface-index|Morse index]] at most one (the sweep is the single unstable direction). This is the abstract form of the [[def-sweepout-width|width]] construction — the mountain pass of the energy over sphere sweepouts.
> - Existence of the critical point at height $c$ needs (PS); without it the min-max value need not be attained.
> - The general compact-parameter version — arbitrary $A$ in place of $[0,1]$ — is [[def-minmax-value]]; the mountain pass is its one-parameter case.
